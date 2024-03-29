Series 40 Web Apps UI Visualisation Examples
============================================

Series 40 Web Apps UI Visualisation Examples demonstrates the use of different
kinds of UI elements, navigational solutions, and patterns created with HTML, 
CSS and JavaScript technologies. The example is meant for both designers and 
developers: designers get an impression of how the components actually look 
on the device, and developers learn how to use the Series 40 Web Apps UI 
components.

The application has been designed for Series 40 full touch, touch and type, 
and most recent non-touch devices. Please note that Nokia Browser version 
2.0 or higher is required for the application to run properly, as certain 
features (such as file uploading or downloading and WQVGA displays) are not 
supported by older browser versions.

The application suite contains examples of the following components and 
patterns:

* Elements
    * Buttons - demonstrates different Button layouts.
    * Radio buttons - demonstrates the use of radio buttons.
    * Check boxes - demonstrates how to create and use check boxes.
    * Lists - demonstrates various list types.
    * Tabs - demonstrates using tabs within a Web Application.
    * Text Fields - demonstrates different types of text fields.

* Navigation
    * Carousel, In-Item - demonstrates using -webkit-transitions with a sliding
      image container.
    * Carousel, Item - as Carousel In-Item, but with full screen.
    * Dynamic Looping - demonstrates using dynamically loaded content using both
      MWL-methods and JavaScript.
    * Expandable List - demonstrates how to create an accordion list.
    * Picker - demonstrates selecting a value for a button from a list.
    * Tabbed pages - demonstrates navigation within a web application using tabs.
    * Tree Structure - demonstrates how to create a dynamic, three levels deep
      tree-like navigational example.
  
* Patterns
    * File upload demonstrates selecting and sending a file with HTML forms.
    * File download demonstrates downloading and saving a file from a server.
    * Page Title Link demonstrates tree structure -like navigation, with added
      title link.
    * Passwords example demonstrates using HTML password input and saving
      information to cloud.
    * Web Page Link demonstrates opening a web link from within a web app.
    * Search demonstrates how to implement searching functionality to a web
      application.
    * Sharing content example demonstrates how to incorporate sharing content
      via SMS or Facebook with web app technologies.
	
In brief, this example application demonstrates:
* Different UI "components" (i.e. HTML, CSS & JavaScript code snippets) and
  design patterns that can be used in Series 40 Web Apps.
* Navigating between web app 'views'.
* How to accommodate different input methods in a web application.

Note that the application was created to demonstrate the UI components and does
not have any actual engine implementation.

The application is hosted in GitHub:
* https://github.com/nokia-developer/web-apps-ui-component-demos

1. Prerequisites
-------------------------------------------------------------------------------
* HTML basics
* CSS basics
* JavaScript basics
* Series 40 Web Apps & Mobile Web Library basics


2. Project structure and implementation
-------------------------------------------------------------------------------

2.1 Folders
-----------
| Folder | Description |
|--------|-------------|
| root | The root folder contains the main index.html file, licence information and this README file |
| css | Contains style definition files for landscape & portrait modes. |
| img | Contains graphics (icons and images) that are packaged within the application widget package.|
| js | Contains application logic script files. |
| screenshots | Contains screenshots taken from the application. |


2.2 Important files and classes
-------------------------------

| File                    | Description |
|-------------------------|-------------|
| index.html              | Defines the HMTL structure of each of the mini apps. Also has most of MWL related functionality. |
| utils.js                | Contains the JavaScript functions implementing the more complex application logic. |
| single_portrait.css, single_landscape.css | Files that have the CSS classes that define the application look and feel on different devices. |

2.3 Used APIs
----------------------------------------------

The following APIs have been used. 

MWL functions:
* iterateClass()
* loadURL()
* scrollTo()
* setGroupTarget()
* stopTimer()
* switchClass()
* timer()
* toggleClass()

JavaScript APIs:
* document.getElementById
* Math.random()
* Math.floor()
* widget.preferences.setItem()
* widget.preferences.clear()

CSS3 features:
* webkit-transition


3. Compatibility
-------------------------------------------------------------------------------

Compatible with:
* Nokia Series 40 full touch, touch and type, and non-touch (landscape) 
  devices with Nokia Browser 2.0 or newer

Tested on:
* Nokia Asha 306
* Nokia Asha 303
* Nokia Asha 201

Developed with:
* Nokia Web Developer Environment / Nokia Web Tools 2.0


3.2 Known issues and design limitations
---------------------------------------

In Series 40 Web Apps, you can implement some business logic locally by 
switching between CSS classes (i.e., MWL functions), but often logic needs to 
be executed on the Nokia proxy side (intermediate server). Latency is then 
unavoidable because data is transferred over a mobile network. In the UI 
Visualisation Demos, most latency can be seen in **Dynamic looping**, **Search**, 
**Tree View**, and **Page Title Link** examples, because each of these examples 
has some logic that has to be executed on the server. 


4. Building, installing, and running the application
-------------------------------------------------------------------------------

4.1 Preparations
----------------

Check that you have the latest Nokia Web Developer Environment installed and
the latest Nokia Browser version on the device.

Nokia Web Tools 2.0 or higher is required.
Only Nokia Browser v2.0 and higher are supported.

4.2 Using the Nokia Web Developer Environment
---------------------------------------------

You can preview and deploy the web application on a server by using the WDE.
Open the project in the SDK, and select either local/cloud preview, or select
deploy Web App for deploying it on the web server.
For more details about the Nokia Web Developer Environment and deploying apps,
visit the Getting Started with Series 40 Web Apps at Nokia Developer
(http://www.developer.nokia.com/Develop/Series_40/Series_40_web_apps/Getting_started/).

4.3 Nokia Series 40 device
--------------------------

Use the device's browser to navigate to the short URL given by the Nokia WDE
upon deployment. The web browser will identify it as an web application and
it will be loaded on the device.

It is also possible to use Bluetooth deployment, which will start the browser
automatically to the correct URL address. This requires that the Bluetooth
launcher is installed on the device.

5. Licence
-------------------------------------------------------------------------------

See the licence text file delivered with this project. The licence file is also
available online at
https://github.com/nokia-developer/web-apps-ui-component-demos/blob/master/LICENCE.TXT


6. Related documentation
-------------------------------------------------------------------------------
Mobile Web Library
* http://www.developer.nokia.com/Resources/Library/Series_40_web_apps_library/#!technical-library/descriptions-of-mwl-methods.html

Web Apps Design Library:
* http://developer.nokia.com/Resources/Library/Nokia_Asha_web_apps_library/#!design-library.html

HTML 4.01
* http://www.w3.org/TR/1999/REC-html401-19991224/

JavaScript 1.6
* https://developer.mozilla.org/en/JavaScript/Reference
* https://developer.mozilla.org/en/JavaScript/New_in_JavaScript/1.6

CSS Mobile Profile 2
* http://www.w3.org/TR/2008/CR-css-mobile-20081210/


7. Version history
-------------------------------------------------------------------------------

* 1.0 Initial release.
