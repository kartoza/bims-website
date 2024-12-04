---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Jeremy Prior
date: 26-09-2023
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# BIMS: Styling Uploaded Layers

>Note: Only admin/super users can style spatial layers:

There are two methods to access the styling `Editor` page.

* [Access Method 1](#access-method-1-from-the-layer-upload-page): From the `Layer Upload` Page.
* [Access Method 2](#access-method-2-from-the-administration-site): From the `Administration` Page.

## Access Method 1: From the Layer Upload Page

To reach the `Layer Upload` page read through the [BIMS: Upload Spatial Layers](./upload-spatial-layers.md) guide. When you get to the [Access the Editor](./upload-spatial-layers.md#access-the-editor) section, you can click the link to return here.

## Access Method 2: From the Administration Page

As an admin/super user, access the `Administration` page by clicking on 1️⃣ your user name in the top right corner of any page and then click on 2️⃣ `Admin Page` on the dropdown menu.
> Note: If your BIMS instance has been customised, you may be able to hover your mouse pointer over `Administration` drop down menu from the top navigation bar.

![Style Editor 1](./img/style-editor-1.png)

On the `Administration` page, scroll down to 1️⃣ the `Cloud Native Layers` section and then click on 2️⃣ `Layers`.

![Style Editor 2](./img/style-editor-2.png)

On the `Layers` page, click on 1️⃣ the `Editor` link next to your preferred layer to be redirected to the `Editor` page.

![Style Editor 3](./img/style-editor-3.png)

## The Maputnik Style Editor Page

When you first arrive on the Maputnik Style editor page, you are greeted by a world map with a default style for the layer.

![Style Editor 4](./img/style-editor-4.png)

If the layer has been previously styled, you can click on 1️⃣ the `Style` dropdown to select the style you would like to edit.

![Style Editor 5](./img/style-editor-5.png)

### Styling a Spatial Layer

#### Basic Colour Change

To start styling a layer, zoom in on the area of the map where your layer should (e.g. This layer was for South Africa, so the map was zoomed in on South Africa).

![Style Editor 6](./img/style-editor-6.png)

If you would like to just change the colour of the layer, click on 1️⃣ the default style layer and then click on 2️⃣ the `Color` textbox that has a colour hexcode in it.

![Style Editor 7](./img/style-editor-7.png)

This will open a modal where you can either use 1️⃣ the various sliders and 2️⃣ colour box to select a colour, or you can paste in the hexcode of the colour you would like in 3️⃣ the textbox (ensure there is a # before the six characters).

![Style Editor 8](./img/style-editor-8.png)

This will change the colour of the entire layer.

![Style Editor 9](./img/style-editor-9.png)

#### Colour Based on Attribute

If you would like to style the layer based on an attribute you need to add a filter to your style layer and will need to add a new layer per different colour.

If you know the attribute name and attribute value you would like to use as a filter, you can can adapt the initial layer's filter to suit your needs. In this example, the attribute name is `Province` and the attribute value is `Northern Cape`.

![Style Editor 10](./img/style-editor-10.png)

If you are unsure of your filter requirements, you can click on 1️⃣ the `View` dropdown menu and then select 2️⃣ the `Inspect` option.

![Style Editor 11](./img/style-editor-11.png)

This will swap you to the inspection view, where you can use your mouse to click on features and display 1️⃣ a `Popup` with information about the feature(s) under your mouse.

![Style Editor 12](./img/style-editor-12.png)

If features are not displaying in the `Inspection` view, click on 1️⃣ the `Delete` filter icon.

![Style Editor 13](./img/style-editor-13.png)
