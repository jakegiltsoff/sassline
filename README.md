# [Sassline](http://sassline.com)

Set text on the web to a baseline grid with Sass & rems using a responsive modular-scale.

## New in v2.1

Layouts added with new mixins to create a main column with optimal measure and a sidebar that doesn’t get too narrow. Better baseline grid overlay.

## Do one thing well

Sassline has one aim and one aim only – to spread better typography across the responsive environment of the web.

The idea is to have easy to use and maintain SCSS partials utilising the power of Sass to make the complex calculations to set type on a baseline grid on the web, with a production ready CSS output. Using rems for the font-sizing and the spacing measurements gives a simple way to use the proportions of the baseline grid throughout the design. Sass mixins do all the heavy lifting so your job is easy.

OpenType features are enabled with `font-feature-settings` to give the most appropriate formatting of text and some flourishes in the headings if available in the web font and supported in the browser.

## Root font-size = ½ line-height

Sassline works by setting the root font-size as half the line-height of the standard paragraph text. The height of the baseline grid is then effectively set at 2rem, with increments at each 1rem. This makes it nice and easy to work proportionally from the baseline with integer rem values. This is based of a technique for setting text in print documents.

## Documentation

Sassline is fully commented with details in the SCSS. Set the font sizes with the `font-size` mixin, set the spacing using the `baseline` mixin or set both at once with the `sassline` mixin. Use rems for everything else. Full documentation is in the works.

### Compiling Sass

Using Sass 3.3.7+ and Sass-Globbing:

`sass -r sass-globbing --watch assets/sass:assets/css`

Alternatively a Mixture simple project settings file is included which will compile the Sass + minify for you (as well as much more).

You can also use your preferred methods for compiling sass as long as you have Sass 3.3.7+ and Sass-Globbing enabled.

### Sass file structure

My preferred method is to work along the lines of the SMACSS & BEM method. In the sass folder there there are two folders — base and modules. The base folder has the Sassline base SCSS partials. The modules folder contains some demo SCSS partials with styles you can keep or remove. All new partials added to modules will be compiled into your css so work in here with new files.

### More on information on using Sassline

Please see [this blog post](https://jakegiltsoff.co.uk/posts/sassline-v2-0).

## Responsive Nav

Viljami Salminen’s [responsive-nav.js](https://github.com/viljamis/responsive-nav.js) plugin is included to provide a mobile-ready navigation to work from.


## ¯\\\_( Browsers )_/¯

Sassline will set text to the baseline in recent versions of Chrome and Firefox, IE 11+ and Safari 8+.

## Roadmap

- Full documentation

========

## License

Sassline is licensed under the MIT license. ([http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT))
