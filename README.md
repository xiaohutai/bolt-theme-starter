# Starter, a Bolt Theme

A simple theme with re-usable components.


## Installation

There are two options to get this theme:

- Install this theme via the Bolt backend at `/bolt/extensions`.
- Do a `composer require xiaohutai/bolt-theme-starter` in your Bolt's `extensions` folder.

For making pull requests, you need to navigate to your Bolt's `themes` folder,
then:

```sh
git clone git@github.com:xiaohutai/bolt-theme-starter.git
```


## Getting Started

```sh
# Install dependencies
npm install

# For development: Serve the website with hot reload for css and js files.
npm start

# For production: Build and minify all assets.
npm run build
```

| Command                | Description                              | Minification? |
|------------------------|------------------------------------------|---------------|
| `npm run sass`         | Compile SASS to CSS                      | ❌           |
| `npm run postcss`      | PostCSS (polyfill, autoprefixer)         | ✅           |
| `npm run styles`       | Build styles (`sass` + `postcss`)        | ✅           |
| `npm run scripts`      | Compile JS                               | ❌           |
| `npm run build`        | Build everything (`styles` + `scripts`)  | ✅           |
| `npm run lint`         | Lint styles                              |               |
| `npm run eslint`       | Lint scripts                             |               |


### Configuration


#### Babel

```
.babelrc
```

- [.babelrc](https://babeljs.io/docs/en/babelrc.html)
- [babel-preset-env](https://babeljs.io/docs/en/babel-preset-env)


#### ESLint

```
.eslintrc.js
```

- [Configuring ESLint](https://eslint.org/docs/user-guide/configuring)
- [List of available ESLint rules](https://eslint.org/docs/rules/)


####  PostCSS

```
.postcssrc
```

- [PostCSS](https://postcss.org/)
- [PostCSS on Github](https://github.com/postcss/postcss)


#### CSSNano

```
cssnano.config.js
```

- [cssnano.co](https://cssnano.co/)
- [cssnano on Github](https://github.com/cssnano/cssnano)


####  Browserlist

```
.browserslistrc
```

- [browserslist on NPM](https://www.npmjs.com/package/browserslist)
- [browserslist on Github](https://github.com/browserslist/browserslist)
- Check the browserslist with `npx browserslist` or online with [browserl.ist](http://browserl.ist/)


#### Modernizr

[Optional]

- (1) Modify `.modernizr.json` accordingly and run `npm run modernizr` once.
- (2) Add `class="no-js"` to `<html>` tag in `templates/layouts/master.twig`
- [Modernizr: the feature detection library for HTML5/CSS3](https://modernizr.com/)
- [Modernizr on Github](https://github.com/Modernizr/Modernizr).


## Folder Structure

```
.
├── dist
│   ├── scripts
│   ├── styles
│   └── ...
├── config
│   ├── config.yml
│   ├── contenttypes.yml
│   ├── routing.yml
│   ├── extensions/boltforms.bolt.yml
│   ├── extensions/seo.bobdenotter.yml
│   └── ...
├── source
│   ├── scripts
│   ├── styles
│   └── ...
├── templates
│   ├── components
│   ├── layouts
│   ├── partials
│   └── ...
├── .babelrc
├── .browserslistrc
├── .editorconfig
├── .eslintrc.js
├── .gitignore
├── .modernizr.json
├── .postcssrc
├── browserconfig.yml
├── CHANGELOG.md
├── composer.json
├── cssnano.config.js
├── LICENSE
├── package.json
├── package-lock.json
├── README.md
├── site.webmanifest
├── theme.yml
└── ...
```


## Recommendations, Tips and Tricks


### Extensions

By default, this extension automatically installs the following extensions:

- `bacboslab/menueditor`
- `bobdenotter/seo`
- `bolt/boltforms`
- `bolt/sitemap`
- `twokings/bolt-searchable-content-extension`
- `twokings/hierarchical-routes`

These extensions will be uninstalled if you uninstall this theme. You can install
them separately in order to keep them:

```sh
composer require bacboslab/menueditor
composer require bobdenotter/seo
composer require bolt/boltforms
composer require bolt/sitemap
composer require twokings/bolt-searchable-content-extension
composer require twokings/hierarchical-routes
```


#### Commonly Used Extensions

- `animal/translate`
- `bolt/basewidget`
- `bolt/disqus`
- `bolt/jsonapi`
- `bolt/labels`

```sh
composer require animal/translate
composer require bolt/basewidget
composer require bolt/disqus
composer require bolt/jsonapi
composer require bolt/labels
```


### Bolt Configuration

`[Optional]`

- `config.yml`
- `contenttypes.yml`
    - singletons
    - blocks
    - common elements
- `routing.yml`


### Blocks

TODO


### Snippets

TODO


### Components

TODO

## Fundamentals

TODO

### Grid

TODO

### Color

TODO

### Typography

TODO

### Accessibility

TODO

- [Inclusive Components by Heydon Pickering](https://inclusive-components.design/)


### Web App Manifest

Generate `favicon.ico`, `site.webmanifest`, and `browserconfig.xml` at [Favicon Generator](https://realfavicongenerator.net).

- [The Web App Manifest on Google Web Fundamentals](https://developers.google.com/web/fundamentals/web-app-manifest/)


## References

- TODO
