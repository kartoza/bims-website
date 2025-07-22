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

# Preparing and checking an Occurrence Data File before uploading

## Extracting data and preparing bulk data for uploading

The online platform includes data capture forms for adding sites, biodiversity data for the biodiversity modules added to the platform (e.g. fish, invertebrate and algae data), as well as associated abiotic data. However, these forms are intended for the capture of individual site visits, and at times, especially during the development phase of an information system, it is useful to be able to upload large amounts of data at a time. To ensure that bulk data are readily uploaded into FBIS, a standardised **Data Upload Template** needs to be produced for each group. This will ensure that data are cleaned and provided in a standardised manner so that the data uploading process runs smoothly and so that the resultant platform serves quality data.

## Data Upload Templates

A standardised generic data upload template in excel has been generated to serve all data platforms. This templates include a number of dropdown attributes.  It is critical that all taxa in the Data Upload file for a particular biodiversity group are present in the Master List of Taxa for that group. If not, the upload process will not work. For this reason, it is recommended that where possible dropdown lists are used in the Data Upload files to ensure that all data entered in the sheet are valid. In addition, functionality has been added to allow for customisation of the occurrence upload template for each module, if desired. The generic data upload template is provided and described below. It is recommended that the data management team review this template and remove any columns that are not needed.

The following data upload template is provided:
* <span style="color: #70ad47;">Generic Data Upload Template.xlsx</span>

Many of the columns are the same for each group, although some additional columns are included for algae, and the dropdown options (e.g. biotopes) sometimes vary amongst groups. The common columns used in each group are given in Table 1. Relevant dropdown lists are provided in each template and additional group-specific columns are included in the relevant templates. <span style="color: red;">Those column headers in red have to be filled in the occurrence upload file.</span> These are provided first in the excel file. See section on **Check the Source Reference** for details of which columns are relevant for different reference categories. Those column headers <span style="background-color:#c1ebaa;">shaded green</span> use dropdown lists in the excel file. These can be modified in the Admin page (BIMS).

It is recommended that once a dataset has been prepared, it is first uploaded to the staging site (i.e. testing site), so that issues can be picked up before the dataset is then uploaded to the production site. The production site is the site that contains the live data.

**Table 1. Column headers with details used in data upload templates**

| Column Header | Details |
| -- | -- |
| <span style="color: red;">UUID</span> | <span style="color: red;">A unique identifier for each record. Drag and copy the formula down.</span> |
| <span style="color: red;">Latitude | <span style="color: red;">Decimal degrees with "-" in front & "," for decimal point |
| <span style="color: red;">Longitude | <span style="color: red;">Decimal degrees with "," for decimal point |
| <span style="color: red;">Sampling Date | <span style="color: red;">yyyy/mm/dd |
| <span style="color: red;">Taxon |  |
| <span style="color: red;background-color:#c1ebaa;">Taxon rank | <span style="color: red;background-color: #c1ebaa;">Select from dropdown options |
| <span style="color: red;">Present |<span style="color: red;"> Fill in with "1" |
| <span style="color: red;">Collector/Owner | <span style="color: red;">Full name |
| <span style="color: red;">Collector/Owner Institute | <span style="color: red;">Institute of collector/owner |
| <span style="color: red;">Author(s) | <span style="color: red;">Surname + Initials |
| <span style="color: red;">Year | <span style="color: red;">Year of study |
| <span style="color: red;">Source | <span style="color: red;">Source of data if from thesis or database |
| <span style="color: red;">Title | <span style="color: red;">Title of data source if thesis, published article or published report |
| <span style="color: red; background-color:#c1ebaa;">Reference category | <span style="color: red;background-color: #c1ebaa">Select from dropdown options |
| <span style="color: red;">URL | <span style="color: red;">Thesis handle, or article link if no DOI available |
| <span style="color: red;">DOI | <span style="color: red;">DOI for reference ( e.g. 10.2989/16085914.2018.1491385) |
| <span style="color: red;">Document Upload Link | <span style="color: red;">Link to "Documents" page after uploading PDF of published report |
| Ecosystem type | River, wetland or open waterbody |
| User River or Wetland Name | Name given in study reference |
| User Site Code | Site Code given in study reference |
| Site Code | Leave blank (autogenerated) |
| Site description | Description given in study reference |
| <span style="background-color:#c1ebaa;">User Geomorphological Zone|  <span style="background-color:#c1ebaa;">Specified by user or listed in study - Select from dropdown options |
|  <span style="background-color:#c1ebaa;">User Hydrogeomorphic Type |  <span style="background-color:#c1ebaa;">Specified by user or listed in study - Select from dropdown options | 
| <span style="background-color:#c1ebaa;">Sampling method | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Sampling effort measure | <span style="background-color:#c1ebaa;">Select from dropdown options |
| Sampling effort value |  |
| <span style="background-color:#c1ebaa;">Abundance measure | <span style="background-color:#c1ebaa;">Select from dropdown options |
| Abundance value | Leave blank if only presence data |
| <span style="background-color:#c1ebaa;">Record type | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Broad biotope | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Specific biotope | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Substratum | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Water Level | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Hydroperiod | <span style="background-color:#c1ebaa;">Select from dropdown options | 
| <span style="background-color:#c1ebaa;">Water Turbidity | <span style="background-color:#c1ebaa;">Select from dropdown options |
| <span style="background-color:#c1ebaa;">Embeddedness | <span style="background-color:#c1ebaa;">Select from dropdown options |
| Depth | Depth (m) |
| Near Bed Velocity | Near Bed Velocity (m/s) |
| COND | Conductivity (mS/cm) |
| PH | PH |
| DOPER | Dissolved Oxygen (%) |
| DO | Dissolved Oxygen (mg/L) |
| TEMP | Temperature (deg C) |
| TURB | Turbidity (NTU) |
| Notes | Any details related to sampling, species, life form etc. |


