* Aha Branding
** Purpose
This holds the branding styles for the Genesys Aha ideas portal. This helps us maintain control of the branding and gives us version history.

All three products have their own portals and this code has be structured to ensure consistency and minimize duplication.

** Instructions
We should not be editing the styles directly on the Aha site. All changes should be made here first and then copied to the idea portals.

To update the portal branding..
1. Navigate to the portal for a product. (ex. PureConnect)
2. Click Configure Portal > Portal Branding Tab (You will need admin access for this.)
3. Copy contents of custom.html into the Custom Header field.
4. Copy contents of custom.css into the Custom CSS field.
5. Copy contents of custom.js into the Custom Javascript Field.
6. Click save.
7. Repeate steps 1-6 for remaining portals.

** Components
*** Custom.html
This is the html template for the header and should be identical for all product portals except for the logo and title. Simply change the css class of each (ex. pureconnect-logo and pureconnect-title) for each portal to pull in the appropriate content.

*** custom.css
This is the css class that will be included in the header and affects the styles for the entire page. All styles should go into this file and it should be identical for each portal. If there are any styles that are specific to a product they should be included in this stylesheet and should use a selector that contains that product name.

*** custom.js
This is the code that actually puts the individual logo and title into the header. It uses jquery to find the title and logo selector and appends the appropriate html.