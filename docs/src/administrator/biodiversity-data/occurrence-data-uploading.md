---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Helen Dallas
    - Jeremy Shelton
    - Jeremy Prior
    - Nazley Liddle
date: 22-07-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Uploading Occurrence Data

## Steps:

Click on your profile and select **Upload Occurrence Data**

![Occurrence Data Uploading 1](./img/occurrence-data-uploading-1.png)

Select the Taxon Group using the dropdown and browse to the file containing the occurrence data for the taxon group, click upload

![Occurrence Data Uploading 2](./img/occurrence-data-uploading-2.png)

![Occurrence Data Uploading 3](./img/occurrence-data-uploading-3.png)

Progress is shown:

![Occurrence Data Uploading 4](./img/occurrence-data-uploading-4.png)

A **Success** file will indicate occurrence records uploaded to the system. An **Error** file will give details of occurrence records not uploaded. The last column in this csv file provides an indication of the reason the occurrence record was not uploaded. The administrator then needs to check the data and correct before uploading again.

**Common errors:**

* Taxon not in Master list
* Taxon Rank incorrect

Occurrence records may be updated by uploaded corrected records in the csv file. As long as the UUID is the same then the old occurrence record will be updated.

New occurrence records may be added by repeating the steps from (4), to upload the additional occurrence records for the Taxon Group.

Note that once the occurrence data has been uploaded, geocontext data (i.e. information about the site such as province, catchment etc.) are automatically populated for each site. This takes time and it is recommended that the next step (i.e. harvesting from GBIF), is done at least 24 hours after uploading occurrence data.
