#reactbp
minimalistic (really) starting point for full stack react apps

- webpack production and development configurations
- react-hot-loader 3 beta
- express
- normalize.css (extracted to vendor.css)
- polyfills via core-js

## npm scripts
`dev:server` develop server

`dev:client` develop client (no hot module replacement)

`dev:client:hot` develop client (hot module replacement)

`dev:hot` develop server and client (client hot module replacement)

`build:client` build bundle (output to dist folder)

## config
create `.env` file and set PORT for server port

## TODO
set up testing via karma, enzyme
