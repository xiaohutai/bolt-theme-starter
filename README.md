# Starter, a Bolt Theme

A simple theme with re-usable components.

Install this theme via Bolt, or `git clone` this repository into your Bolt's
`themes` folder.

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


## Folder Structure

```
.
├── dist
│   ├── scripts
│   ├── styles
│   └── ...
├── config
│   ├── contenttypes.yml
│   └── ...
├── source
│   ├── scripts
│   ├── styles
│   └── ...
├── templates
│   ├── components
│   ├── layouts
│   └── ...
├── .babelrc
├── .editorconfig
├── .eslintrc.js
├── .eslintignore
├── .gitignore
├── .postcssrc.js
├── package.json
├── package-lock.json
├── README.md
└── ...
```


## Recommendations, Tips and Tricks


### Extensions

`[Optional]` Install the following recommended extensions:

- `animal/translate`
- `bacboslab/menueditor`
- `bobdenotter/seo`
- `bolt/basewidget`
- `bolt/boltforms`
- `bolt/labels`
- `twokings/hierarchical-routes`
- `twokings/bolt-searchable-content-extension`


### Configuration

`[Optional]`

- `config.yml`
- `contenttypes.yml`
    - singletons
- `routing.yml`


### Blocks

TODO


### Snippets

TODO


### Components

TODO
