# Starter, a Bolt Theme

A simple theme with re-usable components.


## Getting Started

[Optional] Install the following recommended extensions:

- `bobdenotter/seo`
- `bolt/boltforms`
- `twokings/hierarchical-routes`
- `twokings/searchable-content`
- `bolt/labels`
- ...


[Optional] Install the following extensions if multilingual website:

- `animal/translate`

### Content Types

[Optional]


### Blocks

[Optional]


## CLI

### Install Dependencies

```sh
npm install
```

### Development

```sh
npm start
```

### Build

```sh
npm run build
```

### Other

| Command                | Description                              | Minification? |
|------------------------|------------------------------------------|---------------|
| `npm run sass`         | Compile SASS to CSS                      | ❌           |
| `npm run postcss`      | PostCSS (polyfill, autoprefixer)         | ❌           |
| `npm run styles`       | Build styles (`sass` + `postcss`)        | ✅           |
| `npm run scripts`      | Compile JS                               | ❌           |
| `npm run build`        | Build everything (`styles` + `scripts`)  | ✅           |


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

## Credits

- foo
- bar
