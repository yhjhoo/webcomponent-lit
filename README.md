## modern web component test


to setup from scracth
```shell
npm init @open-wc

npm i -D rollup @open-wc/building-rollup rimraf deepmerge es-dev-server

npm install rollup-plugin-copy -D
```

copy rollup.config.js to local and 

"build": "rimraf dist && rollup -c rollup.config.js",
"start:build": "npm run build && es-dev-server --root-dir dist --app-index index.html --compatibility none --open"

to package.json

## Open-wc Starter App

[![Built with open-wc recommendations](https://img.shields.io/badge/built%20with-open--wc-blue.svg)](https://github.com/open-wc)


## Scripts

- `start` runs your app for development, reloading on file changes
- `start:build` runs your app after it has been built using the build command
- `build` builds your app and outputs it in your `dist` directory
- `test` runs your test suite with Web Test Runner
- `lint` runs the linter for your project
- `format` fixes linting and formatting errors

## Tooling configs

For most of the tools, the configuration is in the `package.json` to reduce the amount of files in your project.

If you customize the configuration a lot, you can consider moving them to individual files.
