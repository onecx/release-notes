# OneCX Portal Release Notes
Release notes for the official **OneCX Portal**[^1] releases. Each release note will tell you what’s new in each version, and will also describe any backwards-incompatible changes made in that version.

## Release 2024-11-12
* Use OneCX lib version 5.23.2
    * Fix: Use local font instaed remote
* Announcement 1.2.0
    * Fix: View announcement details with read only permissions
* Product Store 1.3.0
    * Allow image size up to 200kb
* Theme 1.3.0
    * Improve import with suitable warning messages 
* User Profile 1.4.0
    * Fix: Use HTTP Status code 204 if avatar image does not exist
* Workspace 1.3.0
    * Fix: View menu details with read only permissions
    * Fix: Display loading and exception status on following tabs: roles, slots, products
    * Fix: new backend permissions for product related data [link](https://github.com/onecx/onecx-workspace-bff/commit/dd9b24599b5cf9a16258e952cafaa6634585a372#diff-fae1be0e38e5db5b0a5c9205f249f194e968340bd8918bab56ebfcf5ef3746e1)


## Release 2024-11-05
* Use OneCX lib version 5.22.2
* Shell 1.2.0 [1.2.0](releases/20241105/onecx-shell.md)
    * Fix: The authentication token is shared as long as it is valid.
* Product Store [1.2.0](releases/20241105/onecx-product-store.md)
    * Display workspaces which using a product within a new TAB on detail dialog
    * Display version info in all search results and added version as filter
* Theme [1.2.0](releases/20241105/onecx-theme.md)
    * Fix: If the display name does not exist on import then the theme name is used instead
* User Profile [1.3.0](releases/20241105/onecx-user-profile.md)
    * New backend permissions for admin used endpoints
    * An authorized user can manage the avatar of other users
* Workspace  [1.2.0](releases/20241105/onecx-workspace.md)
    * Fix: If the referenced Theme does not exist then the OneCX default theme settings are used


## Release 2024-10-30
* General Fixes
    * Potential issues with missing Angulars platform browser library in all **OneCX Core Products**
    * Navigation issue with backward navigation between Applications
    * Buttons within Dialogs opened using DialogService are right aligned (OneCX standard)
* Use OneCX lib version 5.22.0 
* Product store [1.1.0](releases/20241030/onecx-product-store.md)
* Data Orchestartor [1.1.0](releases/20241030/onecx-data-orchestrator.md)
* IAM [1.1.0](releases/20241030/onecx-iam.md)
* Shell [1.1.0](releases/20241030/onecx-shell.md)
* Tenant [1.1.0](releases/20241030/onecx-tenant.md)
* Theme [1.1.0](releases/20241030/onecx-theme.md)
* Announcement [1.1.0](releases/20241030/onecx-announcement.md)
    * Increase maximum length of content up to 1000 characters
    * Improve layout of search dialog and banner
    * Improve layout of detail dialog: display remaining characters on text fields, display icon and background color
    * If the announcement text contains line breaks then they are taken into account on displaying
* Help [1.1.0](releases/20241030/onecx-help.md)
    * Improve layout of search and detail dialog
    * Within the search results the complete (used) URL is displayed instead the single parts
    * Align layout of help item editor dialog
* Permissions [1.2.0](releases/20241030/onecx-permission.md)
    * Optimize responsive layout for smaller devices
    * Initial sort order on search result uses display name
    * Improve layout of export dialog
* User Profile [1.2.0](releases/20241030/onecx-user-profile.md)
    * An authorized user (new permissions) can see the roles and permissions of other users
    * An authorized user (new permissions) can delete the user profile of other users
    * Fixing breadcrumbs and translations
* Welcome [1.1.0](releases/20241030/onecx-welcome.md)
    * Improve size and layout of announcement area and detail view
    * If no active announcements exist then no announcement area is displayed
* Workspace [1.1.0](releases/20241030/onecx-workspace.md)
    * Improve menu role loading and filtering
    * Fix basePath issues with starting another existing basePath


[^1]: [OneCX Portal](https://github.com/onecx)