>**Note**: There are additional columns specific to algal data

It is recommended that separate data upload files be created for each Source Reference, with each linked to a GitHub ticket. This ensures accurate management of data preparation and management.

## Preparing and checking an Occurrence Data File

To ensure that data are accurate, several steps should be taken before uploading occurrence data.  After consolidating the occurrence data in the data file, you should check the following:

**Apply filters for checking the data by highlighting the header row**, clicking **Data, Filter**

![Occurrence Data Preparation 1](./img/occurence-data-preparation-1.png)

**UUID:** This is a unique id for each occurrence record. It needs to be copied and pasted so that the formula used to generate it is saved as a number.

**The UUID formula is available here:**
```
=LOWER(CONCATENATE(DEC2HEX(RANDBETWEEN(0,POWER(16,8)),8),"-",DEC2HEX(RANDBETWEEN(0,POWER(16,4)),4),"-","4",
DEC2HEX(RANDBETWEEN(0,POWER(16,3)),3),"-",DEC2HEX(RANDBETWEEN(8,11)),DEC2HEX(RANDBETWEEN(0,POWER(16,3)),3),
"-",DEC2HEX(RANDBETWEEN(0,POWER(16,8)),8),DEC2HEX(RANDBETWEEN(0,POWER(16,4)),4)))
```

Systematically check each column using the dropdown arrows, and look for inconsistencies. Some common issues include, #num in UUID column instead of the UUID, incorrect spelling in the **Site description** column (e.g. Gakiriro wetland, Gakirirowetland), latitude with missing “-“  (e.g. 2.60059 as latitude is incorrect – should be -2.60059), longitude.

**Latitude and Longitude**: Also check that all sites fall within the country boundary so that Site Codes may be generated correctly and geocontext data harvested for each site.

![Occurrence Data Preparation 2](./img/occurence-data-preparation-2.png)
![Occurrence Data Preparation 3](./img/occurence-data-preparation-3.png)

**Check that the sampling date** is in the correct format: yyyy/mm/dd. If the format is not correct then the upload will not work.

**Check that all taxa are correct and are present in the Master List.** If the dropdown of master taxa list was used then this should not be an issue.  

Check that the **Taxon rank** is correct. It is important that the correct Taxon Rank is always used to ensure correct uploading of the data files. Taxon Rank is case sensitive so 'Species' will upload but 'species' will fail. Always ensure the correct Taxon Rank is applied by using the dropdown list. There should be no spaces in SubClass, SubOrder, SubFamily, SubSpecies.

![Occurrence Data Preparation 4](./img/occurence-data-preparation-4.png)

**Check presence** is all “1”, check **sampling method** is correct.

![Occurrence Data Preparation 5](./img/occurence-data-preparation-5.png)
![Occurrence Data Preparation 6](./img/occurence-data-preparation-6.png)

**Check Collector/Owner and Collector/Owner Institute.** Ideally CAPITALS should not be used, First name Surname if known. Do not use middle initial and punctuation.

![Occurrence Data Preparation 7](./img/occurence-data-preparation-7.png)

**Check format of Author(s).** It needs to be: Surname + Initials, no punctuation.  (e.g. Tumushimire L, Mindje M,  Sinsch U & Dehling JM not Lambert Tumushimire, Mapendo MINDJE,  Prof. Ulrich Sinsch & Julian Maxmillian Dehling). It is important to get the authors correct (e.g. Sinsch Ulrich and Dehling, J. Maximilian, Lümkemann Katrin, Rosar Katharina, Christiane Schwarz should be Sinsch U, Lümkemann K, Rosar K, Schwarz C & Dehling M as per the doi).

