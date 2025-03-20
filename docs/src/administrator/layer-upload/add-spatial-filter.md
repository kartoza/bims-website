---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Ketab Bamniya
    - Jeremy Prior
    - Dimas Ciputra
date: 20-03-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2025, Kartoza
contact:
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Add Spatial Filter

Once you have uploaded a spatial layer, you can add it as a spatial filter for BIMS instance.

As an admin/super user, access the `Spatial Filters` page by clicking on 1️⃣ your username in the top right corner of any page and then click on 2️⃣ `Spatial Filters` on the dropdown menu.

![Add Spatial Filter 1](./img/add-spatial-filter-1.png)

## Add Spatial Filter Section

On the `Spatial Filters` page, you can add a new section, which will appear as a section tab in the map view.

![Add Spatial Filter 1](./img/add-spatial-filter-2.png)

To add a section, click on 1️⃣ the `Add new filter section` button.

![Add Spatial Filter 3](./img/add-spatial-filter-3.png)

To add a new filter section, fill in the following field:

1. Name – Enter the section name.

Once completed, click the Save button 2️⃣ to submit.

![Add Spatial Filter 4](./img/add-spatial-filter-4.png)

Your new filter section will then be added to the bottom of the list on the `Spatial Filters` page.

![Add Spatial Filter 5](./img/add-spatial-filter-5.png)

If you navigate back to the map on the BIMS instance, click 1️⃣ the `Search` button, and then click 2️⃣ `Spatial Filter`, you will see the newly created filter section.

![Add Spatial Filter 6](./img/add-spatial-filter-6.png)

If you need to change the position of your filter section in the list, go to the `Spatial Filters` page. Click and hold the drag icon, then move the section to your desired position.

![Add Spatial Filter 7](./img/add-spatial-filter-7.png)

## Add Spatial Filter Context

A spatial filter context refers to the items added under the `Spatial Filter section`. The system uses this context to retrieve data from the associated spatial layer.

For example, if you add `Sanpark boundaries` as a context 1️⃣, the system will extract Sanpark filter data using the provided key. These filters will then appear as selectable options 2️⃣ on the map.

![Add Spatial Filter 8-1](./img/add-spatial-filter-8-1.png)

![Add Spatial Filter 8-2](./img/add-spatial-filter-8-2.png)

To add a `Spatial Filter Context`, you first need to specify which attribute from the layer will be used to extract values. This requires adding a GeoContext key.

Click 1️⃣ the `GeoContext keys` button to proceed.

![Add Spatial Filter 9](./img/add-spatial-filter-9.png)

The `GeoContext Keys` modal will appear. Click the `Add New Key` button.

![Add Spatial Filter 10](./img/add-spatial-filter-10.png)

In the `Add New Key` modal:

- 1️⃣ Select a layer – Choose the layer you want to use. You can select your uploaded layer here.
- 2️⃣ Choose an attribute – Select the attribute the system will use to extract data.

Once done, click `Save`.

![Add Spatial Filter 11](./img/add-spatial-filter-11.png)

Your new context key should appear here. If you want to use a different attribute for the layer, simply remove the key by clicking the wastebasket icon and add a new one. 

![Add Spatial Filter 12](./img/add-spatial-filter-12.png)

Close the modal, and now you can add the new context to the Spatial Filter section.
To do this, click the plus (+) button 1️⃣ in the section panel.

![Add Spatial Filter 13](./img/add-spatial-filter-13.png)

In the `Add New Context` modal, locate your newly added key using the input field 1️⃣. The field supports autocomplete, so you can start typing part of the title, and it will automatically search for matching keys.
Once you've selected the key, click the `Add` button to proceed.

![Add Spatial Filter 14](./img/add-spatial-filter-14.png)

Your new context will be added to the bottom of the list.

To rearrange its position, simply drag the drag icon located to the left of the text.

![Add Spatial Filter 15](./img/add-spatial-filter-15.png)

When you return to the map view and open the `Spatial Filter` panel, you will see your newly added spatial filter context. However, no data will be available yet because the system hasn't harvested it.

You can wait for the system to harvest the data automatically, but for the current setup, it's better to trigger the harvester manually. Follow the next steps to do that.

![Add Spatial Filter 16](./img/add-spatial-filter-16.png)

As an admin/superuser, visit the following URL:

🔗 `https://[your-bims.site.com]/admin/bims/locationsite/`

This will open the Location Site Admin page.

Hover over the `Update GeoContext` button 1️⃣. A dropdown will appear with two options—select the second option 2️⃣ to avoid re-harvesting existing data.

![Add Spatial Filter 17](./img/add-spatial-filter-17.png)

Once selected, the button will change to `Harvesting GeoContext...` 1️⃣, indicating that the system is currently processing data from the layers for all location sites.

![Add Spatial Filter 18](./img/add-spatial-filter-18.png)

The harvesting process may take some time, depending on the number of sites in your BIMS instance.

To check if the process is complete, open the `Spatial Filter` panel on the map. If the sites now contain the context filter, it will be displayed there.

![Add Spatial Filter 19](./img/add-spatial-filter-19.png)