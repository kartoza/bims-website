---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Jeremy Prior
    - Ketan Bamniya
date: 26-09-2023
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Biodiversity Data Dashboard

The Single Site - Invertebrates dashboard provides a detailed view of data and insights for a selected site.

[![Dashboard](./img/dashboard-img-1.png)](./img/dashboard-img-1.png)

1. **[![Close Icon](./img/dashboard-img-2.png)](./img/dashboard-img-2.png):** The button at the top-right corner allows users to close the dashboard window.

2. **Filter History:** The Filter History section provides a detailed summary of the filters applied to generate the dashboard view. This section ensures transparency and clarity about the data presented by including the following details:

    * **Search Query:** Displays the unique query identifier used to retrieve data.

    * **Site ID:** Provides the identification code of the site, serving as a reference for the selected location.

    * **Ecosystem Type:** Lists the types of ecosystems associated with the site, such as rivers, wetlands, or open water bodies.

    * **Data Source:** Indicates the sources of data used in the dashboard, including FBIS, GBIF, and the Virtual Museum.

3. **Occurrence Charts:** Visualises key occurrence metrics in pie chart format.
    * **Categories:**

        * **Origin:** Displays whether species are native or introduced.

        * **Endemism:** Indicates the distribution range.

        * **Conservation Status Global:** Highlights specie's conservation status at the global level.
        
        * **Conservation Status National:** Highlights specie's conservation status at the national level.

        * **Sampling Method:** Details the data collection methodology.

        * **Biotope:** Represents habitat or ecological zones.

4. **[![Download Icon](./img/dashboard-img-3.png)](./img/dashboard-img-3.png):** This feature allows users to download specific sections of the data visualisation chart in SVG format.

* This is how the downloaded data will look like:

    [![Downloaded Data](./img/dashboard-img-4.png)](./img/dashboard-img-4.png)

5. **Distributions:** Provides a geographical representation of the site's location on the interactive map.

    [![Map](./img/dashboard-img-5.png)](./img/dashboard-img-5.png)

    * **[![Download Icon](./img/dashboard-img-6.png)](./img/dashboard-img-6.png):** Allows users to download the map.

        [![Download Distribution Map](./img/dashboard-img-7.png)](./img/dashboard-img-7.png)

        * **Purpose:** Users can select their purpose for downloading the data from this drop-down menu, with options such as scientific articles, reports, theses, or other predefined categories. Custom purposes cannot be added, as users can only choose from the available options.

        * **Notes:** Adding additional notes to accompany the downloaded data is optional but available for users who wish to include them.

        * **Download:** Once the purpose and notes are selected, users can proceed to download the map.

        * **Close:** Users can close the download window by clicking the close button.

    * **`➕` and `➖`:** Users can zoom in and out of the map by clicking the `➕` and `➖` buttons respectively.

* **Display Dashboard Data:** Users can select whether they want to view annually or monthly data using this dropdown menu. 

    * **Annually:** If users select this option, the graph will display only the year in which the data was captured.

        [![Annually Data](./img/dashboard-img-33.png)](./img/dashboard-img-33.png)

    * **Monthly:** If users select this option, the graph will display the year along with the month and date on which the data was captured.

        [![Monthly Data](./img/dashboard-img-34.png)](./img/dashboard-img-34.png)

6. **Occurrences:** Displays a bar chart representing the occurrences of invertebrates.

    * **[![Download Icon](./img/dashboard-img-6.png)](./img/dashboard-img-6.png):** Allows users to download the occurrences.

        [![Download Distribution Map](./img/dashboard-img-9.png)](./img/dashboard-img-9.png)

        * **Purpose:** Users can select their purpose for downloading the data from this drop-down menu, with options such as scientific articles, reports, theses, or other predefined categories. Custom purposes cannot be added, as users can only choose from the available options.

        * **Notes:** Adding additional notes to accompany the downloaded data is optional but available for users who wish to include them.

        * **Download:** Once the purpose and notes are selected, users can proceed to download the data.

            * This is how the downloaded data will look like:

                [![Download Occurrences Data](./img/dashboard-img-8.png)](./img/dashboard-img-8.png)

        * **Close:** Users can close the download window by clicking the close button.

7. **Overview:** This section provides an overview of the site.

    **[![Download Icon](./img/dashboard-img-6.png)](./img/dashboard-img-6.png):** Allows users to download the overview.

    * **Site details:** This section offers detailed information about the site, including its unique code, geographical location, and other pertinent attributes necessary for comprehensive understanding.

        [![Site Details](./img/dashboard-img-10.png)](./img/dashboard-img-10.png)

    * **Ecosystem Characteristics:** This section offers detailed insights into the ecosystem characteristics of the site, including its unique type, wetland name, and environmental significance.

        [![Ecosystem Characteristics](./img/dashboard-img-11.png)](./img/dashboard-img-11.png)

    * **Province, Ecoregion and Water Source Area:** This section provides comprehensive information about the site, including its province, ecoregion, and associated water source area, highlighting its geographical and ecological context.

        [![Province, Ecoregion and Water Source Area](./img/dashboard-img-12.png)](./img/dashboard-img-12.png)

    * **Catchment:** This section provides information about the catchment of the site.

        [![Catchment](./img/dashboard-img-13.png)](./img/dashboard-img-13.png)

    * **Climate, Vegetation and Soils:** This section offers detailed information about the site's climate, vegetation, and soil characteristics, highlighting the environmental factors and natural features that define the area.

        [![Climate Vegetation Soils](./img/dashboard-img-14.png)](./img/dashboard-img-14.png)

    * **Protected Areas:** This section provides information about the protected areas of the site.

        [![Protected Areas](./img/dashboard-img-15.png)](./img/dashboard-img-15.png)

    * **Management Area:** This section offers detailed insights into the site's management area, including its water management area, river management units, and relevant management practices.

        [![Management Area](./img/dashboard-img-16.png)](./img/dashboard-img-16.png)

    * **National Biodiversity Assessment:** This section provides detailed information about the site's national biodiversity assessment, including its ecological importance, conservation priorities, and biodiversity status within a national context.

        [![National Biodiversity Assessment](./img/dashboard-img-17.png)](./img/dashboard-img-17.png)

    * **Species and Occurrences:** This section provides information about the species and their occurrences on the site.

        [![Species And Occurrences](./img/dashboard-img-18.png)](./img/dashboard-img-18.png)