![Occurrence Data Preparation 8](./img/occurence-data-preparation-8.png)

**Check the Date:** This is the publication date (so 2012-2013 should be 2019 as this is when the article was published - Ecology and Evolution. 2019. Same with all other data from this study).

![Occurrence Data Preparation 9](./img/occurence-data-preparation-9.png)

**Check the Source.** Please note when to include source or not, and what to include.  (e.g. Mindje, M., Tumushimire, L., & Sinsch, U. (2020). Diversity assessment of anurans in the Mugesera wetland (eastern Rwanda): impact of habitat disturbance and partial recovery. Salamandra, 56, 27-38. Should be **Salamandra**)

* For Peer-reviewed scientific articles - the Source is the Journal.
* For Published Reports and Theses - the Source is the publisher of the Report.
* For Unpublished Data - the source is the title of the study.

![Occurrence Data Preparation 10](./img/occurence-data-preparation-10.png)

**Check the Title.** For Peer-reviewed scientific article the Title is the title of the article, for Published reports or theses, it is the title of the thesis.  Unpublished data don’t need a title.

![Occurrence Data Preparation 11](./img/occurence-data-preparation-11.png)

**Check all Reference Categories** are correct: 

Options include:
* Database
* Peer-reviewed scientific article
* Published report
* Thesis
* Unpublished data

![Occurrence Data Preparation 12](./img/occurence-data-preparation-12.png)

**Check the Source Reference** (Author(s), Year, Source, Title, Reference category, URL, DOI, Document Upload Link). For each study reference type, you need to populate the following columns:

* Peer-reviewed scientific article (Collector/Owner; Collector/Owner Institute; Author(s); Year; Source; Title; DOI or URL (if DOI is not available)). For Peer-reviewed scientific article the Source is the Journal, For Peer-reviewed scientific article the Title is the title of the article.
* Published report (Collector/Owner; Collector/Owner Institute; Author(s); Year; Source; Title; URL or Document Upload Link). Note the Document Upload Link is obtained after the report is added.
* Thesis (Collector/Owner; Collector/Owner Institute; Author(s); Year; Source; Title; URL or Document Upload Link)
* Database (Collector/Owner; Collector/Owner Institute; Author(s); Year; Source)
* Unpublished data (Collector/Owner; Collector/Owner Institute; Author(s); Year; Source)

**Check URL and DOI.** Use a DOI if it is available, URL – only needed for Peer-reviewed scientific article if there is no DOI. For the DOI you only need to include the number part, so 10.1080/15627020.2012.11407524, not https://doi.org/10.1080/15627020.2012.11407524.  

![Occurrence Data Preparation 13](./img/occurence-data-preparation-13.png)
![Occurrence Data Preparation 14](./img/occurence-data-preparation-14.png)

**Check the document upload link is correct.** Note the Document Upload Link is obtained after the report is added. Reports are only uploaded when there is no DOI or URL to link the data to.

**Checking for duplicate occurrence records.** Use this formula for checking for duplicates. This is a combination of Site description, latitude, longitude, sampling date, Taxon, sampling method, author, year, source and title.  Copy and paste the formula below into a new column at the end and name it “Duplicate check”.

For a basic check where user site codes are not given and no biotopes are used, this formula can be used.

```
=CONCATENATE(B1,C1,D1,E1)
```
For data where User site code has been provides, and biotope/habitat level data is included, then a more complex concatenate formula is needed:

```
=CONCATENATE(B1,C1,D1,E1,T1,AE1,AF1,AG1)
```
This formula can be revised as needed so that potential duplicates may be picked up.

Then copy and paste the formula down to the end of the data rows. Then Highlight the column, and from the Home menu, select **Conditional Formatting, Highlight Cells Rules, Duplicate Values**.

![Occurrence Data Preparation 15](./img/occurence-data-preparation-15.png)

Any duplicates will be highlighted. Check and delete duplicate occurrence records. Then delete the Duplicate Check column.

**Delete blank rows and columns**. Lastly, ensure that there are no extra blank rows or columns, by deleting them.

![Occurrence Data Preparation 16](./img/occurence-data-preparation-16.png)

![Occurrence Data Preparation 17](./img/occurence-data-preparation-17.png)

Remove the data filter, save the file in excel, and save the file as csv file.

![Occurrence Data Preparation 18](./img/occurence-data-preparation-18.png)
