# Jekyll Boilerplate

__Jekyll starter project including full setup for gulp, Sass, Autoprefixer, Browserify, imagemin, Browsersync, PostCSS etc.__

## Documentation

### System Preparation
To use this starter project, you'll need the following things installed on your machine.
[Jekyll](https://jekyllrb.com) & [Bundler](https://bundler.io)
```sh
$ gem install jekyll bundler
```
[Nodejs](https://nodejs.org)
user the installer, Homebrew, etc.

### Local Installation
Clone this repo, or download it into a directory of your voice.
```sh
$ git clone https://github.com/mrdemonwolf/jekyll-boilerplate.git
```
Inside the directory, run `npm install`.
```sh
$ cd jekyll-boilerplate
$ npm install
```

### Usage
**Note:** If you have trouble with the commands, prepending `bundle exec` to your
commands may solve it. e.g.
```sh
$ bundle exec npm start
```

### Start the Development
This will give you file watching, browser synchronisation, auto-rebuild, CSS injecting, etc.
```sh
$ npm start
```

### Build for Production
This will set the `JEKYLL_ENV` to `production` and use the production config file(s)
set in `mrdemonwolf.config.js` to override default settings.
```sh
$ npm run build
```

### See More Commands
This will display all available commands.
```sh
$ npm run
```

### Jekyll
As this is just a Jekyll project, you can use any of the commands listed in their [docs](https://jekyllrb.com/docs/usage)

### What's in DemonWolf Jekyll Boilerplate
* [gulp](https://gulpjs.com)
* [Sass](https://sass-lang.com)
* [Autoprefixer](https://github.com/postcss/autoprefixer)
* [PostCSS](https://postcss.org)
* [Webpack](https://webpack.github.io)
* [UglifyJS](https://github.com/mishoo/uglifyJS2)
* [imagemin](https://github.com/imagemin/imagemin)
* [Browsersync](https://www.browsersync.io)

### Configuration and Defaults
You can change the configurations by editing `mrdemonwolf.config.js`

#### Port
default: `4000`
options: integer

#### Tasks
Tasks to run when you exec `npm start` or `gulp` commands.

* **Imagemin**
To minify images.
default: `true`
options: boolean (`true` / `false`)

* **sass**
To compile Sass.
default: `true`
options: boolean (`true` / `false`)

* **server**
To compile sources via Jekyll and to keep browsers in sync with file
changes via Browsersync.
default: `true`
options: boolean (`true` / `false`)

#### Paths
Settings related to the paths.

* **dest**
The destination directory for the whole project.
default: `"_site"`
options: string

* **posts**
The directory of posts source files.
default: `"_posts"`
options: string

* **assets**
The directory to gather all assets.
default: `"./assets"`
options: string

* **css**
The CSS desination directory for Sass.
default: `"css"`
options: string
example: `"stylesheets"`

* **js**
The JavaScript destination directory for Browserify
default: `"js"`
options: string
example: `"javascripts"`

* **images**
The destination directory of compressed image files for imagemin.
default: `"images"`
options: string
example `"img"`

* **sass**
The directory of Sass files.
default: `"_sass"`
options: string
example: `"src/sass"`

* **jsSrc**
The directory of JavaScript source files to bundle up by Browserify.
default: `"_js"`
options: string
example: `"src/js"`

* **imagesSrc**
The directory of image source files to compress.
default: `"_images"`
options: string
example: `"src/images"`

#### Jekyll
Jekyll settings.

#### Config
Jekyll config files.

* **default**
The default Jekyll config file(s).
default: `"_config.yml"`
options: string (`"FILE1[,FILE2,...]"`)
example: `"_config1.ym,_config2.yml"`

* **development**
Development mode config file(s) to override default settings.
default: `""`
options: string(`"FILE1[,FILE2,...]"`)
example: `"_config_development"`

* **production**
Production mode config file(s) to override default settings.
default: `""`
options: string(`"FILE1[,FILE2,...]"`)
example: `"_config_production"`

#### Sass
Sass settings.

* **outputStyle**
Teh output style of Sass.
default: `"compressed"`
options: `"expanded"`, `"nested"`, `"compact"`, `"compressed"`

#### autoprefixer
Autoprefixer settings

* **browsers**
List of browsers, which are supported in your theme.
default: `["> 1%", "last 2 versions", "Firefox ESR"]`
options: array. See [Browserslist docs](https://github.com/ai/browserslist#queries) for available queries.
example: `["> 5%", "last 2 versions", "IE 8"]`

#### JS
JavaScript settings.

* **entry**
File name(s) of JavaScript entry points.
default: `["main.js"]`
options: array
example: `["pluginA.js", "pluginB.js", "main.js"]`

## Copyright and License

Copyright 2018 MrDemonWolf. Code released under the [MIT](https://github.com/mrdemonwolf/jekyllrb-boilerplate/blob/master/LICENSE) license.

