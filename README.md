# Offer Reports Drupal 7 Module

This a sample of the module made for https://www.netplaytv.com/ . When unistalled all data relating to module is wiped from DB.

## How it works
The module creates two pages (/offer & /offer-reports) as well as a Cookie (agree_offer_report).

### Offer Reports Content Type
There are only two additional fields added to this Content Type (Date and File) - we do not include a Body Field.

### Adding Offer Reports
* We create a Content Type and it is this that hold all content for /offer-reports. 
* This content type will only accept a Title, Date and File Upload (should be PDF).
* These are displayed in order of creation on Website. 

### Offer Reports Page 
* This is created and populated using a view. Any configuration (like Title) can be done inside the "Offer Reports View"

### Offer Page
* This page is generated by the module file. The default version of this page is just a title with Agree or Disagree.
* In order to edit this page you will need to Edit the "Offer Page Content Block" page after the module is created (this will also be removed by Module when uninstalled).


### Better Implementation (Not included due to priority being assigned elsewhere)
 * Detection of prior named pages and renaming module ones to suit
 * Configurable Aliases
 * SimpleTest Functionality (to test Front End functionality)