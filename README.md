Ponticons is the icon font for PMEase. Most of the icons are based on below famous icon set:

* [Octicons](https://github.com/github/octicons)
* [Fontawesome](http://fontawesome.io)
* [Fontello](http://fontello.com)
* [Ionicons](http://ionicons.com)

# Add Icons

Add svg file to src directory, then update `builder/manifest.json`.

## Build Instructions

Build is based on the famous icon font [ionicons](https://github.com/driftyco/ionicons)

This repo already comes with all the files built and ready to go, but can also build the fonts from the source. Requires Python, FontForge and Sass:

1) Install FontForge, which is the program that creates the font files from the SVG files:

    $ brew install fontforge ttfautohint

2) Install [Sass](http://sass-lang.com/)

    $ gem install sass

3) Add or subtract files from the `src/` folder you'd like to be apart of the font files.

4) Modify any settings in the `builder/manifest.json` file. You can change the name of the font-family and CSS classname prefix.

5) Run the build command:

    python ./builder/generate.py

## License

Ponticons is licensed under the [MIT license](http://opensource.org/licenses/MIT).

