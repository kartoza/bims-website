---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Helen Dallas
    - Jeremy Shelton
    - Jeremy Prior
    - Nazley Liddle
date: 20-11-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Managing BIMS Admin tables

Several backend tables can be updated and managed by administrators, including the Biodiversity Information Management System (BIMS), and are accessible via the Admin Page. Here we provide a list of actions related to the Site Administration including the BIMS table management that an administrator (super user status) may need to edit or check. Only the tables that the administrator needs to be able to revise have been described, and not all the tables in the Site Administration and BIMS. They are described chronologically as they appear in Site Administration. This document will continually need to be updated as new administration functions are added.

**Link to specific sub-sections in BIMS as well as other admin tasks:**

**Managing BIMS Admin tables**

- [Managing BIMS Admin tables](#managing-bims-admin-tables)
- [Site administration](#site-administration)

  - [BIMS: Abundance types](#bims-abundance-types)
  - [BIMS: Base map layers](#bims-base-map-layers)
  - [BIMS: Biological collection records](#bims-biological-collection-records)
  - [BIMS: Biotopes](#bims-biotopes)
  - [BIMS: Chemistry records](#bims-chemistry-records)
  - [BIMS: Chemistry units](#bims-chemistry-units)
  - [BIMS: Datasets](#bims-datasets)
  - [BIMS: Decision Support Tool Names and Decision Support Tools](#bims-decision-support-tool-names-and-descision-support-tools)
  - [BIMS: Download request purposes](#bims-download-request-purposes)
  - [BIMS: Download requests](#bims-download-requests)
  - [BIMS: Endemism](#bims-endemism)
  - [BIMS: Harvest schedules](#bims-harvest-schedules)
  - [BIMS: Harvest sessions](#bims-harvest-sessions)
  - [BIMS: Hydroperiods](#bims-hydroperiods)
  - [BIMS: IUCN status](#bims-iucn-status)
  - [BIMS: Layer groups](#bims-layer-groups)
  - [BIMS: Location context filter group orders](#bims-location-context-filter-group-orders)
  - [BIMS: Location context filter](#bims-location-context-filter)
  - [BIMS: Location context groups](#bims-location-context-groups)
  - [BIMS: Location sites](#bims-location-sites)
  - [BIMS: Non-biodiversity layers](#bims-non-biodiversity-layers)
  - [BIMS: Notifications](#bims-notifications)
  - [BIMS: Record types](#bims-record-types)
  - [BIMS: Roles](#bims-roles)
  - [BIMS: Sampling effort measure](#bims-sampling-effort-measure)
  - [BIMS: Sampling methods](#bims-sampling-methods)
  - [BIMS: Site settings](#bims-site-settings)
  - [BIMS: Source references](#bims-source-references)
  - [BIMS: Tag groups](#bims-tag-groups)
  - [BIMS: Taxa](#bims-taxa)
  - [BIMS: Taxon groups](#bims-taxon-groups)
  - [BIMS: Wetland indicator status](#bims-wetland-indicator-status)
- [Flat pages](#flat-pages)
  - [Flat pages: about us](#flat-pages-about-us)
  - [Flat pages: citation guidelines](#flat-pages-citation-guidelines)
  - [Flat pages: Help](#flat-pages-help)
- [People](#people)
  - [People: Users](#people-users)
  - [FBIS user sign up procedure](#fbis-user-sign-up-procedure)
  - [Managing users](#managing-users)

## Site administration

There are five tools to allow administrators to maintain the general integrity of the platform and perform broad admin tasks. These include: 

![site-administration-1](img/site-administration1.png)

**A description of each is provided below:**

**Clear Cache:** This clears the temporary storage area and is useful to clear data that been added or modified. Examples: Clear Cache after harvesting GBIF occurrence records, Clear Cache after renaming a Site Code.

**Delete dangling sites:** This deletes Sites and Surveys (Site Code + Sampling Date) that have no biodiversity occurrence data, physico-chemical data or water temperature associated with them. Admin receives emails confirming the number of Sites and Surveys deleted. 

![site-administration-2](img/site-administration2.png)

**Harvest IUCN Status:** This starts a full harvest of the IUCN global conservation status for all taxa on the platform. 

**Clear taxa not in group:** This allows admin to clean up the BIMS>Taxa table, by deleting all taxa that are not associated with a Taxon Group/Biodiversity Module. If the "Dry run" is ticked, then no taxa will be deleted and admin can check a subset of data before running the delete. It provides a breakdown of the total number of taxa, taxa linked to a group, taxa with ancestors, taxa with occurrences, and candidates to delete. One can then run the "Clear taxa in group", with "Dry run" unchecked, to clean up and delete the candidate taxa. 

![site-administration-3](img/site-administration3.png)

**Remove sites outside boundary:** This allows admin to delete sites that have been harvested from GBIF, but which fall outside of the spatial boundary of the platform.  If the “Dry run” is ticked, then no sites will be deleted and admin can check a subset of sites before running the delete. It provides a breakdown of the sites outside the boundary, GBIF occurrence to be deleted, Surveys and Sites deleted, and sample site codes that admin can then check. One can then run the “Remove sites outside boundary”, with the “Dry run” unchecked, to clean up and delete the candidate taxa. Normally this is only needed if the boundary has been changed. 

![site-administration-4](img/site-administration4.png)

## BIMS: Abundance types

Here you manage the abundance measure (type) such as number, percentage etc. New abundance measures (type) can be added.

![abundance types](img/abundance-types.png)

## BIMS: Base map layers

Here you can see and manage the base maps visible on the platform. The defaults base map can be selected. 

![base map layers](img/base-map-update.png)

## BIMS: Biological collection records

Here you can see all biological collection records. Individual sites can be searched for and filters applied. 

![biological collection records](img/biological-collection-records.png)

## BIMS: Biotopes

Here you manage the broad biotope categories, description and order; the specific biotope categories, description and order; and the substratum.  These biotopes are initially populated by the biodiversity data upload files, where each biotope is specified in the dropdowns. Details are provided below. Certain biotopes and substrata may be associated with one or more modules.  As more biodiversity modules are added, it may be necessary for the administrator to update biotopes.

| Module | Broad Biotope | Specific Biotope | Substratum |
| -- | -- | -- | -- |
| All | Unspecified |  |  |
| All | Mixed |  |  |
| Algae, invertebrates, anurans | Stones In Current |  |  |
| Algae, invertebrates, anurans | Stones Out Of Current |  |  |
| Algae, invertebrates, anurans | Marginal Vegetation |  |  |
| Algae, invertebrates, anurans | Aquatic Vegetation |  |  |
| Algae, invertebrates, anurans | Gravel/Sand/Mud |  |  |
| Algae, invertebrates | Artificial substrate |  |  |
| Fish only | Slow-Shallow |  |  |
| Fish only | Slow-Deep |  |  |
| Fish only | Fast-Shallow |  |  |
| Fish only | Fast-Deep |  |  |
| All |  | Backwater |  |
| All |  | Bedrock |  |
| All |  | Cascade |  |
| All |  | Chute |  |
| All |  | Detritus |  |
| All |  | Mixed |  |
| All |  | Pool |  |
| All |  | Rapid |  |
| All |  | Riffle |  |
| All |  | Run |  |
| All |  | Slackwater |  |
| All |  | Unspecified |  |
| All |  | Waterfall |  |
| All |  |  | Unspecified |
| All |  |  | Mixed |
| All |  |  | Bedrock |
| All |  |  | Boulder |
| All |  |  | Cobble |
| All |  |  | Detritus |
| All |  |  | Gravel |
| All |  |  | Pebble |
| All |  |  | Sand |
| All |  |  | Silt/Mud/Clay |

If these have not been included in the data occurrence upload files, then they are blank. New biotopes can be added by clicking the “+ Add biotope”.

## BIMS: Chemistry records

Here you can see all chemical records. Individual sites can be searched for and filters applied. 

![chemistry records](img/chemistry-records.png)

## BIMS: Chemistry units

Here you manage the physico-chemical data including the Chem Code (**NB this needs to match the column in the physico-chemical data upload template**), chem description, chem unit, whether the variable needs to be shown in abiotic form (abiotic list), minimum and maximum values. New chemistry units can be added by clicking the “+ Add chemistry unit”.

![Chemistry units 1](img/chemistry-units-1.png)

Changes can be made to each variable by clicking on the relevant **Chem code** and editing the appropriate field. Here one can also specify the number of decimal places.

![Chemistry units 2](img/chemistry-units-2.png)

## BIMS: Datasets

When occurrence data are harvested from GBIF, the datasets that comprise the data are stored in the Datasets table. When the system is harvesting occurrences data from GBIF, it will automatically update the dataset table. To manually update the dataset table, click `Fetch Datasets`. Here you can add an abbreviation for the dataset so that when the citation is pulled down in the checklist, the abbreviation is provided. 

![Datasets](img/datasets-1.png)

Details for each dataset can be viewed by clicking the UUID. The dataset Name, description, citation and URL are provided. 

![Change dataset](img/datasets-2.png)

## BIMS: Decision Support Tool Names and Decision Support Tools

Here you manage the decision support tools that are added and what they are called. Individual UUIDs are assigned specific decision support name.

![Decision support tool](img/decision-support-tool.png)

## BIMS: Download request purposes

Here you manage the download request purposes that a user chooses when requesting a download of a graph or csv file. New purposes can be added by selecting “Add download request purpose” and the sort order can be updated.

When a system is first set up the administrator needs to add Download request purposes here before users are able to download information or csv files.

![Download request purposes 1](img/download-request-purposes-1.png)

## BIMS: Download requests

Here you can see all download requests from users, including details of the requester, resource type (csv, table, chart), resource name and purpose (as specified in the download request purposes). One can find out further details of the request by clicking on the Request date link, which opens up a second form. This is useful to track the progress of the large request downloads.

![Download requests 1](img/download-requests-1.png)

![Download requests 2](img/download-requests-2.png)

## BIMS: Endemism

Here you manage the endemism categories including the Name (what is shown on the dashboard), description and display order.  The endemism categories are added during the uploading of the taxonomic master lists. Note that if the description is used in the master list, then this will be shown on the side panel and / or dashboard. It is important to always upload the Name only. Endemism categories can be merged in the event that erroneous uploading of categories occurs. 

![Endemism 1](img/endemism-1.png)

Each endemism category can be edited by clicking on the Name

![Endemism 2](img/endemism-2.png)

## BIMS: Harvest schedules

Here you manage the harvesting of GBIF occurrence records. 

1.	Go to Admin > Bims > Harvest schedule
2.	Click Add harvest schedule.
3.	Choose the module group.
4.	Set the period:

    •	Weekly: specify the day(s) of the week. You can use values like mon, tue or 0-6 (where 0 = Sunday).

    •	Monthly: specify the date (e.g., 15 for the 15th).

    •	Custom (cron): enter a cron expression. This option is mainly for developers, but it allows more flexibility (e.g., hourly, every 30 minutes).
5.	Add the run time. The task will be triggered at this hour (UTC timezone).
6.	Configure the defaults from the job section (these are for the harvest session settings).
7.	Set the boundary.
8.	Check Is fetching species if you want to harvest species.

Notes:

  •	We can only have 3 harvest sessions running at a time.

 •	If you want to harvest species, make sure the GBIF parent species is added to the module group, just like when a user harvests species.

## BIMS: Harvest sessions

Here you can view and manage the GBIF harvest sessions. The Start time, Status, Harvester, Module group are listed. To view details click on the Start time and a new form is opened up where you can see details such as if the harvest is fetching species or occurrences. 

![harvest-sessions-1](img/harvest-sessions1.png)

![harvest-sessions-2](img/harvest-sessions2.png)

## BIMS: Hydroperiods

Here you manage the hydroperiods, including display order. New hydroperiods can be added if required. 

![Hydroperiods](img/hydroperiods.png)

## BIMS: IUCN status

Here you can manage the Conservation status categories for global and national. Global is pulled down from the IUCN, while national is from SANBI. Status’s only applicable to national need to be opened and national checked. To change a status click on category.

![IUCN Conservation status 1](img/iucn-conservation-status-1.png)

![IUCN Conservation status 2](img/iucn-conservation-status-2.png)

The colour used can also be changed. For example, the colour template codes for the Global Conservation Status and <span style="color: red;">National Conservation Status (in South Africa as an example)</span> are: 

| Status | Colour code |
| -- | -- |
| Extinct | #C9CAC7|
| Extinct in the Wild | #A2A3A0 |
| <span style="color: red;">Regionally Extinct| #797A78</span> |
| <span style="color:red;">Critically Endangered – Possibly Extinct |#DD456A</span> |
| Critically Endangered | #641F30 |
| Endangered | #8D2641 |
| Vulnerable | #525351 |
| Near Threatened | #3D647D |
| Near Threatened – Legacy | #4D7E9D |
| <span style="color:red;">Critically Rare | #005904</span> |
| <span style="color:red;">Rare | #009106</span> |
| <span style="color:red;">Declining | #91900D</span> |
| Data Deficient | #D7CD47 |
| <span style="color:red;">Data Deficient – Insufficient Information | #D7CD47</span> |
| <span style="color:red;">Data Deficient – Taxonomically Problematic |#D7CD47</span> |
| Least Concern | #17766B |
| Least Concern – Legacy | #14655C |
| Conservation Dependent | #0F4D46 |
| Not evaluated | #39B2A3 |

## BIMS: Invasions

Here you can manage the Invasion categories. New categories are added using the "Add invasion" button. The name and description can be updated by clicking on the ID.

![invasions-1](img/invasions1.png)

## BIMS: Layer groups

Here you can manage layer groups that are visualised on the map under the layer selector. Layers can be grouped according to common features. For example, users can create a Catchment group that contains the primary, secondary, tertiary and quaternary catchments layers. 

To add a new group, click Administration and then select Publish Spatial Layer on Map. Click '+ Add layer group'. A layer group form will appear. Populate the fields and click Add. 

![Add layer group](<img/Layer group-1.png>)

All layers that will be assigned to a group must already be published to the map (see [Publish Spatial Layer on Map](https://kartoza.github.io/bims-website/administrator/layer-upload/publish-spatial-layer/)). To assign layers to a group, go to the admin page and select Layer groups. Click the new created group and assign layers to it by selecting the layers under 'Available layers' and pressing the right arrow, click Save. From this page, users can also edit existing groups add group descriptions. 

![Add layer group items](<img/Layer group-2.png>)

If you need to adjust the order of the layers, it can be adjusted by dragging the layers to the desired order under Publish Spatial Layer on Map on the main site.

Layers should now be visible under the group on the map on the main BIMS platform. The group can be opened and closed by clicking the arrow.

![Layer draw](<img/Layer group-3.png>)


## BIMS: Location context filter group orders

This can also be managed in the Layer upload, Styling and Spatial filter> Add Spatial filter section of BIMS.

Here you can manage the spatial layers shown in the side panel and dashboards, as well as the display and filter orders. The side panel dashboard is visible on the right hand side of the map. The detailed dashboard is visible once the user has clicked on the dashboard for a specific biodiversity module.  

![Side panel dashboard](img/side-panel-dashboard.png)

![Detailed dashboard](img/detailed-dashboard.png)

**Overview dashboard**    

![Location context filter group orders 1](img/location-context-filter-group-orders-1.png)

Clicking on the ID opens up this form, where one can select the Group and Filter, and change the group display order. One can also add new groups and / or filters. 

By clicking the box “ Show in dashboard” and /or “Show in side panel” the filters and groups are included or excluded in the different dashboards. 

![Location context filter group orders 2](img/location-context-filter-group-orders-2.png)

If you do not want the Group visible as a spatial filter, click the "Is hidden in spatial filter" box. 

If the filter is visible, and includes a long list, then it may be easier to click "Use autocomplete in filter", which allows the user to select one or more from a dropdown list. 

![Autocomplete filter](img/autocomplete-filter.png)

## BIMS: Location context filter

Here you can change the name and display order of the spatial filters.

![Location context filter order 1](img/location-context-filter-order-1.png)

## BIMS: Location context groups

Here you can manage the spatial layers and groups, which relate to geocontext. Each layer can be opened to view detail. To change what is displayed click the ID Number and check or uncheck the box for each. Note that there are some extra aspects that still need clarifying related to order etc.

![Location context groups 1](img/location-context-groups-1.png)

## BIMS: Location sites

Here you can view sites, filter for specific site and update site codes.

![Location sites 1](img/location-sites-1.png)

Here we are also able to update the geocontext data for each site or selection of sites.

![Location sites 2](img/location-sites-2.png)

## BIMS: Non-biodiversity layers

Here you manage the order that spatial layers are shown - it is more easily managed in the Layer upload, Styling and Spatial filter > Add Spatial filter section of BIMS. 

![Non-biodiversity layers 1](img/non-biodiversity-layers-1.png)

![Non-biodiversity layers 2](img/non-biodiversity-layers-2.png)

## BIMS: Notifications

Here you can assign specific administrator(s) to receive the different notifications that are generated when, for example, a new user signs up, or a new taxon is added.  This is changed by clicking on the Name of the notification and revising the list of Chosen users.

When a system is first set up the administrator has to add the notifications as well as the individuals who should receive each notification.

![Notifications](img/notifications-1.png)

![Change notifications](img/notifications-2.png)

## BIMS: Record types

Here you manage the record types used for collection of biodiversity occurrence data. New record types can be added and sort order changed. 

![Record types](img/record-types.png)

## BIMS: Roles

Here you manage the roles for users who sign up to the platform. New roles can be added and sort order changed. 

![Roles](img/roles.png)

## BIMS: Sampling effort measure

Here you manage the sampling effort measures used for collection of biodiversity occurrence data. These sampling effort measures are initially populated by the biodiversity data upload files, where each sampling method is specified in the dropdowns.  New measures can be added, existing ones edited, and a measure can be linked to a specific module if required.

![Sampling effort measure](img/sampling-effort-measure.png)

## BIMS: Sampling methods

Here you manage the sampling methods used for collection of biodiversity occurrence data. These sampling methods are initially populated by the biodiversity data upload files, where each sampling method is specified in the dropdowns.  Details are provided below.

For each sampling method the administrator needs to select the taxon group or groups that the method is associated with and certain sampling methods may be associated with one or more taxon groups / modules. As more biodiversity modules are added, it may be necessary for the administrator to update the sampling methods.

| Module | Sampling method |
| -- | -- |
| Invertebrates only | Baited Line |
| Invertebrates only | Box/Surber |
| Invertebrates only | Drift Net |
| Invertebrates only | Kick Net |
| Invertebrates only | Light Trap |
| Invertebrates only | Stone |
| Invertebrates, fish | Hand Net |
| Fish only | Fyke net |
| Fish only | Gill net |
| Fish only | Rod and line angling |
| Fish only | Seine net |
| Fish only | Snorkelling |
| Fish, anurans | Underwater video analysis |
| Fish, anurans | Electro-fishing |
| Fish, anurans | Visual survey |
| Anurans | Active acoustic survey |
| Anurans | Passive acoustic survey |
| Anurans | Baited trapping |
| Anurans | Non-baited survey |
| All | Unspecified |
| All | Multiple |

![Sampling methods 1](img/sampling-methods-1.png)

Changes can be made to each sampling method by clicking on the **Sampling method** and editing the name, order and Taxon group it is appropriate to.  To select more than one taxon group click Control Select simultaneously. If these have not been included in the data occurrence upload files, then they are blank. New sampling methods can be added by clicking the “+ Add sampling method”.

We have also added functionality to merge sampling methods, in the event that the same sampling method is added, but with a slight variation. For example:

![Sampling methods 2](img/sampling-methods-2.png)

To merge these two or more sampling methods, first you need to verify the correct one, by opening the method and ticking the verify box.

![Sampling methods 3](img/sampling-methods-3.png)

Then you use the select “Merge sampling methods” and click `Go`.

![Sampling methods 4](img/sampling-methods-4.png)

## BIMS: Site settings

Here you manage several components related to the setting of the site (i.e. webpage, url for the information systems, e.g. FBIS, RBIS, ORBIS etc.). Details of the sections that an administrator can change are provided below. It is divided into sections (those in red are not managed by admin).

- General
- <span style="color: red;">Landing & Docs
- Map
- Boundary and Park Layers
- Upload & Templates
- <span style="color: red;">GitHub App
- <span style="color: red;">External Integration & Tokens
- <span style="color: red;">Pesticide Dashboard
- GBIF

**General:** Here you can add and edit the Site notice. 

![site-settings-1](img/site-settings-general-1.png)

You can view and/or edit the copyright text that is visible at the bottom of the landing page. 

![site-settings-2](img/site-settings-general-2.png)

**Map:** You can change the default basemap, enable or disable the third part layer as not all information systems have links to third party data. 

![Site settings 6](img/site-settings-6.png)

![Site settings 7](img/site-settings-7.png)

**Boundary & Park Layers:** If occurrence data are uploaded for an area/Park or Section that does not have latitude and longitude, then it is possible to upload a csv of the Park Names with latitude and longitudes generated. These are then used to upload occurrence data for a Park or Section. 

![Uploading centroids](img/uploading-centroids.png)

**Upload & Templates:** Here you can: 
- You can specify the `readme` file that is bundled with the downloaded occurrence data.
- You can specify the taxonomic upload template for the Master lists. This is then downloadable on the Upload – Taxonomic data.
- You can specify the generic occurrence upload template for the occurrence data. This is then downloadable on the Upload – Occurrence data. If different biodiversity groups have customised master and occurrence upload templates then these are added in Taxon Management. ([See notes on Taxon Management](taxa-management.md))
- Turn on / off Auto validation of taxa (taxa uploaded using Taxonomic upload are automatically validated if this is clicked).

![uploads-and-templates](img/uploads-and-templates.png)

**Features / Toggles:** Here you can: 

![features-and-toggles](img/features-toggles.png)

- Enable or disable SASS as not all information systems have SASS data.
- Enable or disable water temperature data as not all information systems have water temperature data. 
- Enable or disable ecosystem type. 
- Enable or disable download request approval. If this is disabled then the user can download the data without waiting for approval from the administrator.
- Enable or disable the module summary on the landing page dashboard. This is not applicable to FBIS and other BIMS platforms.

![Site settings 12](img/site-settings-12.png)

- Enable or disable the 'Remove All' occurrence tool in Taxon Management. This should never be activated on the live/production site as clicking the 'Remove All' button, will delete all the occurrence data for the module. It can be enabled on the testing site as this allows administrators to practice the creation of new modules, uploading of taxonomic master lists and the uploading of occurrence data.

![Site settings 14](img/site-settings-14.png)

- Enable or disable allow edit in admin (in Taxon management).

![edit-taxon](img/edit-taxon.png)


**GBIF:** Here you can specify the GBIF username and GBIF password needed for harvesting taxa and occurrences from GBIF. The admin of each platform need to register on GBIF and then insert the details here for harvesting. 

You can view and/or edit the disclaimer form text and disclaimer doc text.

![disclaimer](img/disclaimer.png)

## BIMS: Source references

Generally it is easiest to manage source references (i.e. the metadata associated with each occurrence record).

![Source references 1](img/source-references-1.png)

However, on occasions, issues arise whereby the source reference is duplicated, possibly because of a small typo during data capture.  In the Admin - Source references – section it is possible to merge two source references. One does this by finding the two relevant source reference, opening the correct one and selecting “Verify”, then checking the box next to the two (or more) references to be merged, and using the Merge from the dropdown lists, then `Go`. Note that the Source reference needs to be the same type to be able to merge. If the Mobile box is checked, then this source reference will be available on the mobile App. 

![Source references 2](img/source-references-2.png)

![Source references 3](img/source-references-3.png)

## BIMS: Tag groups:

A tag group controls how the TAGS, which are uploaded for each taxon when the master list is uploaded, is visualised, specifically its colour. Click on the ID and change the colour. Tags are visible in Taxon Management as as a filter on the map interface. 

![tag-groups-1](img/tag-groups1.png)

![tag-groups-2](img/tag-groups2.png)


![tag-groups-3](img/tag-groups3.png)

![tag-groups-4](img/tag-groups4.png)


## BIMS: Taxa

Here you manage all aspects related taxa within the information system. Most of this is done easily within Taxon Management, but there are some actions that can only be done within this table, including delete a taxon (this cannot be done if occurrence data are associated with it), merge taxa, update taxa, fetch common names, fetch cites listing, extract author and harvest synonyms for accepted taxa (GBIF).

![taxa-1](img/taxa-1.1.png)

The table includes the Canonical Name (also referred to as the "true name”), Link to GBIF, Scientific Name, Author, Taxonomic Rank, Parent, the Import date, Taxonomic Status, Accepted taxonomy, Global Red List Status (IUCN), and whether the taxon has been Verified, and the Tag list.  A filter allow admin to select taxa for various criteria including Taxon Group.

![Taxa 1](img/taxa-1.png)

A search field and filters are also included to assist you to navigate.

![Taxa 3](img/taxa-3.png)


Clicking on the canonical name opens up the Change Taxonomy form for the selected species. Note that this is same as that accessed within Taxon Management.

![Taxa 2](img/taxa-2.png)

To delete a taxon, click the check box, and select Delete selected taxon, and click `Go`.

![Taxa 5](img/taxa-4.png)

There is a check, and if you click, "Yes, I am sure", then the taxon will be deleted.

![Taxa 6](img/taxa-5.png)

Sometimes errors are picked up in the taxa, for example there are two taxa that are the same. One then needs to merge these taxa. Prior to merging, the correct taxon needs to be checked and the verified button checked. Then to merge the two taxa, click the check box, and select Merge taxa, and click `Go`.

![Taxa 7](img/taxa-6.png)

Updating is used when one wants to update a synonym with the accepted name. Prior to updating, the accepted taxon needs to be checked and the verified button checked. Then to update the synonym, click the check box of both taxa, and select Update taxa, and click `GO`. This functionality is currently being refined.

## BIMS: Taxon groups

Here you manage the taxon groups added to the information systems. 

![Taxon groups 1](img/taxon-groups-1.png)

To note is the need to add the singular name so that it is correct in the Add XXXX data form.

![Taxon groups 2](img/taxon-groups-2.png)

![Taxon groups 3](img/taxon-groups-3.png)

You can also manage the wheel chart type that is viewed on the landing page. Options include: Global Conservation Status, Endemism, Division (Algae only), SASS Ecological Category (Invertebrates only). 

![Biodiversity Wheel Chart](img/biodiversity-wheel-chart.png)

## BIMS: Wetland indicator status

Here you manage wetland indicator status used for collection of biodiversity occurrence data. A new status type can be added and sort order changed. 

![Wetland Indicator Status](img/wetland-indicator-status.png)

## Flat pages

This is access outside of the BIMS section, in Flat Pages. From here you can update the “About us”, Citation guidelines and Help page.

![Flat Pages 1](img/flat-pages-1.png)

### Flat pages: About us

Text for the About Us on the menu bar can be modified here by nativigating to the Admin Page > Flat Pages > About.

### Flat pages: citation guidelines

![Flat Pages 2](img/flat-pages-2.png)

Text for the Citation on the landing page can be modified from Admin > Flat pages > Citation

### Flat pages: Help

Text for the Help on the menu bar can be modified from Admin > Flat pages > Help

Links to manuals can be added. For example, for FBIS: 

* Open this page https://freshwaterbiodiversity.org/admin/flatpages/flatpage/2/change/
* Double click the user manual
        ![Flat Pages 3](img/flat-pages-3.png)
* Open the Link tab, and change the url
        ![Flat Pages 4](img/flat-pages-4.png)
* Click `Ok`, and then click `Save`

Get the url for the FBIS Manual by opening Source References and right clicking the green title, and choose 'Copy link address'. Then insert this url into the URL in the Link tab and `Save`.

## People

### People: Users

![People 1](img/people-1.png)

### FBIS user sign up procedure

New users will click on the sign up button and enter details including email, First Name, Surname, Organisation, Role, Password. 

![User sign up 1](img/user-sign-up-1.png)

![User sign up 2](img/user-sign-up-2.png)

A link will then be sent to the administrators for approval.

![User sign up 3](img/user-sign-up-3.png)

The administrator will click on the activation link for their email. 

![User sign up 4](img/user-sign-up-4.png)

The activation link will take you to the following page where you will activate the user. Change the username to start with capital letters and check the Active checkbox and click Save. 

![User sign up 5](img/user-sign-up-5.png)

![User sign up 6](img/user-sign-up-6.png)

The user has now been added successfully. 

### Managing users

Details of all users are visible here and can be edited as needed. When a user first registers they are activated by clicking the Permission - Active box. 

Several filters have been included to manage and find users. 

![Managing users](img/managing-users.png)

#### Restricting access of certain data to specific users

Administrators can control which users are able to view different data types by including a column called Data Type in the occurrence upload template. The user roles are then managed in the People – Users table.

**Public or empty data type:** All users will be able to see the data.

**PrivateDataGroup:** All the staff of the tenant site will be able to see the data. For example, SANParks staff will be able to see Sanparks occurrence data with the data type set to private.

**SensitiveDataGroup:** Only users able to see sensitive data will be able to see the data.

![Restricting data](img/restricting-data.png)