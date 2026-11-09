---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - 
date: 09-11-2026
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2026, Kartoza
contact:
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Live Layers (OGC API - Features)

Technical notes on the live layers that BIMS publishes for GIS clients. For how to publish a layer, see the [administrator guide](../../administrator/ogc-live-layers/index.md).

## Endpoints

A layer published from the BIMS filter (see the [user guide](../../administrator/ogc-live-layers/index.md)) follows OGC API - Features Part 1 (Core), with GeoJSON output. All paths are below `/ogc/layers/<token>/`:

| Path | Returns |
| -- | -- |
| `/` | Landing page with links to the other documents |
| `/api` | OpenAPI definition |
| `/conformance` | Conformance classes (core, oas30, geojson) |
| `/collections` | The list of collections (one, with id `records`) and its spatial extent |
| `/collections/records` | The `records` collection |
| `/collections/records/items?limit=1000&offset=0` | The features, as `application/geo+json` |
| `/collections/records/items/<uuid>` | A single record |

The `items` endpoint accepts `limit` (default 1000, maximum 5000), `offset`, and `bbox`. The response contains `numberMatched`, `numberReturned` and `next`/`prev` links. Example, abbreviated:

```json
{
  "type": "FeatureCollection",
  "numberMatched": 978,
  "numberReturned": 1,
  "links": [
    {"rel": "self", "href": ".../collections/records/items?limit=1&offset=0"},
    {"rel": "next", "href": ".../collections/records/items?limit=1&offset=1"}
  ],
  "features": [
    {
      "type": "Feature",
      "id": "b73a9163-12a7-4849-85fa-9a9aea60344a",
      "geometry": {"type": "Point", "coordinates": [22.916667, -32.25]},
      "properties": {"Site code": "L1BREI-00001", "Sampling date": "1978-02-15", "Kingdom": "Plantae"}
    }
  ]
}
```

The management API used by the dialog is `/api/ogc-layers/` (list, create, `preview/`, rename, `rotate-token/`, delete). It requires a logged-in user.

## Limits and protection of the server

Live layers read from the shared BIMS database, so they are limited on purpose. The defaults below can be changed by the system administrator with environment variables (see `core/settings/ogc.py`).

| Setting | Default | Meaning |
| -- | -- | -- |
| `OGC_LAYERS_ENABLED` | on | Switches every layer URL off when set to false (answers 503) |
| `OGC_LAYER_MAX_RECORDS` | 100000 | Largest layer allowed |
| `OGC_LAYER_DEFAULT_PAGE_SIZE` / `OGC_LAYER_MAX_PAGE_SIZE` | 1000 / 5000 | Records per page |
| `OGC_MAX_LAYERS_PER_OWNER` | 20 | Active layers one user may have |
| `OGC_LAYER_STATEMENT_TIMEOUT` | 20 s | A layer query is cancelled after this time |
| `OGC_LAYER_MAX_CONCURRENT_EVALUATIONS` | 4 | Layers evaluated at the same time, per tenant |
| `OGC_RATE_LIMIT_IP` / `_LAYER` / `_OWNER` | 600 / 1200 / 2400 per minute | Rate limits. A client over the limit receives 429 with `Retry-After` |
| `OGC_LAYER_MAX_FAILURES` | 5 | A layer is switched off after this many timeouts in a row |
| `OGC_HTTP_CACHE_MAX_AGE` | 60 s | How long a client may reuse a response |

A busy server answers 503 with `Retry-After`; clients normally retry on their own. A revoked, deleted or unknown token answers 404.
