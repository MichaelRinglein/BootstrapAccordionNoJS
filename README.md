# BootstrappAccordionNoJS
The Bootstrap Accordion with the collapse functionality but without the Bootstrap.js or jQuery.js (or other external JS libraries)

## Why this project?
The accordion is part of a series of animation I make for a client. Those animations are loaded into already existing websites.

Therefore the accordion needs to work without any external JS library (like Bootstrap.js or jQuery) to avoid any possible conflicts between different loaded Javascript libraries.

## How it works
First I deleted all bootrap data toggle from the HTML tags (aria-labelledby, data-parent, data-toggle, data-target, aria-expanded, aria-controls) since we don't need those anymore

Second I changed and added the id's in the Card buttons and Card bodies.

Third I added the onclick="togglePanel(this)" to each button. 

The togglePanel(this) function loops through all available Panels and switches all off but the selected by simply adding or deleting Bootraps own "show" class.
