# Joon: Roon theme for Jekyll

Jekyll theme based on the Roon for [Ghost](http://github.com/tryghost/roon/).

## Demo
View this jekyll theme in action [here](https://vormwald.github.io/joon)

## Screenshot
![screenshot](https://raw.githubusercontent.com/vormwald/joon/master/screenshot.png)

## Font Options

This theme comes with two font options; a serif and sans-serif (the default). 
Switching between them is done in the HTML, by adding `serif` to the `class` of 
the `<body>` element in [head.html](https://github.com/vormwald/joon/blob/master/_layouts/default.html.hbs#L6).

## Colour Options

This theme uses an accent colour for links and the border at the top of pages.

To change this colour, you need to edit [assets/css/screen.css](https://github.com/vormwald/joon/blob/master/assets/css/screen.css).

There are only two values you need to change, conveniently **located at the very
top of the file**.

## For More Information
For more on Jekyll, read the [documentation](http://jekyllrb.com/)


## Copyright & License

Roon is Copyright (c) 2013-2015 Sam Soffes & Ghost Foundation - Released under 
the [MIT license](LICENSE).

## Serve

Serve locally with

    bundle exec jekyll serve

## Ruby Instruction (from homebrew)

    ==> ruby
    By default, binaries installed by gem will be placed into:
      /usr/local/lib/ruby/gems/2.7.0/bin

    You may want to add this to your PATH.

    ruby is keg-only, which means it was not symlinked into /usr/local,
    because macOS already provides this software and installing another version in
    parallel can cause all kinds of trouble.

    If you need to have ruby first in your PATH run:
      echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc

    For compilers to find ruby you may need to set:
      export LDFLAGS="-L/usr/local/opt/ruby/lib"
      export CPPFLAGS="-I/usr/local/opt/ruby/include"

    For pkg-config to find ruby you may need to set:
      export PKG_CONFIG_PATH="/usr/local/opt/ruby/lib/pkgconfig"
