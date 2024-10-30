# OneCX Portal Release Notes
Release notes for the official **OneCX Portal**[^1] releases. Each release note will tell you what’s new in each version, and will also describe any backwards-incompatible changes made in that version.
## 1.1.0 release (2024-10-30)

* Fixes
    * Potential issues with missing Angulars platform browser library in all **OneCX Core Products**
    * Navigation issue with backward navigation between Applications
    * Buttons within Dialogs opened using DialogService are right aligned (OneCX standard)
* Use OneCX lib version 5.22.0
* Permissions
    * Optimize responsive layout for smaller devices
    * Initial sort order on search result uses display name
    * Improve layout of export dialog
* Workspace
    * Improve menu role loading and filtering
    * Fix basePath issues with starting another existing basePath
* Help
    * Improve layout of search and detail dialog
    * Within the search results the complete (used) URL is displayed instead the single parts
    * Align layout of help item editor dialog
* Announcement
    * Increase maximum length of content up to 1000 characters
    * Improve layout of search dialog and banner
    * Improve layout of detail dialog: display remaining characters on text fields, display icon and background color
    * If the announcement text contains line breaks then they are taken into account on displaying
* User Profile
    * An authorized user (new permissions) can see the roles and permissions of other users
    * An authorized user (new permissions) can delete the user profile of other users
    * Fixing breadcrumbs and translations
* Welcome
    * Improve size and layout of announcement area and detail view
    * If no active announcements exist then no announcement area is displayed


[^1]: [OneCX Portal](https://github.com/onecx)
