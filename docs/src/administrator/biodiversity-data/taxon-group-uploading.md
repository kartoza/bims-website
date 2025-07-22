---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Helen Dallas
    - Jeremy Shelton
    - Jeremy Prior
    - Nazley Liddle
date: 21-07-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Creating a new Taxon Group (Biodiversity Module), creating a Master List from GBIF and uploading a Master List of Taxa

> Only registered users with **super user status** are able to do this, typically the administrators.

Suggested workflow is to: 
* Create a new Biodiversity Module / Taxon Group.
* Upload Taxonomic data if a Master List exists.
* Harvest GBIF taxa (species) for the group, if no Master List exists.
* Download and edit Master list if needed.
* Harvest GBIF occurrence records for the group.

## Steps

Click on your name and select Taxon Management
![Taxon management](<img/taxon group-3-taxon management.png>)

Click + and Add a New Module, Add Name (Label) and Logo by browsing to a suitable logo already created. A useful website for logos is found here: https://www.phylopic.org.  Click Save.

<img src="img/master list-2-edit module.png" alt="Add a module" width="200"><img src="img/taxon group-3-module popup.png" alt = "Add a module2" width = "300">

**Add a Taxon** that you will be using as a parent. E.g. Tracheophyta as the parent Phylum for Plants. 
![Add a taxon](<img/taxon group-3-add a taxon.png>)
![Add a taxon2](<img/taxon group-3-add a new taxon2.png>)

Approve/validate the Taxon. Clear the filters to see the new taxon added
![Validate Taxon](<img/taxon group-3-approve taxon.png>)

Click "edit" on the taxon group, by clicking the pencil icon in the taxon group list. A popup will be displayed. In the bottom field, you can see the GBIF taxonomy; choose the new taxon here. (Type the first few letters to get options). Click Save.

![Edit module](<img/taxon group-3-edit module.png>)
![GBIF Taxonomy](<img/taxon group-3-gbif taxonomy.png>)

Additional functionality allows you to: 

* Assign an expert - relevant for FADA only
* Select a parent taxonomy
* Add a customised Master List/Taxon upload template, and/or occurrence upload template. The default is the standard template. If extra attributes are added then the customised template can be uploaded. 

![GBIF Taxonomy2](<img/taxon group-3-gbif taxonomy2.png>)

To harvest GBIF species/taxa go to Harvest Species. Now, when you harvest taxa, it will check all the taxa related to the GBIF Taxonomy that was added to the Taxon Group. 

![Harvest Species](<img/taxon group-3-harvest species.png>)

Select the Boundary and Taxon Group and click **Start Harvesting**

![Harvest Species2](<img/taxon group-3-harvest species2.png>)

**Note that only one GBIF harvest can happen at a time per user, either for species or occurrences.**

Further management and editing of the Master list is done in Taxon Management.  It is also recommended that once an initial master list is created using harvest species from GBIF, that it is downloaded as a csv, edited with additional data such as Origin and Endemism, and reuploaded with extra attributes added as needed. See section below.

![Download Masterlist csv](<img/taxon group-3-download csv.png>)

If a Master list is created without using GBIF, or an edited Master list needs to be uploaded, then it can be uploaded as follows:

Click on your name and select **Upload Taxonomic Data**

![Taxon Group Upload 1](./img/taxon-group-upload-1.png)

Select the new Taxon Group using the dropdown and browse to the file containing the Master List of Taxa for the Taxon Group, click Upload.

![Taxon Group Upload 4](./img/taxon-group-upload-4.png)

Progress is shown:

![Taxon Group Upload 6](./img/taxon-group-upload-6.png)

A **Success** File will indicate taxa uploaded to the system. An **Error** file will give details of taxa not uploaded. The last column in this csv file provides an indication of the reason the taxon was not uploaded. The administrator then needs to check the data and correct before uploading again.

![Taxon Group Upload 7](./img/taxon-group-upload-8.png)

Once the Master List of Taxa has been added it can be viewed in the Taxon Management section.

An **Error File** provides details of the problem in the last column of the csv. Once these have been corrected, the file can be uploaded again.

![Taxon Group Upload 8](./img/taxon-group-upload-9.png)

New taxa may be added individually using the **Taxon Management**, or if there are multiple new taxa to be added, then the steps can be repeated, to upload the additional new taxa for the Taxon Group.