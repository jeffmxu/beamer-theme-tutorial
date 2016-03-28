## `tutorial`  
**version 0.3.6**  
A light modern LaTeX Beamer theme for academics

+ style
  - `light`x`minimal` flat style based on Szeged 
+ color
  - `whale` with energetic text colors
+ font
  - Fira Sans typeface font theme from [Metropolis](https://github.com/matze/mtheme)

`tutorial` [title page](/demo/tutorial-title.pdf), [style gallery](/demo/tutorial-style.pdf) and its full [demo slides](/demo/tutorial-demo.pdf)



## Installation
+ theme
  - (frequent, recommended) allocate both `sty` files into your Beamer theme `texpath`, or
  - (occasional) leave them aside with your main `tex` file
+ font
  - (`xelatex`, recommended) install Fira Sans typeface from [Mozilla](https://www.mozilla.org/en-US/styleguide/products/firefox-os/typeface/), or
  - (`pdflatex`) MiKTeX might install `FiraSans`, `FiraMono` and `newtxsf` packages on the fly 
+ document
  - write your main `tex` file header as follows
  - replace either `<options>` with comma-separated `light` and/or `minimal`
  - recommend to enable _both_ options for minimal visual noise
```latex
\documentclass[<options>]{beamer}
\usetheme[<options>]{tutorial}
```



## Intention
+ originally designed for my weekly tutorial sessions --- hence _default_ `tutorial` keeps
  - headline section navigation bar
  - footline presentation information  
  in each non-title frame for students' reference in class
+ extended with `light`x`minimal` options for less visual noise
  - `light` background for headline, footline and frametitle
  - `minimal` without headline or footline but frame number
+ traditional Beamer Blended Blue x white color theme in accordance with
  - current "mainstream" presentation preference in Academia
  - convenient inclusion of graphs and/or tables with white background
+ convenient to customize your own colors as follows for
  - main theme `structure` and general background
  - `normal text`, `alerted text` and `example text`  
  where an asterisk `*` means to _reset both_ `fg` and `bg` values
```latex
\setbeamercolor*{structure}{fg=<main color>, bg=<background>}
\setbeamercolor{<text style>}{fg=<text color>}
``` 



## Limitation
+ headline section navigation bar _always_ coexists with footline information
+ math and text font theme not carefully adjusted yet
+ fixed frame numbering style
  - frame number only for `minimal`
  - otherwise shown as a fraction
+ theme options cannot `\PassOptionsToClass` or `\PassOptionsToPackage` through command line
+ common Beamer `compress` option untuned



## Licensing
`tutorial` may be distributed and/or modified under the [LaTeX Project Public License 1.3](http://www.latex-project.org/lppl.txt "LPPLv1.3c") and/or under the [GNU General Public License 3.0](http://www.gnu.org/licenses/gpl-3.0.txt "GNU GPLv3").

`tutorial` is also required to be licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/ "CC-BY-SA-4.0").  
This means that if you modify the theme and/or distribute it, you are required to retain the copyright notice header and license it under the same CC-BY-SA license.
This does not affect the presentation created with the theme.
![CC-BY-SA](https://i.creativecommons.org/l/by-sa/4.0/80x15.png "CC-BY-SA-4.0")
