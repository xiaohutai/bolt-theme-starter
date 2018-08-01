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


## Development

Install dependencies
```
npm install
```

Serve with hot reload at localhost
```
npm start
```
or
```
npm run dev
```

Build for production
```
npm run build
```
or
```
npm run prod
```

## Folder Structure

```
.
├── dist
│   └── ...
├── config
│   └── ...
├── source
│   ├── scripts
│   └── styles
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

## Notes

For a Bolt theme, use:

```
parcel build source/index.js
```

For a web app, use:

```
parcel build source/index.html --public-url ./ --detailed-report
```

This will automatically add hashes to included assets which is not needed for a Bolt theme.
