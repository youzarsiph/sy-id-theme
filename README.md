# Syrian Identity Theme

![Logo](src/assets/images/logos/eagle.png)

[![CI](https://github.com/youzarsiph/sy-id-theme/actions/workflows/ci.yml/badge.svg)](https://github.com/youzarsiph/sy-id-theme/actions/workflows/ci.yml)
[![CD](https://github.com/youzarsiph/sy-id-theme/actions/workflows/cd.yml/badge.svg)](https://github.com/youzarsiph/sy-id-theme/actions/workflows/cd.yml)

## Overview

[**Live Demo**](https://play.tailwindcss.com/iQtTPySoN7)

`sy-id-theme` is a custom UI theme designed to facilitate the development of web
applications aligned with the official Syrian Identity design system. Built on
top of [`Tailwind CSS`](https://tailwindcss.com/) and the
[`daisyUI`](https://daisyui.com/) component library, this package provides a
comprehensive suite of branding assets, including the official color palette,
typography, logos, and standardized background patterns.

## Key Features

- **Official Design System Integration:** Pre-configured with the precise Syrian
  Identity color palette and branding guidelines.
- **Tailwind CSS Utility:** Fully compatible with Tailwind CSS, offering
  complete access to its extensive utility class framework.
- **daisyUI Component Library:** Seamlessly integrates with daisyUI, allowing
  developers to leverage scalable, pre-built semantic UI components.
- **Bundled Brand Assets:** Includes ready-to-use fonts, official logos, and
  thematic background patterns.

## Quick Start Guide

> **Note:** If your project already has `tailwindcss`,
> `@tailwindcss/typography`, and `daisyui` installed, you can bypass manual
> configuration by simply copying the contents of [`src/app.css`](src/app.css)
> directly into your main stylesheet.

To integrate the `sy-id-theme` into your project from scratch, follow these
setup instructions:

1. **Initialize Tailwind CSS:** Ensure Tailwind CSS is configured in your
   project. Refer to the
   [official Tailwind documentation](https://tailwindcss.com/docs/installation/)
   for guidance.
2. **Install daisyUI:** Add [`daisyui`](https://daisyui.com/docs/install/) to
   your project dependencies.
3. **Configure the Theme:** Open your main stylesheet and append the custom
   theme configuration immediately following the daisyUI plugin directive
   (`@plugin "@daisyui";`):

   ```css
   @plugin "daisyui/theme" {
     name: "syrian";
     default: true;
     prefersdark: false;
     color-scheme: "light";
     --color-base-100: oklch(100% 0 0);
     --color-base-200: oklch(98% 0 0);
     --color-base-300: oklch(96% 0 0);
     --color-base-content: oklch(20% 0 0);
     --color-primary: oklch(34.1% 0.059 179.567);
     --color-primary-content: oklch(100% 0 0);
     --color-secondary: oklch(73.3% 0.065 89.121);
     --color-secondary-content: oklch(20% 0 0);
     --color-accent: oklch(28.5% 0.080 13.735);
     --color-accent-content: oklch(100% 0 0);
     --color-neutral: oklch(35.2% 0.004 354.953);
     --color-neutral-content: oklch(92% 0.003 48.717);
     --color-info: oklch(74% 0.16 232.661);
     --color-info-content: oklch(39% 0.09 240.876);
     --color-success: oklch(76% 0.177 163.223);
     --color-success-content: oklch(37% 0.077 168.94);
     --color-warning: oklch(82% 0.189 84.429);
     --color-warning-content: oklch(41% 0.112 45.904);
     --color-error: oklch(70% 0.191 22.216);
     --color-error-content: oklch(39% 0.141 25.723);
     --radius-selector: 1rem;
     --radius-field: 0.5rem;
     --radius-box: 1rem;
     --size-selector: 0.25rem;
     --size-field: 0.25rem;
     --border: 1px;
     --depth: 1;
     --noise: 1;
   }
   ```

4. **Apply the Theme:** Declare the theme in your HTML document by adding the
   `data-theme="syrian"` attribute to the root `<html>` tag:

   ```html
   <!DOCTYPE html>
   <html lang="en" data-theme="syrian">
     <head>
       <!-- Meta tags and other head elements -->
       <link rel="stylesheet" href="path/to/your/styles.css" />
     </head>

     <body>
       <!-- Your application content -->
     </body>
   </html>
   ```

## Assets

All visual and typographic assets required for the Syrian Identity design system
are located in the [`src/assets/`](src/assets/) directory. This includes:

- **Fonts:** Official brand typography files.
- **Logos:** High-resolution and scalable vector formats of the official logo.
- **Backgrounds:** Standardized graphical patterns for thematic consistency.

## Resources

For further information regarding the official design guidelines, please refer
to the following resources:

- [Syrian Identity Portal](http://syrianidentity.sy/)
- [Syrian Visual Identity Official Website](https://visual-identity.momc.gov.sy/)

## Contributing

We welcome and appreciate community contributions. If you are interested in
improving this theme, please review our
[Contribution Guidelines](CONTRIBUTING.md) for detailed instructions on
workflows, coding standards, and submission processes. Your input is vital to
the ongoing enhancement of this project.

## Support

If you encounter technical issues, have configuration questions, or wish to
suggest new features, please open an issue in the project repository. We
actively monitor feedback to ensure the continuous reliability and improvement
of the theme.

## Licensing

This project is distributed under the MIT License. Please review the
[LICENSE](LICENSE) file for comprehensive terms and conditions.
