---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Helen Dallas
    - Jeremy Shelton
    - Jeremy Prior
    - Nazley Liddle
date: 21-11-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---
# Taxon Management

A dedicated Taxon Management module has been developed to allow users to view and administrators to manage taxa within their BIMS platform.  The taxa shown in Taxon Management are those taxa that have been uploaded via the “Upload Taxonomic Data” or harvested from GBIF. 

The taxa included in a platform are those consolidated from variable sources such as GBIF, IUCN, FishBase, checklists, and often depends on what taxonomic information is available for the geographic region and taxonomic group and are continually updated as information becomes available. 

Over time it is hoped that the freshwater taxa will be homogenised through the Freshwater Animal Diversity Assessment (FADA) project currently underway. 

All registered users with are able to view Taxon Administration, but only administrators are able to edit data in Taxon Management. Access Taxon Management via the Menu Bar>Name>Taxon Management.

![taxa-management-0](img/taxa-management-0.png)


**In Taxon Management users can do the following:**

- [Search for a taxon](#search-for-a-taxon)
- [Filter taxa](#filter-taxa)
- [Sort taxa](#sort-taxa)
- [View the GBIF and IUCN pages](#view-the-gbif-and-iucn-pages)
- [View a Taxon's details](#view-a-taxons-details)
- [View occurrence records per taxon](#view-occurrence-records-per-taxon)

### Search for a taxon

![taxa-management-4](img/taxa-management-4.png)

### Filter taxa

![taxa-management-7](img/taxa-management-7.png)

### Sort taxa
Taxa can be sorted using up ![taxa-management-6.01](img/taxa-management-6.01.png) arrow, by each of the headers given below.

![taxa-management-6](img/taxa-management-6.png)

### View the GBIF and IUCN pages
Clicking the GBIF and IUCN buttons will take you to the taxon pages on each respective website.

![taxa-management-10](img/taxa-management-10.png)

![taxa-management-11](img/taxa-management-11.png)

### View a Taxon's details
Expand a taxon by clicking the ![taxon-expand](img/taxon-expand2.png) next tp the taxon name to view Supra-generic Information, Infra Categories, Valid/Accepted Names, Conservation Status, and Common name. 

![taxon-details](img/taxon-details.png)

### View Tags
Tags are uploaded to provide information on taxonomic backbone, wetland dependency etc. These tags are generally platform specific and not all platforms have tags. 

![view-tags](img/view-tags.png)

Users can aso filter tags by going to the Map > clicking Search on the toolbar > Taxon Tags > selecting tag(s) > Apply

![taxon-tags-filter](img/taxon-tags-filter.png)

### View occurrence records per taxon 

Users can see how many occurrence records are associated with a taxon. When clicked, you are taken to the map where taxon records are displayed. 

![taxon-records-1](img/taxon-records-1.png)

In taxon management, only the total records for that specific taxon are shown. On the map, records are aggregated across accepted names and associated synonyms that are on the Master List. 

![taxon-records-2](img/taxon-records-2.png)

### Downloading taxa
All taxa in a group can be downloaded as a CSV file or checklist pdf.

![taxa-management-19](img/taxa-management-19.png)

Users can also apply filters to select a subset of the taxa in a taxon group. The download will then include those selected taxa.

**CSV**

![taxa-management-20](img/taxa-management-20.png)

**PDF**

![taxa-management-20.2](img/taxa-management-20.2.png)

## Administrator View

Administrators, in addition to the functionality all users have access to (listed above), are able to do the following:

- [Add or update a Taxon Group Name and logo](#add-or-update-a-taxon-group-name-and-logo---edit-module)
- [Edit a Taxon’s details](#edit-a-taxons-details)
- [Add a new Taxon](#adding-a-new-taxon)
- [Remove a taxon from the taxon group](#remove-a-taxon-from-the-taxon-group)
- [Add images of a taxon](#adding-images-of-a-taxon)
- [Add additional attributes specific to a taxon group](#adding-additional-attributes-specific-to-a-taxon-group)
- [Add and edit tags specific to a taxon group](#add-and-edit-tags-specific-to-a-taxon-group)

### Add or update a Taxon Group Name and logo - edit module

The name of the Taxon Group and logo can be updated easily by highlighting the group, and clicking “Edit” indicated by the pencil, then typing the new name in “Label”, and browsing to the correct logo.

![Taxa Management 2](./img/taxa-management-2.png)

### Edit a Taxon's details
Admin can edit a taxon’s details in “Edit” or “Edit in Admin” by clicking the three vertical dots ![kebab-menu](img/kebab-menu2.png) (kebab menu) at the far right of the taxon row. The first is primarily used by taxonomists, while the second is useful for adding origin and endemism. 

![Taxa Management 8](./img/taxa-management-8.png)

### Edit in Admin

 “Edit in Admin” opens up a pop up window that is the taxon in BIMS>Taxa. Here you can check and update additional details of a taxon.

Often Origin, Endemism and Invasion are uploaded when the master list is uploaded, but there are times when it is useful to edit these on the BIMS>Taxa form. The options for selection are managed in BIMS>Endemisms and BIMS>Invasions, while Origin is hard-coded.

![Taxa Management 9](./img/taxa-management-9.png)


### Adding a new Taxon

If a new taxon needs to be added to the group, click the “Add a Taxon” button, type in the species name, and click “Find”. 

![Taxa Management 13](./img/taxa-management-13.png)

 If the Taxon is on GBIF it will provide the link to the GBIF taxonomic backbone, then click “Add” to confirm the addition of the new taxon to the taxon group.

![Taxa Management 14](./img/taxa-management-14.png)

If the taxon is not on GBIF, the administrator may add the new taxon, after which they must assign it to the appropriate Family and indicate the taxonomic rank of the new taxon. Taxa at all taxonomic levels may be added, although it is generally genus and/or species that are added.

![Taxa Management 15](./img/taxa-management-15.png)

Then edit details of the taxon by following the [Edit in Admin](#edit-in-admin) process.

### Remove a taxon from the taxon group

This needs to be used with caution. If data are associated with the taxon, then you will not be able to delete the taxon.

![Taxa Management 16](./img/taxa-management-16.png)


### Adding images of a taxon

By default images of a taxon are harvested from GBIF is they exist. In some instances an administrator may want to add images of a taxon themselves. To do this:

* Open Taxon Management
* Select the Taxon Group
* Select the Taxon and click Edit in Admin
        ![Taxa Management 21](./img/taxa-management-21.png)
* Go to the bottom of the “**Change Taxonomy**” form and add an image by browsing to the file. This image will then replace any GBIF image. Several images may be added for a taxon if desired.

    ![Taxa Management 22](./img/taxa-management-22.png)
* Click “Save”.

### Adding additional attributes specific to a taxon group

It may be desirable to add attributes for specific taxon groups such as “Water dependence” (Highly dependent, Moderately dependent, Minimally dependent, Terrestrial). These additional attributes are assigned to each taxon during the uploading of the master lists as long as the additional attribute is added in Taxon Management before uploading.

This is done in the Edit Module form, Add attribute. The attribute needs to match the attribute column header in your Master List for uploading.

![Taxa Management 23](./img/taxa-management-23.png)

You can add taxon specific attributes to a taxon group by adding additional column to the Master list and uploading , or individually by adding to the “**Change Taxonomy**” form:

* Open Taxon Management
* Select the Taxon Group
* Select the Taxon and click Edit

### Add and edit tags specific to a taxon group

Tags are used to provide additional categories about taxa in a module. They are uploaded with the column header being the tag name, and taxa populated with "Y" or "N" in the Master list. 

![taxa-tags-3](img/tags-3.png)

Taxa with Y will receive that tag name in taxon management. 

![taxa-tags-1](img/tags-1.png)

They can be edited in Admin>Taggit>Tags

![taxa-tags-4](img/tags-4.png)

To edit the colour of a tag, you need to create a group and add colour in Admin>Bims>Tag Group

![taxa-tags-5](img/tags-5.png)
