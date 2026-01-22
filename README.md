# OneCX Portal Release Notes
Release notes for the official **OneCX Portal**[^1] releases. Each release note will tell you what’s new in each version, and will also describe any backwards-incompatible changes made in that version.


## Release 2026-x-y
* Announcement 1.x.0
* IAM 1.x.0
    * Feat: Manage IDM Users and Roles (planned)
* Help 1.x.0
* Parameter 1.x.0
* Permission 1.x.0
    * Feat: Use product data via slot and remote component (planned)
      * SLOT: onecx-product-data => new => ./OneCXProductDataComponent (product-store)
* Product Store 1.x.0
* Shell 2.0.0
    * Fix: translate "Unauthorized" (planned)
    * Feat: new default favicon (planned)
* Tenant 1.x.0
* Test 1.x.0
* Theme 1.x.0
* User Profile 1.x.0
* Welcome 1.x.0
* Workspace 1.x.0
    * Feat: Improve slot TAB layout using a tree with several quick views (planned)
    * Feat: Display indicator of non-existing theme on workspace tiles (planned)
    * Feat: Use product data via slot and remote component in product TAB (planned)


## Release 2026-01-23
* Announcement 1.8.0
    * Feat: Improvements of a11y in search/detail/delete dialog
    * Feat: Improvements of search/detail/delete dialog layout for huge display names
    * Feat: Use product data via slot and remote component
      * SLOT: onecx-product-data => new => ./OneCXProductDataComponent (product-store)
    * Feat: Use workspace data via slot and remote component
      * SLOT: onecx-workspace-data => new => ./OneCXWorkspaceDataComponent (workspace)
* IAM 1.9.0
    * Feat: Replace onecx-iam-kc-svc with onecx-iam-svc
* Help 1.7.0
    * Feat: Improve layout of missing help article dialog
    * Feat: Improvements of a11y in search/detail/delete dialog
    * Feat: Improvements of search/detail/delete dialog layout for huge display names
    * Feat: Use product data via slot and remote component
      * SLOT: onecx-product-data => new => ./OneCXProductDataComponent (product-store)
* Parameter 1.8.0
    * Feat: Replaced slots
      * SLOT: onecx-product-infos => onecx-product-data
* Permission 1.10.0
    * Feat: Improve responsive layout of application detail dialogg and a11y
* Product Store 1.13.0
    * Feat: Removed slot
      * SLOT: onecx-product-list-workspaces-using-product
    * Feat: Removed remote components
      * Component: ./OneCXProductInfosComponent
    * Feat: Displaying multi-tenancy flag on product tiles in product search
* Shell 2.0.0
* Tenant 1.8.0
* Test 1.10.0
* Theme 1.11.0
    * Feat: Remove Slots
      * onecx-theme-list-workspaces-using-theme
    * Feat: Improvements in RC for current theme logo (external URLs and small logos)
    * Feat: Improvements of image management for logos
    * Feat: add small Logo
* User Profile 1.12.0
    * Feat: Add permission PROFILE_IDM#VIEW
* Welcome 1.9.0
* Workspace 1.20.0
    * Fix:  Logout menu item clickable
    * Fix:  Use query parameter correctly on routing menu item links
    * Fix:  Reorder menu items
    * Feat: Add filter for role assignments by role column header
    * Feat: Improve menu layout: message displaying, routing
    * Feat: Remove Slots
      * onecx-page-footer-menu
      * onecx-theme-infos
    * Feat: Remove Components
      * ./OneCXWorkspaceFooterComponent
    * Feat: Add target property for menu items (values: _self, _blank) - _self is default
    * Feat: Improvements in RC for current workspace logo (external URLs and small logos)
    * Feat: Improvements of image management for logos
    * Feat: Improvements of a11y in menu and menu detail dialog
    * Feat: Improvements of a11y in detail dialog, several TABs
    * Feat: Improvements of search/detail/delete dialog layout for huge display names
    * Feat: Add small logo
    * Feat: Allow SVG as logo format


## Release 2025-08-15
* All UIs
    * Use OneCX Angular 18 Lib 5.47.4
    * Use OneCX Angular 19 Lib 6.5.3
    * Use docker-spa 1.18.0
    * Fix: Secure q endpoints
* All SVC/BFFs: Use Quarkus 3.20.0
* Announcement 1.7.0
* Data Orchestrator 1.7.0
    * Fix: Editing CDR
    * Feat: Add Parameter as CDR (Custom Data Resource)
    * Feat: CDR types are fetch from BFF (configured via env. variables)
* IAM 1.8.0
    * Feat: Multi Keycloak support for searching, permissions adjusted:
      * REALM#SEARCH             => removed
      * role,provider,user       admin-read
      * role,user                admin-write
      * provider                 read
      * password                 write
      * endpoints: users, roles
