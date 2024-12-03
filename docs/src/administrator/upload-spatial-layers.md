---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Jeremy Prior
date: 26-09-2023
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# BIMS: Upload Spatial Layers

>Note: Only admin/super user can upload spatial layers.

Click on [here](https://bims.site.com/upload-spatial-layer/) to access the upload spatial layers page.

This is how it looks.

![Upload Layers UI](./img/upload-spacial-layer-1.png)

* **Name:** Enter the name of the layer.

* **Choose files:** Select the shape file to upload.

* **Submit:** Uploads the shape file.

* **❎:** Close the form.


## Upload Layers

Click on the `Choose files` button to select the shape file to upload.

![Upload Layers UI](./img/upload-spacial-layer-4.png)

This will open the file explorer from where user can select the shape files.

> Note: User can select multiple files at the same to upload.

![File Explorer](./img/upload-spacial-layer-2.png)

* **Cancel:** Cancel the process.

* **Open:** After selecting the files, click on the `Open` button to upload the file.

* **✅ Open files read only:** Open the files in read only mode.

* **None:** File extension.

This process will take some time to complete.

## 413 Request Entity Too Large

This error appears when the uploaded file exceeds the maximum size limit.

![Error](./img/upload-spacial-layer-3.png)

## Current Process:

### Status: Start

Indicates that the process has started.

![Start Status](./img/upload-spacial-layer-7.png)


### Status: Running

Indicates that the process is in progress and may take some time to complete.

![Running Status](./img/upload-spacial-layer-5.png)

### Status: Success

Indicates that the files have been uploaded successfully.

![Success Status](./img/upload-spacial-layer-8.png)

* User will receives a success message.

    ![Success Status Message](./img/upload-spacial-layer-10.png)

### Status: Failed

Indicates that the files failed to upload.

## Access Editor

After successfully completing the process, the user will gain access to the editor page.

Click on the `Editor` button to access the editor page

![Editor Button](./img/upload-spacial-layer-9.png)

This is the UI of the `Editor` page.

![Editor UI](./img/upload-spacial-layer-11.png)

## Admin page 

* To access the admin page, hover on the `Administration` drop down menu from the top navigation bar.

    ![Administration tab](./img/upload-spacial-layer-12.png)

* Choose the `Admin Page` option from the drop down menu. This will open the admin page.

    ![Drop Down Menu](./img/upload-spacial-layer-13.png)

### Access the Uploaded Layers

* Navigate to the `Cloud Native Layer` section from the left menu.

    ![Cloud Native Layers Section](./img/upload-spacial-layer-15.png)

    Click on the `Cloud Native Layer` heading to navigate to this section on a new page. 

    ![Cloud Native Layers Section](./img/upload-spacial-layer-16.png)

    1. **Layer uploads:** By clicking on this user will be able to see all the uploaded layers.

        ![Layer Uploads](./img/upload-spacial-layer-17.png)

        **1. total:** Displays the total number of layers uploaded.

        **2. Data:** This is the list of uploaded layers with the corresponding details.

        **3. Add layer upload:** This button is used to upload a new layer.

        **4. Filter:** By using this user can filter the data. After clicking on this a dropdown menu will appear.

        ![Filter](./img/upload-spacial-layer-18.png)

        * **Layer:** This is used to filter the layers by name.

        * **Status:** This filter allows users to arrange the layers by their current status such as success, failed, etc.

            ![Filter By Status](./img/upload-spacial-layer-19.png)

        **5. Dropdown menu:** This menu allows users to perform some actions on the data. This are the available options.

        ![Dropdown Menu](./img/upload-spacial-layer-20.png)

        * **Import data:** This option allows users to import the data.

        * **Delete selected layer uploads:** This option is used to delete the selected layers. Users can delete multiple layers at once.

        **6. Go:** This button allows users to proceed with the actions they have selected from the dropdown menu.

    2. **Layers:** By clicking on this users will be able to see the list of the layers they have uploaded including their details.

        ![Layers](./img/upload-spacial-layer-21.png)

        **1. total:** Total number of layers.

        **2. Data:** This is the list of layers with their details such as id, status and created_by etc.

        **3. Add layer:** This button allows users to upload a new layer from the admin panel.

        **4. Dropdown menu:** This menu allows users to perform some actions on the data. This are the available options.

        ![Dropdown Menu](./img/upload-spacial-layer-22.png)

        * **Delete selected layers:** This option is used to delete the selected layers. Users can delete multiple layers at once.

        * **Go:** This button allows users to proceed with the actions they have selected from the dropdown menu.
