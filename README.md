# ![Monachese Photography](assets/images/logo-readme.png "Monachese Photography")  onachese Photography

The purpose of this site is to showcase an independent photographer's gallery, demonstrate their ability to digitally enhance photos, and to advertise photo 
sessions and editing packages to meet the photography needs of potential clients. A majority of the images showcased cater to parents and grandparents, however 
these also may appeal to a smaller market of young adults seeking business portraits and clients who wish to digitally enhance photographs.

# Live Protype Demo and WireFrame
+ An active prototype can be found [here](https://richardaeld.github.io/MonaMemorabilia/ "Web Page") at GitHub.
+ The wireframe PNG's can be found [here](https://github.com/Richardaeld/MonaMemorabilia/tree/master/assets/wireframe "Wireframe") also embedded at GitHub.

# UX Choices
![display-responsiveness](assets/images/display-devices.png "display-responsiveness") 
### Home
+ Shows off four eye-catching photos in bootstrap carousel
+ Gives a brief description of the general services offered in a responsive four box layout that makes use of negative space

### Main Nav
+ Includes a clean, responsive bootstrap nav bar
+ Provides a clear display of the company logo in top left corner

### Main Footer
+ Uses Fontawesome icons paired with text to display a contemporary social link design
+ Added social links that could be used by an independent photographer

### About Us
+ Features a Hero image which demonstrates the photographer’s ability to digitally enhance photos. One side of the photo is the original and has no editing, 
    while the other half shows the image after digital enhancement.
+ Features a no-frills text section which emphasizes the exceptional work offered by the company

### Gallery
+ Utilizes negative space to draw the eye to the four categories of sub-gallery image links
+ Images on the page include a *hover* and *scale* feature to provide the appearance of conventional links

### Sub-Galleries (All Pages That Are Linked From Within Gallery)
+ Includes a back button to the main gallery and a two-way in-page nav for user convenience
+ All images have an added *border* and *box-shadow* to give a three-dimensional effect

### Contact Us
+ Contains a simple submission form which prevents users from accidentally submitting without completing the contact information
+ The final box (Describe Your Session needs...) includes plenty of space for users to submit a substantial and well-thought out response

### Image Compression
+ [TinyPNG](https://tinypng.com/) image compression roughly elimates 51% of kb load from images
+ The reduction of image size allows the page to load in roughly 0.241 seconds according to [Pingdom](https://tools.pingdom.com/)


![Tinyify differrence image](assets/images/tiny-ping-combo.png "Displays the minification done to image")

# Brand Identity
+ The headers (h1, h2…) *font-families* match the style of the logo
+ The main page color scheme uses the monochromatic coloration of the logo
+ The pictures used maintain themes of family, digital enhancement, and demonstrate the photographer’s artistic style

# Potential Client Examples
## Clients 
+ As a client, I'd like a framable photograph for a gift
+ As a client, I'd like a portrait photograph for a work portfolio
+ As a client, I'd like a photograph I already own to be digitially improved 
+ As a client, I'd like a photographer to attent a family event to capture natural photos
+ As a client, I'd like a photo session that is considered non-standard 
+ As a client, I'd like a studio photo session with my family

# Testing
## Checking Responsiveness 
Pages should have good UX at a starting resolution of 320*px* width by 568*px* heigth and past 1200*px* wide <br />
+ Assumption:  
    1. Using latest version of Chrome 
    1. A monitor that supports 1080p resolution or greater 
+ Testing steps:
    1. Open index page in Chrome 
    1. Open inspect mode in Chrome browser
    1. Select Responsive tab on top of screen and cycle through all media sizes availiable
        + Check for visual bugs, misalignments, or bad UX at every single size
        + Document any problem area or abnormal occurrence witnessed
    1. Select Responsive tab and select the responsive function
    1. Stretch screen *width* from 320*px* to 1200*px* and beyond
        + Check for visual bugs, misalignments, or bad UX as the pixal width is increased
        + Document any problem area or abnormal occurrence witnessed
+ Expected result:
    1. documentation on all viewable resolutions of bad UX
    1. documentation of where visual bugs or misalignments occure
--------------------------------
## Checking for Errors in Code
Code should not return errors<br />
+ Precondition: 
    1. Website has been deployed and is visible to browsers online
+ Assumption:
    1. Know that vendor extensions do not validate and can be ignored
    1. know that not all warnings given will show code that requires change 
    1. Know that external resources, like Bootstrap, return errors and warning that do not concern this process
+ Testing Steps:
    1. Open deployed website page, copy its index link, and leave open
    1. Open another tab in browser and go to [W3C Markup Validation Service](https://validator.w3.org/)
    1. Paste the link of website page into W3C's validation bar and submit it to see what W3C finds
    1. Document errors and warnings that should be corrected
    1. Repeat steps three and four until all pages have been checked in W3C
    1. Open a tab in browser and go to  [Jigsaw (CSS Validation Service)](https://jigsaw.w3.org/css-validator/)
    1. Paste the link of websites index page into Jigsaws's validation bar and submit it to see what Jigsaw finds
    1. Document errors and warnings that should be corrected
+ Expected result:
    1. List of problem code and where it can be found   
---------------------------------
## Checking for browser support
Should not return time out, have an error, or grapical misalignment when viewed<br />
+ Assumption:
    1. Know what the index page is supposed to look like at different resolutions
+ Testing Steps:
    1. Open deployed website page, copy its index link, and leave open
    1. Open another tab in browser and go to [browser Stack Screenshots](hhttps://www.browserstack.com/screenshots)
    1. Paste the link of index page into Browser Screenshots testing bar
    1. Pick a device or operating system and select the most current versions of browsers supported by said operating system
    1. Repeat step four until there are 25 browser and/or device combinations
    1. Click "Generate" and wait for results to finish
    1. View each screenshot checking for image accuracy
    1. Document the successful generations
    1. Click "Back to Devices" and clear previous selections
    1. Repeat steps four through nine until all operations systems and devices are documented
+ Expected result:
    1. List of supported and none supported browsers and devices 
+ Actual Browserstack results can be found [here](https://github.com/Richardaeld/MonaMemorabilia/tree/master/assets/browserstack)
----------------------------------
## Checking for webpage load times
Should return a load time for page
+ Precondition: 
    1. Website has been deployed and is visible to browsers online
+ Testing Steps:
    1. Open deployed website page, copy its index link, and leave open
    1. Open another tab in browser and go to [Pingdom](https://tools.pingdom.com/)
    1. Paste the link of page into Pingdom "URL" bar and select a location, North America-USA-San Francisco, for "Test from" 
    1. Click "Start Test" and wait for results
    1. Record Results
    1. Repeat steps three through five until all pages have been tested
+ Expected result:
    1. List of load times for site
+ Pingdom results can be found [here](https://github.com/Richardaeld/MonaMemorabilia/tree/master/assets/pingdom)

## Previous and Current Bugs
+ During the programming of this webpage, there were numerous graphical misalignments. These were primarily generated by Bootstrap creating 
    padding and margins and was the result of using rows and container-fluid commands. These were easily taken care of with appropriate padding 
    and margin removal and the use of "!important".
+ Various pages were not filling the entire screen on specific interface devices when using the inspect function in Chrome. By matching the 
    body’s default *background-color* to the footer’s *background-color*, it gives the illusion that the footer's *background-color* extends 
    to the bottom of the screen.
+ The file "Core.python3.2641.1592707923" will crash GitPod when attempting to delete it.
+ When viewing all sub-galleries at an i5 resolution in landscape (568px x 320px) while using the Chrome inspect function, the top and bottom 
    borders of photos cannot be seen due to the size of the nav bar and the physical limitations of the pixels on the screen.

## Supports these operatings systems with current versions of associated browsers 
+ Windows 10
    + Chrome, Internet Explorer, Firefox
+ Windows 8.1, 8.0, 7 
    + Chrome and Internet Explorer
+ Mac OS X Catalina and Mojave
    + Chrome
+ Mac OS X High Sierra, Sierra, and El Capitan
    + Safari and Chrome
+ Mac OX X Yosemite and Mavericks
    + Chrome

## Not Supported Determined by Browserstack and Version of Bootstrap
+ Internet explorer 9 and older
+ Opera 12.15 and older
+ Firefox 3.6 and older
+ Safari 8.0 and older

## Web Browsers That Support Transition Effects Used
+ Chrome 26.0 and newer
+ Internet explorer 10 and newer
+ Firefox 16 and newer
+ Safari 6.1 and newer
+ Opera 12.1 and newer

## Scalability
+ Adding a user operable slide-bar to change images from the original to an edited version could offer better representation on the digital 
    enhancement section and in the About Us section (This feature is outside the scope of this project)
+ The use of a modal in the sub-gallery pages would allow for pictures to pop up instead of relying on a clunky in-page nav
+ Changing *px* to *rem* in CSS would help reduce code length in CSS and add better responsiveness to all pages on smaller devices


# Tool, References, and Code Used
## Tools
+ [Balsmiq](https://balsamiq.com/) - Helped produce the wireframe used for this web page
+ [Bootstrap](https://getbootstrap.com/) - Used as framework
+ [BrowserStack](https://www.browserstack.com/screenshots) - Checking for platform incompatibility
+ [Fontawesome](https://fontawesome.com/v4.7.0/icons/) - Icons used
+ [GitHub](https://github.com/) - Deployment of prototype site
+ [GitPod](https://www.gitpod.io/) - Integrated development environment
+ [Google fonts](https://fonts.google.com/) - Fonts used
+ [Jigsaw(Validation Service)](https://jigsaw.w3.org/css-validator/) - Used to identify errors in CSS
+ [Pingdom](https://tools.pingdom.com/) - Checking for page load time
+ [Techsini](https://techsini.com/multi-mockup/) - for their viewable responsiveness PNG
+ [TinyPNG](https://tinypng.com/) - Minimizing KB load per image
+ [W3C Validator](https://validator.w3.org/) - Used to identify errors in markup

## References and Code used
+ [Webaccessibilitychecklist](http://webaccessibilitychecklist.com/) - Helped with making web page ARIA accessible
+ [MDN web docs](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/What_is_accessibility) - Helped with understanding of when and how to use ARIA
+ [Stack overflow](https://stackoverflow.com/) - Helped in understanding how to correct visual bugs with Bootstrap's automatic padding and margins
+ [W3schools](https://www.w3schools.com/) - Helped with fine-tuning CSS and provided examples of advanced tricks involving *transition*, *hover*, and *scale*. These can be seen in:
    1. Index (*Hover* button effects are found under "Custom Project" and *text-shadow* is used on the busisness name, Monachese Photography)
    2. Main footer (*Hover* effect used for the social media icons)
    3. Gallery and sub-galleries (All nav images use the *scale* effect and a *box-shadow*)
    4. Sub-galleries (The clickable images use a *scale* and *transition* effect. The other images use *box-shadow*)
+ [Bootstrap](https://getbootstrap.com/) -
  1. Main nav (Used responsive design nav bar)
  2. Index (Image carousel)
  3. Contact us (Form)
  4. Sub-Gallery (Scrollspy was used for the in-page nav and the *invisible* properity was used to hide placement of in-page nav snap-to points)
+ Code Institute (Class) - Used footer design based on the golden ratio and made social links like the examples shown in class
+ Used a visual reference from a classmate (Simon "jumboduck") for the About Us section. The idea that was used is a large Hero image followed by the golden 
    ratio of three text boxes that share the *background-color* of the page.

# Technologies
## Languages
+ HTML
+ CSS
+ JS (with Bootstrap)
+ JQuery (with Bootstrap)

# Acknowledgements
+ The idea for this website came from Micheal Monachese because of his forte for photography
+ The photos and logo were created by Micheal Monachese
+ Felipe Souza Alarcon for guidance and providing a plethora of information and web-based applications
+ Emily Grooms for help in revising this README document
