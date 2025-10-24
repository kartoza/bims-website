---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Helen Dallas
    - Jeremy Shelton
    - Jeremy Prior
    - Nazley Liddle
date: 17-10-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Harvesting GBIF data

All existing taxon occurrence data are harvested per Taxon Group from the Global Biodiversity Information Facility (GBIF). This section outlines the steps for harvesting GBIF data.

Only registered users with **super user status** are able to do this, typically the administrators .

The Master List of Taxa for a Taxon Group is used to facilitate harvesting of data from GBIF, thereby ensuring that the correct taxa are included on the information system.

## Steps

Click on your profile and select **Harvest from GBIF**.

![Harvesting GBIF data 1](./img/harvesting-gbif-data-1.png)

Select the Taxon Group using the dropdown and click Start harvesting.

![Harvesting GBIF data 2](./img/harvesting-gbif-data-2.png)

You can keep track of progress. The more taxa in the master list, the longer the time needed for harvesting data from GBIF. You can keep it running in the background and continue with other work as it harvests the data.

![Harvesting GBIF data 3](./img/harvesting-gbif-data-3.png)

You can view the GBIF data harvested via the **Download Logs**.

![Harvesting GBIF data 4](./img/harvesting-gbif-data-4.png)

# Setting up GBIF harvest schedules

There is also functionality for users to set up harvesting schedules to download occurrences and species from GBIF automatically in the backend. 

To set up a harvesting schedule, visit the Admin page > BIMS > Harvest schedules

Click '+ Add harvest schedule'

![Harvesting GBIF data 5](./img/harvesting-gbif-data-5.png)

Choose the biodiversity module or group from the dropdowns available.

![Harvesting GBIF data 6](./img/harvesting-gbif-data-6.png)

Set the period:

![Harvesting GBIF data 7](./img/harvesting-gbif-data-7.png)

- Weekly: specify the day(s) of the week. You can also use values like mon, tues or 0-6 (where 0 = Sunday).
- Monthly: specify the date (eg., 15 for the 15th)
- Custom (cron): enter a cron expression. This option is mainly for developers, but it allows more flexibility (e.g., hourly, every 30 mins)

Add the run time. The task will be triggered at this hour (UTC timezone).

![Harvesting GBIF data 8](./img/harvesting-gbif-data-8.png)

Configure the defaults from the job section (these are for the harvest session settings).

Set the boundary.

Check 'Is fetching species' if you want to harvest species.

**Note:**
- Only 3 harvest sessions can run at a time per BIMS instance.
- If you want to harvest species, make sure the GBIF parent species is added to the module group, just like when a user harvests species.
