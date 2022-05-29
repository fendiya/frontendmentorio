The 7/1 structure pattern
sass/
|
|– abstracts/ (or utilities/)
|   |– _variables.scss    // Sass Variables
|   |– _functions.scss    // Sass Functions
|   |– _mixins.scss       // Sass Mixins
|
|– base/
|   |– _reset.scss        // Reset/normalize
|   |– _typography.scss   // Typography rules
|
|– components/ (or modules/)
|   |– _buttons.scss      // Buttons
|   |– _carousel.scss     // Carousel
|   |– _slider.scss       // Slider
|
|– layout/
|   |– _navigation.scss   // Navigation
|   |– _grid.scss         // Grid system
|   |– _header.scss       // Header
|   |– _footer.scss       // Footer
|   |– _sidebar.scss      // Sidebar
|   |– _forms.scss        // Forms
|
|– pages/
|   |– _home.scss         // Home specific styles
|   |– _about.scss        // About specific styles
|   |– _contact.scss      // Contact specific styles
|
|– themes/
|   |– _theme.scss        // Default theme
|   |– _admin.scss        // Admin theme
|
|– vendors/
|   |– _bootstrap.scss    // Bootstrap
|   |– _jquery-ui.scss    // jQuery UI
|
`– main.scss              // Main Sass file


Our folders would typically contain the following.

Abstracts contains tools, helpers, variables, mixins etc.
Base contains boilerplate code for the project. This includes styles such as resets, typography etc.
Components contains all the smaller page components like separated into multiple smaller files like slider, carousel etc.
Layout contains the layout styles, separated into several smaller files like header, footer etc.
Pages contains page-specific styles. For example, the home page and search results page typically looks very different.
Themes contains files that are theme specific, like alternate color schemes (if any).
Vendors contains third party code from external framworks and libraries like jQueryUi, Bootstrap etc.
Our main file is only used to import all the other files.

NOTE Files should be imported according to the folder they live in, one after the other, unless they need to be in a specific order. For example, vendor code like normalize.css should be above any other styles.