* Help 1.6.0
    * Feat: Improve test coverage
* Parameter 1.6.0
    * Feat: Display validation error on parameters with JSON object type
    * Feat: parameter service v2 (change endpoints) - do not use
    * Feat: Use product data via slot and remote component
      * SLOT: onecx-product-data => new => ./OneCXProductDataComponent (product-store)
    * Feat: Outdated slots
      * SLOT: onecx-product-infos => outdated
* Permission 1.9.0
    * Fix: Quick filters in search/detail page have always a value
* Product Store 1.12.0
    * Fix: translate ok and nok message on copy apps
    * Feat: Add Slot management, new UI permissions
      * SLOT#CREATE => onecx-product-store-ui
      * SLOT#EDIT   => onecx-product-store-ui
      * SLOT#VIEW   => onecx-product-store-ui
    * Feat: Redesign slot overview: use table style, group product names, filter slot/product names
    * Feat: Added search criteria provider and classifications for products/applications
    * Feat: Provide a remote component for product data
      * Component: ./OneCXProductDataComponent => onecx-product-data (help, ...)
    * Feat: Outdated slots
      * SLOT: onecx-product-list-workspaces-using-product
    * Feat: Outdated remote components
      * Component: ./OneCXProductInfosComponent
* Shell 2.2.0
    * Feat: Support of Angular 18 and 19
    * Fix: URL on page initialization error is stable now on reload
    * Feat: Reactivate shell footer slot
      * SLOT: onecx-shell-footer => with following components assigned
        * ./OneCXCurrentThemeLogo (theme)
        * ./OneCXFooterMenuComponent (workspace)
        * ./OneCXVersionInfoComponent (workspace)
    * Feat: New slot for header left region
      * SLOT: onecx-shell-header-left => new => ./OneCXCurrentThemeLogo (theme)
    * Feat: Improve accessibility: use footer tag on page
    * Feat: Add reload action on page for workspace initialization error
    * Feat: Outdated slots
      * SLOT: onecx-page-footer
* Tenant 1.7.0
    * Feat: Improve UI layout
* Test 1.9.0
* Theme 1.10.0
    * Feat: Provide a remote component to display the logo of the current theme
      * Component: ./OneCXCurrentThemeLogo => onecx-shell-header-left, onecx-shell-footer
      * Component: ./OneCXThemeInfosComponent => undeployed (not longer supported)
    * Feat: Provide a new slot for usage of theme in workspaces
      * SLOT: onecx-workspace-data => new => ./OneCXWorkspaceDataComponent (workspace)
    * Feat: Outdated slots
      * SLOT: onecx-theme-list-workspaces-using-theme
* User Profile 1.11.0
    * Feat: Improve accessibility
    * Feat: Display IDM provider and issuer within personal data
    * Fix: Time zone and color scheme settings disabled because they are not currently in use
* Welcome 1.8.0
    * Fix: display a single URL background image
* Workspace 1.18.0
    * Fix: Manage assignments of components to slots
    * Fix: use native footer tag in workspace footer (aria/a11y issue)
    * Fix: use product default logo in product TAB for products
    * Fix: Quick filters in roles/slots/products/menu TABs have always a value
    * Feat: Extend slot quick filter for outdated slots
    * Feat: Improve item filter in slot detail and product TAB
    * Feat: Provide a remote component for workspace data
      * Component: ./OneCXWorkspaceDataComponent => onecx-workspace-data (theme, ...)
    * Feat: Outdated slots
      * SLOT: onecx-page-footer-menu
      * SLOT: onecx-theme-infos
    * Feat: Outdated/Removed remote components
      * Component: ./OneCXWorkspaceFooterComponent
      * Component: ./OneCXListWorkspacesUsingThemeComponent
      * Component: ./OneCXListWorkspacesUsingProductComponent


## Release 2025-07-11 (FIX)
* Parameter 1.5.0
    * Fix: Operator stores values now as imported value (before: in value)


## Release 2025-06-26
* Shell 1.11.1
    * Feat: Added tenant ID to user profile, aligned to user-profile-svc v1 API
* User Profile 1.9.1
    * Feat: Added tenant ID to user profile service v1 API


## Release 2025-04-11
* For all UIs: Use OneCX lib 5.34.5
* For all UIs: Use docker-spa 1.14.0
* For all UIs: Use Angular 18.2.13
* For all SVC/BFFs: Use Quarkus 3.15.0
* Data Orchestrator 1.5.0
    * Feat: Improve UI: responsible forms, fix minor UI issues
* Permissions 1.7.0
    * Fix: Improve Microservice display names
* Product Store 1.9.0
    * Fix: Improve Microservice display names
    * Feat: Add product search criteria for provider and classifications
      * Model change: new table PRODUCT_CLASSIFICATION with 1:n realtionship to product
