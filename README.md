# Bread.CSS :bread: - A CSS Framework created using Sass and Sass partials.

Contributors: Taro Routly, Taylor Baker, Lauren Brunet, Paul Decker
Created for MTM6407 - Web Development IV

Bread.CSS is a follow up CSS framework to our in-class lab creating Butter.CSS to learn about SaSS partials and framework organization.

## Installation

### Direct CSS Implementation

If you are looking to directly import this theme without changing variables, we recommend downloading the already compiled CSS file. 

For that, there are two options: 
- To download the readable CSS document, go to [`dist/bread.css`](/dist/bread.min.css)

- To download the minified CSS document, go to [`dist/bread.min.css`](/dist/bread.min.css).


These files should be added to your project by adding the file into your project's CSS folder, then add the link to the stylesheet in the head of your document using the relative path of the bread.css file. 

Example: `<link rel="stylesheet" href="./css/bread.css">`

### Source Code Implementation

If you are looking to modify the theme to fit your project's needs, we recommend that you download our source code .zip file, which can be found at [`dist/bread-source-code.zip`](/dist/bread-source-code.zip).

This option may be difficult for people new to [SaSS](https://sass-lang.com/), so we recommend only people with an understanding of complex CSS and beginner level SaSS knowledge do this path. Below has more information on the variables.

SaSS **MUST** be installed on your machine to modify the source code and see updates in your compiled CSS.


## Components
We included 4 components in Bread.CSS: Breadcrumbs, buttons, cards, and infoboxes. 
See [our Homepage](https://rout0052.github.io/mtm6407-css-framework/ "Home") for more information.


## Variables
The variables in Bread.CSS are customizable when doing the *source code installation* (if you are importing the CSS file, it is still possible to change variable values, you would just need to search and replace every instance of the variable, which seems like far too much work).

Here is a table with the variable maps used in Bread.CSS.

| **File Name**                    | **Map Name**       | **Map Values**                                                                                                                                                                                                                                                                   |
|------------------------------------|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| src/variables/**_borders.scss**    | $border-style        | 'none': none,<br>'dotted': dotted,<br>'dashed': dashed,<br>'solid': solid,<br>'double': double,<br>'inset': inset,<br>'outset': outset                                                                                                                                             |
| src/variables/**_borders.scss**    | $border-width        | 'none': 0pt,<br>'xs': 1pt,<br>'sm': 2pt,<br>'md': 4pt,<br>'lg': 8pt,<br>'xl': 16pt                                                                                                                                                                                                 |
| src/variables/**_colors.scss**     | $theme-colors        | 'primary': #b7c4d1,<br>'secondary': #574435,<br>'neutral': #e6e0d6,<br>'success': #bdc4bb,<br>'danger': #fdbfb2,<br>'warning': #e4de94,<br>'info': #cfb6db,<br>'light': #eeeeee,<br>'dark': #333333                                                                                |
| src/variables/**_colors.scss**     | $theme-colors-hovers | 'primary': #587089,<br>'secondary': #c9b5a6,<br>'neutral': #e6cfa7,<br>'success': #586255,<br>'danger': #e46d53,<br>'warning': #ede364,<br>'info': #9267a6,<br>'light': #c2c2c2,<br>'dark': #242424                                                                                |
| src/variables/**_display.scss**    | $display-type        | 'none': none, <br>'block': block,<br>'flex': flex,<br>'grid': grid,<br>'inline-block': inline-block,<br>'inline-flex': inline-flex,<br>'inline-grid': inline-grid                                                                                                                  |
| src/variables/**_display.scss**    | $content-alignment   | 'flex-start': flex-start,<br>'flex-end': flex-end,<br>'center': center,<br>'space-between': space-between,<br>'space-around': space-around,<br>'space-evenly': space-evenly                                                                                                        |
| src/variables/**_display.scss**    | $cursor-styles       | 'none': none,<br>'default': default,<br>'auto': auto,<br>'pointer': pointer,<br>'help': help,<br>'crosshair': crosshair,<br>'grab': grab,<br>'not-allowed': not-allowed,<br>'progress': progress,<br>'text': text,<br>'wait': wait,<br>'zoom-in': zoom-in,<br>'zoom-out': zoom-out |
| src/variables/**_sizing.scss**     | $spacing-sizes       | 'none': 0rem,<br>'xxs': 0.1rem,<br>'xs': 0.25rem,<br>'sm': 0.5rem,<br>'md': 0.75rem, <br>'lg': 1rem,<br>'xl': 1.5rem,<br>'xxl': 3rem                                                                                                                                               |
| src/variables/**_sizing.scss**     | $border-radius-sizes | 'none': 0rem,    <br>'small': 0.5rem,<br>'medium': 1rem,<br>'large': 2rem,<br>'circle': 50%                                                                                                                                                                                        |
| src/variables/**_sizing.scss**     | $container-sizes     | '10': 10%,<br>'20': 20%,<br>'30': 30%,<br>'40': 40%,<br>'50': 50%,<br>'60': 60%,<br>'70': 70%,<br>'80': 80%,<br>'90': 90%,<br>'100': 100%,<br>'quarter': 25%,<br>'half': 50%,<br>'3-quarter': 75%,<br>'third': 'calc(100% * 1/3)',<br>'2-third': 'calc(100% * 2/3)'                |
| src/variables/**_typography.scss** | $fonts               | 'body': 'Montserrat',<br>'heading': 'Lora'                                                                                                                                                                                                                                         |
| src/variables/**_typography.scss** | $font-size           | 'xs': 0.75rem,<br>'sm': 1rem,<br>'md': 1.5rem,<br>'lg': 2rem,<br>'xl': 3.75rem,<br>'2xl': 4.5rem                                                                                                                                                                                   |
| src/variables/**_typography.scss** | $font-weight         | 'thin': 100,<br>'extralight': 200,<br>'light': 300,<br>'regular': 400,<br>'medium': 500,<br>'semibold': 600,<br>'bold': 700,<br>'extrabold': 800,<br>'black': 900                                                                                                                  |
| src/variables/**_typography.scss** | $text-alignment      | 'center': center,<br>'left': left,<br>'right': right,<br>'justify': justify                                                                                                                                                                                                        |


### Adding Fonts
To add new fonts to the theme, go to to the `src/fonts` folder and add a new file. The naming convention for this file should be `_font-name.scss`, replacing 'font-name' with the actual name of your font, in lowercase. Then, add the new file name to `src/fonts/index.scss` as `@forward './font-name';`, without the _ or .scss extention. 

To overwrite the current default for body and headings, go to `src/variables/_typography.scss` and change the values of the $fonts map to the new font name as you would declare it in the CSS property `font-family`, without the sans-serif or serif declaration. 

### Adding Icons 
To add a new icon set without getting rid of the old one, go to to the `src/icons/` folder and add a new file. The naming convention for this file should be `_icon-kit-name.scss`, replacing 'icon-kit-name' with the actual name of your icon kit, in lowercase. Then, add the new file name to `src/icons/index.scss` as `@forward './icon-kit-name';`, without the _ or .scss extention. 

To overwrite the current icon set with a new one, change the `@import` statement in `src/icons/_icons.scss` to the one used for the new icon set. 

### Modifying Colors
To modify the theme colors, go to `src/variables/_colors.scss` and modify **both** the `$theme-colors` and `$theme-colors-hovers` map with your new colours and an associated color for its hover state.

Components may need to be updated to adjust for colour contrast issues.