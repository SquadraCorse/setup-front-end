# FB front-end 

> Static front-end code for our website FB with total package for testing and deploying our complete code. We can easily deliver components and build new versions using grunt.

### [Visit the website →](http://squadracorse.github.io/build-frontend/)

## Getting Started
This installation requires NodeJS and Grunt `~0.4.1`. Eventually we will introduce SASS wich will require SASS, bourbon and libsass.org (for now Ruby, will change after compress becomes stable) as well.

Our default task makes our complete package for distribution. Make sure to update versioning inside "package.json" when deploying (use SNAPSHOT's only when testing). It will deliver a zip which can be diffed with our previous one.

```bash
grunt
```

While developing html/css/js you run the development environment which has liverelaod.

```bash
grunt dev
```

If you then wish to check the compiled and build front-end you can run the following command which will run a webserver on your default browser running our compiled front-end.

```bash
grunt server
```

First run this visual check after switching to your last released tag(so: switch, grunt, grunt visual). This will create the images to compare with. Then switch back to your feature branch or master. So always run grunt test for mocha testing with coverage but for simple visual check you can use.

```bash
grunt visual
```

It is also possible to select simple tasks like 'lint' or 'watch' or 'clean'. Our watcher currenlty looks for changes in JavaScript and documentation pages (actually handlebar templates). Next time we will use livereload.

```js
grunt lint (csslint and jshint)
grunt watch
```

Happy coding. Work from master, make a feature branch if you wish to upgrade a component. Always diff your deliveries (zip file). Tag when doing a deployment. Talk with your team!

## Authors

**Maarten van Oudenniel**

+ [github/squadracorse](http://squadracorse.github.io/build-frontend)
+ [maas38](http://maas38.com)


## Release History
27-03-2014 v0.0.3 Added i18n support and lazy modules load using Stephan Bakker his innitcomponents
23-03-2014 v0.0.2 Added SASS support and added visual check
22-03-2014 v0.0.1 Basic setup using Grunt and Require for building/testing and documentation
