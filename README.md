# [Sassline](https://sassline.com)

Set text on the web to a baseline grid with Sass & rems using a responsive modular-scale.

`Please note this code is p old now and is no longer actively maintained.`

## Do one thing well

Sassline has one aim and one aim only – to spread better typography across the responsive environment of the web.

The idea is to have easy to use and maintain SCSS partials utilising the power of Sass to make the complex calculations to set type on a baseline grid on the web, with a production ready CSS output. Using rems for the font-sizing and the spacing measurements gives a simple way to use the proportions of the baseline grid throughout the design. Sass mixins do all the heavy lifting so your job is easy.

OpenType features are enabled with `font-feature-settings` to give the most appropriate formatting of text and some flourishes in the headings if available in the web font and supported in the browser.

Sassline includes some basic layouts, and includes mixins to create a main column with optimal measure and a sidebar that doesn’t get too narrow.

## Root font-size = ½ line-height

Sassline works by setting the root font-size as half the line-height of the standard paragraph text. The height of the baseline grid is then effectively set at 2rem, with increments at each 1rem. This makes it nice and easy to work proportionally from the baseline with integer rem values to create harmony in your layout and typography. This is based off a technique for setting text in print documents.

## Documentation

Sassline is fully commented with details in the SCSS. Set the font sizes with the `fontsize` mixin, set the spacing using the `baseline` mixin or set both at once with the `sassline` mixin. Use rems for everything else. Full documentation is in the works.

### Running / compiling

You can also use your preferred methods for compiling Sass as long as you have Sass 3.3.7+. To just include the necessary partials in your existing sass project, you only need to import [sassline-base.scss](assets/sass/_sassline-base.scss).

If you want to run Sassline as a standalone project use the gulp setup included (or modify it to your needs).

1. Clone the repo or grab the zip file
2. Open a terminal window and `cd` into this directory
3. Run `npm install -g gulp` (this may need sudo in front)
4. Run `npm install`

Once that is done you can start the server with `gulp` and stop it with `ctrl` + `c`.

The pages will run at http://localhost:1234/

### Sass file structure

My preferred method is to work along the lines of the SMACSS & BEM method. In the sass folder there there are two folders — sassline-base and modules. The base folder has the Sassline base SCSS partials. The modules folder contains some demo SCSS partials with styles you can keep or remove. All new partials should be added to the modules folder and referenced in `style.scss` to be compiled into your CSS.

### More on information on using Sassline

Please see [this blog post](https://jakegiltsoff.co.uk/posts/sassline-v2-0).

## Responsive Nav

Viljami Salminen’s [responsive-nav.js](https://github.com/viljamis/responsive-nav.js) plugin is included to provide a mobile-ready navigation to work from.

## Browsers

Sassline will set text to the baseline in recent versions of Chrome and Firefox, IE 11+ and Safari 8+.

## Roadmap

- Full documentation

========

## License

Sassline is licensed under the MIT license. ([http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT))
