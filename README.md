#reactbp
minimalistic (really) starting point for full stack react apps

- webpack production and development configurations
- react-hot-loader 3 beta
- nodemon for server restarts
- eslint with airbnb styleguide
- dotenv for environment variables
- express
- normalize.css (extracted to vendor.css)
- polyfills via core-js

## npm scripts
`dev:server` develop server

`dev:client` develop client (no hot module replacement)

`dev:client:hot` develop client (hot module replacement)

`dev:hot` develop server and client (client hot module replacement)

`build` build client production bundle (output to dist folder)

`test:client` run client tests via karma mocha kai
`test:client:watch` run client tests and watch for changes to run again
`test:client:sanity` run client sanity tests (make sure things are working)

## config
create `.env` file and set variables

`PORT` express app. defaults to 3030

`WEBPACK_HOST` webpack-dev-server. defaults to localhost

`WEBPACK_PORT` webpack-dev-server. defaults to 8080

## TODO

- finish npm test scripts (tdd, tdd:hot, etc)
- set up server side testing
- decide where to initialize dotenv for server, etc
