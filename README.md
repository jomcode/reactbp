#reactbp

[![Build Status](https://travis-ci.org/jomcode/reactbp.svg?branch=master)](https://travis-ci.org/jomcode/reactbp)
[![Test Coverage](https://codeclimate.com/github/jomcode/reactbp/badges/coverage.svg)](https://codeclimate.com/github/jomcode/reactbp/coverage)

starting point for full stack react apps.

**client**
- webpack development, production, and test configurations
- react-hot-loader 3 beta
- eslint with airbnb styleguide
- tests via karma, mocha, chai, sinon, enzyme
- code coverage via istanbul, babel-plugin-istanbul, karma-coverage
- normalize.css (extracted to vendor.css)
- polyfills via core-js

**server**
- nodemon for server restarts
- express
- dotenv for environment variables
- tests via mocha, chai, sinon, supertest

## npm scripts
**development**

`dev:server` develop server (nodemon restarts)

`dev:client` develop client (no hot module replacement)

`dev:client:hot` develop client (hot module replacement)

`dev:hot` develop server (nodemon restarts) and client (hot module replacement)

**production**

`build` build client production bundle (output to dist folder)

`start` runs server

**tests**

`test:client` run client tests via karma and generates coverage report

`test:client:watch` run client tests and watch for changes to run again

`test:client:sanity` run client sanity tests (make sure things are working)

`test:server` run server tests via mocha

`test:server:watch` run server tests and watch for changes to run again

`test:server:sanity` run server sanity tests (make sure things are working)

`tdd:client` runs `dev:client` & `test:client:watch` concurrently

`tdd:client:hot` runs `dev:client:hot` & `test:client:watch` concurrently

`tdd:server` runs `dev:server` & `test:server:watch` concurrently

**coverage reports**

`test:client`, `coverage:server` generate client & server reports

`coverage:combine` combine reports

`codeclimate` set CODECLIMATE_REPO_TOKEN env variable then run

## config
create `.env` file and set variables

`PORT` express app. defaults to 3030

`WEBPACK_HOST` webpack-dev-server. defaults to localhost

`WEBPACK_PORT` webpack-dev-server. defaults to 8080

`HMR` enabled | undefined, hot module replacement via webpack

`SANITY` enabled | undefined, run sanity tests

`NODE_ENV` production | development | test

## TODO
- minify css included in client/vendor.js entrypoint (look at extracttext in prod config)
- decide where to initialize dotenv for server, etc
- eslint env and globals
- env variable to have karma output coverage or not
