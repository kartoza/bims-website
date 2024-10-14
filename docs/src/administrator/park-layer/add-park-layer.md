---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Dimas Ciputra
date: 14-10-2024
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2024, Kartoza
contact:
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Adding a Park Layer to the "Add Site" Form

This guide will help you fetch the park name from a spatial layer on the "Add Site" form, following the steps outlined below:

![Inline image](img/Screenshot%202024-10-14%20at%2014.53.44.png)

## Step 1: Upload the Layer

As a superuser, navigate to the layer upload page at /upload-spatial-layer/ to upload your shapefiles. When prompted, give the layer an appropriate name based on your needs.

![Inline image](img/Screenshot%202024-10-14%20at%2014.48.33.png)

After uploading, wait until the process is completed. The upload status will change to "Success" once it's finished.

## Step 2: Select the Layer in Site Settings

Next, go to the admin page and select Site Setting by visiting /admin/bims/sitesetting/. Click on the first setting that appears.

Scroll down to find the Park Layer dropdown, and choose the layer you just uploaded.

## Step 3: Set the Park Attribute Key

Set the Park Attribute Key to specify the attribute you want to use when selecting park names from the layer’s properties.

Once all these settings are configured, click Save.

![Inline image](img/Screenshot%202024-10-14%20at%2014.52.03.png)

Once all these settings are configured, click Save.