8. **Taxa:** Displays taxa data for the site. Displays a list of the first 25 taxa if the total number exceeds 25.

[![Dashboard 2](./img/dashboard-img-19.png)](./img/dashboard-img-19.png)

1. **Origin:** Displays the origin of the taxa in a graphical form.

2. **Endemism:** Displays the endemism of the taxa in a graphical form.

3. **Conservation Status:** Displays the conservation status of the taxa in a graphical form.

## Site Visit Data

[![Site Visit Data](./img/dashboard-img-20.png)](./img/dashboard-img-20.png)

* **Recent site visit:** It displays the recent site visit data, including the site code, visit date, and total records.

* **See more site visit:** By clicking on this button users will be redirected to the new page where thy can see all the site visit data.

## Occurrence Data

Displays the occurrence data of the species.

[![Occurrence Data](./img/dashboard-img-21.png)](./img/dashboard-img-21.png)

* **[![Download Icon](./img/dashboard-img-6.png)](./img/dashboard-img-6.png):** Allows users to download the occurrence data.

    [![Download Occurrence Data](./img/dashboard-img-22.png)](./img/dashboard-img-22.png)

    * **Purpose:** Users can select their purpose for downloading the data from this drop-down menu, with options such as scientific articles, reports, theses, or other predefined categories. Custom purposes cannot be added, as users can only choose from the available options.

    * **Notes:** Adding additional notes to accompany the downloaded data is optional but available for users who wish to include them.

    * **Download:** Once the purpose and notes are selected, users can proceed to download the data.

        * This is how the downloaded data will look like.

            [![Downloaded Occurrence Data](./img/dashboard-img-23.png)](./img/dashboard-img-23.png)

    * **Close:** Users can close the download window by clicking the close button.

* **Download data:** Users can download the occurrence data in csv or excel format.

* **Download checklist:** Users can download the checklist in CSV, Excel, or PDF format. When this button is clicked, it will change to a processing button to indicate that the process has started.

    [![Processing](./img/dashboard-img-25.png)](./img/dashboard-img-25.png)

    * User will encounter this window after clicking on the download button.

        [![Download Checklist](./img/dashboard-img-27.png)](./img/dashboard-img-27.png)

        * **Purpose:** Users can select their purpose for downloading the data from this drop-down menu, with options such as scientific articles, reports, theses, or other predefined categories. Custom purposes cannot be added, as users can only choose from the available options.

        * **Notes:** Adding additional notes to accompany the downloaded data is optional but available for users who wish to include them.

        * **Format:** Users can select the format of the checklist, with options such as csv, excel, or pdf.

        * **Download:** Once the purpose and notes are selected, users can proceed to download the data.

            * After clicking on download, the user will receive a notification stating that they will be emailed once the download is completed.

                [![Alert Message](./img/dashboard-img-24.png)](./img/dashboard-img-24.png)

                * This is the email users will going to receive on their registered email with the attached checklist file.

                    [![Email](./img/dashboard-img-26.png)](./img/dashboard-img-26.png)

                    1 **File:** Hover over this file, then click the download icon to download it. The downloaded file will be in ZIP format as it contains multiple files.

    * **Close:** Users can close the download window by clicking the close button.

* **Download GBIF ids:** Allows users to download GBIF ids.

## Metadata Table

[![Metadata Table](./img/dashboard-img-29.png)](./img/dashboard-img-29.png)

* **[![Download Icon](./img/dashboard-img-6.png)](./img/dashboard-img-6.png):** Allows users to download the metadata.

[![Download Metadata Table](./img/dashboard-img-30.png)](./img/dashboard-img-30.png)

* **Purpose:** Users can select their purpose for downloading the data from this drop-down menu, with options such as scientific articles, reports, theses, or other predefined categories. Custom purposes cannot be added, as users can only choose from the available options.

* **Notes:** Adding additional notes to accompany the downloaded data is optional but available for users who wish to include them.

* **Download:** Once the purpose and notes are selected, users can proceed to download the data. This will download the metadata table in png format.

    * This is the downloaded metadata.

        [![Downloaded Metadata Table](./img/dashboard-img-31.png)](./img/dashboard-img-31.png)

* **Close:** Users can close the download window by clicking the close button.

## Export Dashboard to Image

Users can export the dashboard as image in their system by clicking on `Export Dashboard to Image` button located at the bottom of the dashboard page.

[![Export Dashboard](./img/dashboard-img-32.png)](./img/dashboard-img-32.png)