* Shell 1.11.0
    * Fix: Improve Microservice display names
    * Fix: Improve menu and topbar styles
    * Feat: Use a slot to display page footer
      * SLOT: onecx-page-footer => new => ./OneCXWorkspaceFooterComponent (workspace)
      * SLOT: onecx-shell-footer => outdated
* Test 1.6.0
* Theme 1.8.0
    * Fix: Improve Microservice display names
    * Feat: Improve layout of tiles in theme search results
    * Feat: Provide a remote component for theme information (logo, themes etc.)
      * Component: ./OneCXThemeDataComponent => onecx-theme-data (workspace)
* User Profile 1.9.0
    * Fix: Improve Microservice display names
    * Fix: Uploading big avatar image successfully
    * Feat: Uploading avatar images up to 500.000 bytes
    * Feat: Improve avatar image compression
* Workspace 1.15.0
    * Fix: Improve Microservice display names
    * Fix: Use default avatar icons if avatar image cannot ne loaded, in user sidebar/avatar menu
    * Feat: New Microservice onecx-workspace-api-legacy
    * Feat: Provide a slot for additional custom user info, displayed on top of avatar menu, below user name
      * SLOT: onecx-custom-user-info => new
    * Feat: Provide a remote component for page footer
      * Component: ./OneCXWorkspaceFooterComponent => onecx-page-footer (shell)
      * SLOT: onecx-page-footer-menu => new => ./OneCXFooterMenuComponent (workspace)
      * SLOT: onecx-theme-data => new => ./OneCXThemeDataComponent (theme)
    * Feat: Improve layout of displaying avatar image and user display name within user menu
    * Feat: Improve workspace detail: use display names of Themes and show theme logo
    * Feat: Improve workspace export: sorting product, slots, components by name
    * Feat: Improve workspace import: upload possible if display name, theme, base url are missing


## Release 2025-04-02
* Product Store 1.7.0
    * Feat: Bigger tiles for product search results
* Shell 1.10.0
    * Fix: Set height of main content area to 100%
* Workspace 1.10.0
    * Feat: Bigger tiles for workspace search results


## Release 2025-03-17
* For all UIs: Use OneCX lib 5.32.1
* For all UIs: Use docker-spa 1.14.0
* For all UIs: Use Angular 18.2.12
* For all SVC/BFFs: Use Quarkus 3.15.xx
* Announcement 1.5.0
* Data Orchestrator 1.4.0
* IAM 1.5.0
    * Feat: Add realm as search criteria (single value drop down)
      * Permission: REALM # SEARCH
      * Permission: realm # read
    * Feat: Display user details within modal dialog => USER#VIEW
      * Permission: IAM_ROLE # VIEW
    * Feat: Display user permissions within modal dialog
      * Slot: onecx-iam-user-permissions => ./OneCXUserRolesPermissionsComponent
      * Permission: PERMISSION#VIEW
    * Feat: Provide Remote Component for IAM User Roles
      * Component: ./OneCXIamUserRolesComponent
* Help 1.4.0
* Permissions 1.6.0
    * Feat: Display user assigned roles contained in token or iam roles
      * Slot: onecx-permission-iam-user-roles => ./OneCXIamUserRolesComponent
      * Permission: IAM_ROLE#VIEW
    * Feat: Improve layout of app search using ocx-chip
* Product Store 1.6.0
    * Fix: filter for product classifications
    * Fix: enable endpoint TAB in app detail dialog again
    * Feat: Linking app detail from endpoint search results
* Shell 1.9.0
    * Fix: Use empty favicon if theme does not provide favicon
    * Fix: Reduce number of logo image loading
    * Fix: Cleanup basic layout of header, footer, menu sections
    * Fix: Disable limitations of dimensions (overflow, height) of modal dialogs
* Tenant 1.5.0
* Test 1.2.0
* Theme 1.7.0
    * Feat: Add deletion of logo and favicon
    * Feat: Add mandatory flag and manag it in designer dialog
    * Feat: Improve deletion dialog: prevent deletion if mandatory flag is set or Theme is in use
* User Profile 1.8.0
    * Feat: Added permission to see IAM user roles
* Welcome 1.6.0
    * Feat: Use OneCX standard page layout for Welcome Configuration
    * Feat: Import and Export of Welcome configuration and images
    * Feat: Improve responsive layout
    * Feat: Improve test coverage
* Workspace 1.9.0
    * Fix: Adjust translations
    * Fix: Multiple reorder of registered products
    * Feat: Fallback theme on import
    * Feat: Improve Workspace menu and detail layout
    * Feat: Improve Workspace role detail layout
    * Feat: Improve Workspace import
    * Feat: Improve layout of roles and slots overview using ocx-chip
    * Feat: Use specific slot and IAM remote component to display IAM roles
      * Slot: onecx-iam-user-roles => ./OneCXIamUserRolesComponent


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
