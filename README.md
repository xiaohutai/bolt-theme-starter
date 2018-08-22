# Starter, a Bolt Theme ![work in progress](https://img.shields.io/badge/-work--in--progress-yellow.svg?longCache=true&style=flat-square)

<p align="center">
    <a href="#installation">Installation</a>
  | <a href="#getting-started">Getting Started</a>
  | <a href="#configuration">Configuration</a>
  | <a href="#folder-structure">Folder Structure</a>
  | <a href="#recommendations">Recommendations</a>
  | <a href="#fundamentals">Fundamentals</a>
  | <a href="#references">References</a>
</p>

---

## Installation

There are two options to get this theme:

- Install this theme via the Bolt backend at `/bolt/extensions`.
- Do a `composer require xiaohutai/bolt-theme-starter` in your Bolt's `extensions` folder.

For making pull requests, navigate to your Bolt's `themes` folder and clone this repo:

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
|:-----------------------|:-----------------------------------------|:-------------:|
| `npm run sass`         | Compile SASS to CSS                      | ![no](https://img.shields.io/badge/-no-red.svg?longCache=true&style=flat-square)   |
| `npm run postcss`      | PostCSS (polyfill, autoprefixer)         | ![yes](https://img.shields.io/badge/-yes-brightgreen.svg?longCache=true&style=flat-square) |
| `npm run styles`       | Build styles (`sass` + `postcss`)        | ![yes](https://img.shields.io/badge/-yes-brightgreen.svg?longCache=true&style=flat-square) |
| `npm run scripts`      | Compile JS                               | ![no](https://img.shields.io/badge/-no-red.svg?longCache=true&style=flat-square)   |
| `npm run build`        | Build everything (`styles` + `scripts`)  | ![yes](https://img.shields.io/badge/-yes-brightgreen.svg?longCache=true&style=flat-square) |
| `npm run lint`         | Lint styles                              | ![n/a](https://img.shields.io/badge/-n/a-lightgrey.svg?longCache=true&style=flat-square) |
| `npm run eslint`       | Lint scripts                             | ![n/a](https://img.shields.io/badge/-n/a-lightgrey.svg?longCache=true&style=flat-square) |


## Configuration

| Name                                                        | File                | Github | More info |
|:------------------------------------------------------------|:--------------------|:------:|:----------|
| [Babel](https://babeljs.io)                                 | `.babelrc`          | [:octocat:](https://github.com/babel/babel) | [.babelrc](https://babeljs.io/docs/en/babelrc.html), [babel-preset-env](https://babeljs.io/docs/en/babel-preset-env) |
| [ESLint](https://eslint.org)                                | `.eslintrc.js`      | [:octocat:](https://github.com/eslint/eslint) | [Configuring](https://eslint.org/docs/user-guide/configuring), [ESLint rules](https://eslint.org/docs/rules/) |
| [PostCSS](https://postcss.org/)                             | `.postcssrc`        | [:octocat:](https://github.com/postcss/postcss) | |
| [cssnano](https://cssnano.co/)                              | `cssnano.config.js` | [:octocat:](https://github.com/cssnano/cssnano) | |
| [Browserlist](https://github.com/browserslist/browserslist) | `.browserslistrc`   | [:octocat:](https://github.com/browserslist/browserslist) | [browserl.ist](http://browserl.ist/) |

Check the browserslist with
```
npx browserslist
```


## Folder Structure

<details>
    <summary>Folder structure</summary>
<pre>
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
</pre>
</details>


## Recommendations


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


#### Suggested Extensions ![optional](https://img.shields.io/badge/-optional-brightgreen.svg?longCache=true&style=flat-square)

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


### Bolt Configuration ![optional](https://img.shields.io/badge/-optional-brightgreen.svg?longCache=true&style=flat-square)

The `config` directory has some `yml` files with useful blocks that you can copy
and paste.

- `config.yml`
- `contenttypes.yml`
- `routing.yml`


### Blocks ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)
### Snippets ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)
### Components ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)

## Fundamentals
### Grid ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)
### Color ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)
### Typography ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)
### Accessibility ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)

- [Inclusive Components by Heydon Pickering](https://inclusive-components.design/)


### Web App Manifest

Generate `favicon.ico`, `site.webmanifest`, and `browserconfig.xml` at [Favicon Generator](https://realfavicongenerator.net).

- [The Web App Manifest on Google Web Fundamentals](https://developers.google.com/web/fundamentals/web-app-manifest/)


## References ![todo](https://img.shields.io/badge/-todo-red.svg?longCache=true&style=flat-square)
