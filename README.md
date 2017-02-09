# Heroku buildpack

This is a Heroku buildpack for using pngquant version 2.8.2 in your application.

## Usage

To use this buildpack you'll first need to set it as your custom buildpack:

    $ heroku buildpacks:set https://github.com/heroku/heroku-buildpack-multi.git

From here you will need to create a `.buildpacks` file which contains (in order) the buildpacks you wish to run when you deploy:

    $ cat .buildpacks
    https://github.com/gaussgroup/heroku-buildpack-pngquant
    https://github.com/heroku/heroku-buildpack-ruby
