---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Helen Dallas
    - Jeremy Shelton
    - Jeremy Prior
    - Nazley Liddle
date: 24-07-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Validating a record (occurrence data) or taxon

This section explains the process when a user adds data to a platform, and how the administrator views, checks and validates the occurrence record or new taxon.

Data served on the platform includes both validated and unvalidated data, where validated implies some degree of checking that the record is accurate.  The user is able to select one or the other using the filter:

![Validate Records 1](./img/validate-records-1.png)

All data added to the platform by administrators using the Upload Occurrence data template, is given the status of validated on the assumption that the administrator has checked the data prior to uploading.

However, when a user adds data directly to the platform, this data remains unvalidated until the administrator checks the data.

## Validating new biodiversity occurrence records

When a user adds new occurrence data, the data is automatically assigned an unvalidated status. The administrator is sent an email alerting them to the new record.

![Validate Records 2](./img/validate-records-2.png)

This unvalidated record is also added to the Validate Records form, which the administrator has access to.

![Validate Records 3](./img/validate-records-3.png)

This form includes functionality to **See Unvalidated data**, and filter by Owner, Site Code, or Module. The administrator can then undertake the following actions, using these buttons

![Validate Records 5](./img/validate-records-5.png)

The administrator can then undertake the following actions, using these buttons. 

![Validate Records 4](./img/validate-records-4.png)

## In summary

**Viewing**: the data is viewed by the administrator and checked for accuracy in terms of all entries including the taxa recorded. If a taxon is outside of its expected geographical range, then the administrator would reject the data with a reason to the person who uploaded the data.

**Reject**: the data is rejected and the user receives an email notification with the reason. The user then has the opportunity to edit their data and resubmit for validation.

**Validate**: the data is validated by the administrator if everything is correct.

**Delete**: this is only used when data have been accidentally added to a site but is generally easier done via the data forms.

## Validating a new taxon

Generally a user should not need to add a new taxon often as the master lists for each biodiversity module are updated and represent the full expected checklist of species for a country. However, in the event that the user records a new taxon not currently in the master list, they are able to add this taxon to the information system. The administrator then receives a message alerting them to a new taxon that has been added. This new taxon then goes through a validation process by the administrator, and the new taxon is either accepted or rejected (with reasons).

![Validate Records 6](./img/validate-records-6.png)

Once the Administrator receives the email, they follow the link to Taxon Management:

![Validate Records 7](./img/validate-records-7.png)

The Admin checks the taxon, and if it is acceptable to add to the Master List, then click Validate. Note the administrators may need to seek expert taxonomic input. The user receives an email indicating that the data has been approved.

If it is not acceptable, then Reject the taxon. An email will be sent to the user who uploaded the records, with reasons for the rejection.

**Note**: A new occurrence record (site visit) cannot be validated if the new taxon has not been validated. On Validate records it is shown as an **Unvalidated taxon**. First the administrator must validate the taxon by following the link in the email, or by clicking on the **Validate Taxon** button below. The taxon is then either validated or rejected. Once the new taxon has been validated, then the record can be validated.  
Before the taxon is validated:

![Validate Records 8](./img/validate-records-8.png)

After the taxon is validated:

![Validate Records 9](./img/validate-records-9.png)
