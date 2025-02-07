# OneCX Portal Release Notes
Release notes for the official **OneCX Portal**[^1] releases. Each release note will tell you what’s new in each version, and will also describe any backwards-incompatible changes made in that version.


## Release 2025-02-xx
* For all UIs: Use OneCX lib version 5.xx.x
* For all UIs: using docker-spa 1.xx.0
* IAM 1.4.0 => need tbc.
    * Increase the max number search result in UI => 1000
    * User per Role => GET /admin/realms/{realm}/roles/{role-name}/users
    * User Count => GET /admin/realms/{realm}/users/count
    * User Roles => GET /admin/realms/{realm}/users/profile/metadata
* Help 1.4.0
    * Improve test coverage (planned)
* Product Store 1.6.0
    * Fix: enable endpoint TAB in app detail dialog again
    * Feat: Linking app detail from endpoint search results
* Shell 1.9.0
    * Fix: Reduce number of logo image loading (planned)
* User Profile 1.8.0
    * Fix: Display the current avatar image after change (planned)
    * Feat: Improve avatar image compression (planned)
* Welcome 1.5.0
    * Feat: Import and Export of Welcome configuration and images
    * Test coverage 100%
* Workspace 1.6.0
    * Fix: Adjust translations


## Release 2025-02-03
* For all UIs: Use OneCX lib version 5.30.0
* For all UIs: using docker-spa 1.11.0
* Announcement 1.4.0
* Data Orchestrator 1.3.0
* IAM 1.3.0
* Help 1.3.0
* Permissions 1.5.0
    * Display message if IAM user not exists in RC user permissions
* Product Store 1.5.0
    * New UI permission: ENDPOINT#SEARCH
    * Feat: added endpoint overview page
    * Fix: search by criteria
* Shell 1.8.0
* Tenant 1.4.0
* Theme 1.6.0
    * Feat: Improve save-as dialog and fix auto apply in designer
    * Feat: prevent theme deletion in UI if theme is used by a workspace
    * Feat: allow ico as accepted format for favicon
    * Feat: store and use original MIME-TYPE for favicon and logo
* User Profile 1.7.0
* Welcome 1.4.0
    * Feat: New styling option for each image setting CSS properties in detail dialog
    * Feat: Improve detail dialog: step through all images
    * Feat: Foreground color uses an inverted color as used for background
* Workspace 1.6.0
    * Feat: Display names of registered applications are editable now
    * Feat: Import workspaces do not overwrite existing workspaces


## Release 2025-01-16
* For all UIs: Use OneCX lib version 5.30.0
* For all UIs: Bitnami image replaced by native nginx image
* For all UIs: using docker-spa 1.10.0
* For all UIs: Security improvements
* Announcement [1.3.0](releases/20250116/onecx-announcement.md)
    * Fix: align Angular setup
    * Improve layout and efficiency of search page (frozen columns, ...)
    * Improve layout of detail dialog: using TABs
* Data Orchestrator [1.2.0](releases/20250116/onecx-data-orchestrator.md)
* IAM [1.2.0](releases/20250116/onecx-iam.md)
* Help [1.2.0](releases/20250116/onecx-help.md)
    * Fix: align Angular setup
    * Improve layouts and efficiency of search and detail dialog (frozen columns, ...)
* Permissions [1.4.0](releases/20250116/onecx-permission.md)
    * Display message if IAM user not exists in RC user permissions
* Product Store [1.4.0](releases/20250116/onecx-product-store.md)
    * Fix: remove unused scope ocx-ws:read
* Shell [1.7.0](releases/20250116/onecx-shell.md)
    * Add OneCX background image
    * Improve error pages used if something went wrong during app/page loading
* Theme [1.5.0](releases/20250116/onecx-theme.md)
* Tenant [1.2.0](releases/20250116/onecx-tenant.md)
* User Profile [1.6.0](releases/20250116/onecx-user-profile.md)
    * Fix: Display dedicated message on detail if user does not exist anymore in IDM
    * Use profile id instead user id (IAM) on admin requests
    * Improve layout and permission handling within profile search
    * Reduce number of backend requests
* Welcome [1.3.0](releases/20250116/onecx-welcome.md)
    * Add OneCX background image
    * Fix: align Angular setup
* Workspace [1.5.0](releases/20250116/onecx-workpace.md)
    * Fix: Preview menu during workspace import
    * Improve layout of menu mgmt
    * Add role filter in menu mgmt to display the menu according to selected roles


## Release 2024-12-02
* Use OneCX lib version 5.28.0
* Permission [1.3.0](releases/20241202/onecx-permission.md)
    * Fix: update Angular setup
    * Added a filter for role in detail dialogue
    * Layout improvements in detail dialogue (zebra look, frozen columns)
    * If IAM is not available then display message
    * Display messages on import conflicts
* Product Store [1.4.0](releases/20241202/onecx-product-store.md)
    * Fix: remove unused scope ocx-ws:read
* Shell [1.6.0](releases/20241202/onecx-shell.md)
    * Improve start/default pages used if something went wrong on page loading
    * Fix: favicon URL
* Theme [1.4.0](releases/20241202/onecx-theme.md)
    * Fix: update Angular setup
    * Fix: remove unused scope ocx-ws:read
* User Profile [1.5.0](releases/20241202/onecx-user-profile.md)
    * Fix: update Angular setup
    * Fix: user profile search
    * Fix: manage avatar images of user
    * Improve test coverage
* Workspace [1.4.0](releases/20241202/onecx-workspace.md)
    * Fix: update Angular setup
    * Improve layout of menu mgmt
    * Improve layout of deletion dialogs
    * Improve test coverage
    * If IAM cannot be used then disable the use in roles TAB


## Release 2024-11-15
* Use OneCX lib version 5.26.0
* Shell [1.5.0](releases/20241115/onecx-shell.md)
    * Fix: Rate HTTP Status code 204 as error on getting images
* User Profile [1.4.0](releases/20241115/onecx-user-profile.md)
    * Fix: Use HTTP Status code 204 if avatar image does not exist
    * Use default settings (lang, menu position) for new user-profiles via environment variables


## Release 2024-11-14
* Use OneCX lib version 5.25.0
* Shell [1.4.0](releases/20241114/onecx-shell.md)
    * In ocx-data-table the select-all checkbox is checked if all options are checked
    * In ocx-data-table the column order is updated after reorder in column group dialog
    * In ocx-data-table and ocx-data-list only the things are rendered which are in viewport
    * In ocx-data-table the column headers are align to top and the sort/filter are on next row
    * There is a environment variable to control the order of search criteria actions


## Release 2024-11-13
* Use OneCX lib version 5.23.6
    * Fix: Use local font instaed remote
* Shell [1.3.0](releases/20241113/onecx-shell.md)
    * Filter view component with chips and overlay
* Announcement [1.2.0](releases/20241113/onecx-announcement.md)
    * Fix: View announcement details with read only permissions
* Product Store [1.3.0](releases/20241113/onecx-product-store.md)
    * Allow image size up to 200kb
* Theme [1.3.0](releases/20241113/onecx-theme.md)
    * Improve import with suitable warning messages 
* Workspace [1.3.0](releases/20241113/onecx-workspace.md)
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
