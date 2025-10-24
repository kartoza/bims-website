---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Tim Sutton
    - Dimas Ciputra
    - Jeremy Prior
    - Nazley Liddle
date: 17-10-2025
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact: 
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# Landing page customisation

This guide contains details on how to add landing page sections, section contents and information on how to add videos or images.

Navigate to BIMS Theme in Admin
![BIMS Theme](<img/Screenshot 2025-10-17 092323.png>)

## Adding a Landing Page Section

This guide will help you in adding a new section to your landing page.

![section 1](img/Screenshot%202023-07-16%20at%201.53.56%20PM.png)

- Ensure that there is at least one custom theme enabled. To check this, proceed to 'Custom Theme' and see if a record is present and enabled. If not, you can create a new one.

![section 3](img/Screenshot%202023-07-16%20at%201.57.12%20PM.png)

- Let's create a new landing page section. Navigate to 'Landing page sections', and click 'Add new section'.

![section 4](img/Screenshot%202023-07-16%20at%201.58.58%20PM.png)

- (1) Name the new section (note that this name will not appear on the landing page).

    (2) Optionally, add a title that will be displayed on the landing page.

    (3) Set the background color for the section.

![section 4](img/Screenshot%202023-07-16%20at%202.02.17%20PM.png)

- Click 'Save and continue editing'. This will allow you to add content to the section afterwards.

- If you have previously created landing page section content, you can select it in the content field. If not, you can add a new one by clicking the plus button.

- Once you have finished editing the new content, click 'Save'. Remember, you can always update this later.

![section 4](img/Screenshot%202023-07-16%20at%202.06.04%20PM.png)

- Be sure to select at least one content here.

![section 5](img/Screenshot%202023-07-16%20at%202.07.28%20PM.png)

- Click 'Save'. The next step is to add this section to your theme. Navigate to 'Custom Themes' (see [Custom Themes](./custom-themes.md) for more details) and select the enabled theme.

- Scroll to 'Landing page sections' and select your new section. If you want to select more than one section, hold down the Control key (or Command on a Mac).

![section 6](img/Screenshot%202023-07-16%20at%202.10.38%20PM.png)

- Finally, click 'Save'. Your new landing page section should now be visible.

![section 7](img/Screenshot%202023-07-16%20at%202.12.27%20PM.png)

## Embedding Youtube Video on the Landing Page

- First, select the YouTube video you wish to show on the landing page
- Click the 'Share' button under the video

![Youtube share](img/Screenshot%202023-07-16%20at%2011.31.11%20AM.png)

- In the popup, click the 'Embed' button

![Youtube embed](img/Screenshot%202023-07-16%20at%2011.32.38%20AM.png)

   Click the 'Copy' button on the bottom right. This action copies the video's embed code to your clipboard

![Youtube popup](img/Screenshot%202023-07-16%20at%2011.34.25%20AM.png)

- Now, navigate to the admin page and open the landing page section editor

![Admin page](img/Screenshot%202023-07-16%20at%2011.36.20%20AM.png)

- Click on 'Source'

![Admin page-2](img/Screenshot%202023-07-16%20at%2011.55.00%20AM.png)

- Paste the copied embed code into the 'Source' editor using Ctrl+V (or Cmd+V for Mac)

![Admin page-3](img/Screenshot%202023-07-16%20at%2011.56.54%20AM.png)

- Click 'Source' again. You should now see an iframe containing the video player

![Admin page-4](img/Screenshot%202023-07-16%20at%2011.58.13%20AM.png)

- Once the landing page content is added to the current theme, your video will appear on your landing page like this

![Admin page-5](img/Screenshot%202023-07-16%20at%2012.09.46%20PM.png)

- To adjust the video size, double-click the iframe. A popup will appear where you can edit the width and height of the video player. Click 'OK' when done, and then 'Save'

![Admin page-6](img/Screenshot%202023-07-16%20at%2012.12.59%20PM.png)

## Adding Inline Images on the Landing Page

This section will help you display images inline, just like the one below:

![Inline image](img/Screenshot%202023-07-16%20at%2012.35.47%20PM.png)

- Start by navigating to the section editor on the landing page. Once there, create a new section.

- To facilitate the upcoming steps, switch the editor to full-screen mode. Click on 'maximize' to do this.

![Inline image2](img/Screenshot%202023-07-16%20at%2012.40.09%20PM.png)

- Next, click on the 'Table' button.

![Inline image2](img/Screenshot%202023-07-16%20at%2012.41.13%20PM.png)

- For this example, we want to showcase three inline images, each with its title underneath. To do this, create a table with 3 columns and 2 rows. Ensure the border width is set to 0.

![Inline image2](img/Screenshot%202023-07-16%20at%201.25.14%20PM.png)

- Start with the titles so you can easily add images later. Click on the 2nd row and input the corresponding text.

![Inline image3](img/Screenshot%202023-07-16%20at%201.09.22%20PM.png)

To switch to the next column, simply press the 'Tab' key on your keyboard.

- To centralize the text and images in the table, select all contents by pressing Ctrl+A (Cmd+A for Mac). Then, click the 'center alignment' option.

![Inline image4](img/Screenshot%202023-07-16%20at%201.12.26%20PM.png)

- Now, let's add the images. Click on the first row and select the 'Image' icon.

![Inline image5](img/Screenshot%202023-07-16%20at%201.13.49%20PM.png)

- Navigate to the 'Upload' tab, choose the desired image file, then click on 'Send it to the Server'.

![Inline image6](img/Screenshot%202023-07-16%20at%201.16.52%20PM.png)

- Once the image is uploaded, the 'Image Info' tab will open. Set the image width to 300 (to avoid the image taking up the whole screen) and the HSpace (horizontal padding) to 10.

![Inline image6](img/Screenshot%202023-07-16%20at%201.20.04%20PM.png)

- Follow the same steps for the other two columns. Your table should look something like this:

![Inline image7](img/Screenshot%202023-07-16%20at%201.21.52%20PM.png)

- Click on 'Maximize' once more to exit the full-screen mode. Click 'Save' to preserve your changes.

- Verify that the newly created landing page section has been added to the current theme. This will ensure your changes are visible on the landing page.

![Inline image7](img/Screenshot%202023-07-16%20at%201.23.51%20PM.png)
