# Project Title

GoogleFontsSassTester
It makes it easy to test google fonts while developing a project. Every time the Sass code is compiled, a random google font combination is used reducing the time needed to preview the appearence of different font. 

### Prerequisites

It requires Sass.

### Installing

Add the following line in the global configuration Sass file in your project (for example style.scss):

@import "googleFontsTester";

To customize the fonts you want to test for your project modify the following lists in the _googleFontsSassTester.scss file:

-> $gft_h_fonts: populate with the font families you want to test for headings
-> $gft_b_fonts: populate with the font families you want to test for body text

To use the fonts just reference the following variables in you custom scss files:

-> $header-font-family 
-> $body-font-family 

For example:

h1 {
   font-family; $header-font-family;
}

p {
   font-family; $body-font-family;
}

In case you want either the header font or the body font to be keep constant just set the appropiate value for the $gft_h_font and $gft_b_font variables.

For example:

$gft_h_font: 'Abril Fatface';
$gft_b_font: '';

to keep the header font constant equal to 'Abril Fatface' and play randomly with body text font.



