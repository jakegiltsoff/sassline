# Sassline

Set text on the web to a baseline grid with Sass & rems. [Sassline](http://sassline.com) can be used for blogs, prototyping, and other web projects. It has recommended base typography styling and mixins to work proportionally from the baseline grid. Select a modular-scale for each breakpoint and work responsively type-first.

## v2

Version 2 of Sassline has been vastly improved with the use of Sass 3.3 and Sass maps. The mixins are now much more powerful and flexible. Make sure to keep reading to find out how to use the mixins and how they work. Note: as v1.1 pixel fallbacks are not included for rems.

## Demo

A demo of Sassline in action can be viewed with web fonts [here](http://demo.sassline.com), and local fonts [here](http://demo.sassline.com/local-fonts).

## Do one thing well

There are many different options when it comes to boilerplates, frameworks and pattern libraries these days. Sassline has one aim and one aim only – to spread better typography across the responsive environment that is the web.

The idea is to have easy to use and maintain SCSS files utilising the power of Sass to make the complex calculations to set type on a baseline grid on the web, with a production ready CSS output. Using rems for the font-sizing and the spacing measurements gives a simple way to use the proportions of the baseline grid throughout the design. Sass mixins do all the heavy lifting so your job is easy.

OpenType features are enabled to give the nicest formatting of text and some flourishes in the headings if available in the web font and supported in the browser.

## Root font-size = ½ line-height

Sassline is based on setting the root font-size as half the line-height of the paragraph text. The height of the baseline grid is then effectively set at 2rem, with increments at each 1rem. This makes it nice and easy to work proportionally from the baseline with integer rem values.

## Smaller web fonts for mobiles

Getting the most out of OpenType features can end up with large typeface files being served to your site as discussed on the [Typekit blog](http://blog.typekit.com/2013/04/17/fallback-fonts-on-mobile-devices). Included in Sassline is a method for using a smaller kit (without the full character sets) at smaller viewport sizes where OpenType support is low anyway to save downloading the extra characters.

## Documentation

Sassline is fully commented with details in the SCSS. Set the font sizes with the font-size mixin, set the spacing using the baseline mixin or set both at once with the sassline mixin. Use rems for everything else. Here are some other key points:

### Compiling Sass

Using Sass 3.3.7+ and Sass-Globbing:

`sass -r sass-globbing --watch assets/sass:assets/css`

Alternatively a Mixture simple project settings file is included which will compile the Sass + minify for you (as well as much more). Sassline is also available as a mixture boilerplate [here](https://github.com/designbyjake/sassline-mixture).

You can also used your preferred methods for compiling sass as long as you have Sass 3.3.7+ and Sass-Globbing enabled.

### Sass file structure

My preferred method is to work along the lines of the SMACSS & BEM method. In the sass folder there there are two folders — base and modules. The base folder has the Sassline base SCSS partials. Use the modules folder contains some demo SCSS partials with styles you can keep or remove. All new partials added to modules will be compiled into your css so work in here with new files. 

### Using Sassline

Please see [this blog post](http://jakegiltsoff.co.uk/posts/sassline-v2-0).

## Responsive Nav

Viljami Salminen’s [responsive-nav.js](https://github.com/viljamis/responsive-nav.js) plugin is included to provide a mobile ready navigation to work from.


## Roadmap

- More complex demos
- Lightweight Sass grid system

========

## License

The MIT License (MIT)

Copyright (c) 2013-2014 Jake Giltsoff

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.