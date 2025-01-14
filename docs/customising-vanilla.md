---
layout: default
---

## Customising Vanilla

<hr>

Here you will find information on customising Vanilla to suit your project.

### Overriding default settings

To override the default settings you must do so _before_ you include Vanilla in your main Sass file. It is good practice to include custom styles in a separate settings file. A list of configurable settings can be found in the [Related section](#related).

```
// Override default Vanilla settings in your main Sass file
$breakpoint-medium: 900px;
$color-accent: #7cf0ee;
$font-base-family: 'Merriweather';
$grid-max-width: 1440px;

// ...or include it from a separate settings file in the same folder
@import 'settings';

// Import Vanilla framework
@import 'vanilla-framework/scss/vanilla';

// Include all of Vanilla Framework
@include vanilla;
```

---

### Importing individual components

Your project may not warrant including all of Vanilla, in which case you can include components modularly. You must at least include `vf-base` as many components depend on the base styling. Below is an example of how to include Vanilla components on an as-needed basis:

```
// Import Vanilla framework
@import 'vanilla-framework/scss/vanilla';

// Include base Vanilla styles
@include vf-base;

// Include the components you want
@include vf-p-buttons;
@include vf-p-forms;
@include vf-p-links;
```

---

### Related

- [Animation settings](/settings/animation-settings)
- [Assets settings](/settings/assets-settings)
- [Breakpoint settings](/settings/breakpoint-settings)
- [Color settings](/settings/color-settings)
- [Font settings](/settings/font-settings)
- [Layout settings](/settings/layout-settings)
- [Placeholder settings](/settings/placeholder-settings)
- [Spacing settings](/settings/spacing-settings)
