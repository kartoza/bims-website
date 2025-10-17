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

# Custom Fonts

Here, users can add custom fonts to the platform to customise any text in the BIMS Theme tables (eg., Landing page). Custom fonts are added from [Google Fonts](https://fonts.google.com/) only. If the required font is not available on Google Fonts, it cannot be added.

![BIMS Theme](<img/Screenshot 2025-10-17 094500.png>)

### Steps:

- 	Click "+ Add custom font". Users will need to populate the Name, Css URL and Stack fields in the form using information sourced from Google Fonts.

![Add custom font-1](<img/Screenshot 2025-09-22 100032.png>)

- In a new browser tab, paste the URL: https://fonts.google.com/
- Search and select the custom fonts required. 

![Add custom font-2](<img/Screenshot 2025-09-22 100207.png>)

- Click "Get font" in the top right-hand corner.

![Add custom font-3](<img/Screenshot 2025-09-22 100357.png>)

- Select the " <> Get embed code " button. 

![Add custom font-4](<img/Screenshot 2025-09-22 100429.png>)

- In the first grey box, copy all the text in quotation marks after link href, excluding the rel = > part as shown below:
![Add custom font-5](<img/Screenshot 2025-09-22 100526.png>)
Users will copy https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100..900;1,100..900&display=swap

- Return to the BIMS admin window and paste the copied text into the Css URL

![Add custom font-6](<img/Screenshot 2025-09-22 100706.png>)

- Return to the Google Fonts page, under "CSS class for a variable style", copy font-family and paste it into the BIMS custom fonts in both the Name and Stack.

![Add custom font-7](<img/Screenshot 2025-09-22 100815.png>)

In the example above, users will copy and paste Roboto into the BIMS custom fonts form:

![Add custom font-8](<img/Screenshot 2025-09-22 100932.png>)

- Once all fields in the Custom fonts form are filled, tick 'Is active' and click Save.