![Seneca](http://senecajs.org/files/assets/seneca-logo.png)
> A [Seneca.js](http://senecajs.org) plugin

# @seneca/entity-transaction

[![build](https://github.com/senecajs/seneca-entity-transaction/actions/workflows/build.yml/badge.svg)](https://github.com/senecajs/seneca-entity-transaction/actions/workflows/build.yml)
[![Known Vulnerabilities](https://snyk.io/test/github/senecajs/seneca-entity-transaction/badge.svg)](https://snyk.io/test/github/senecajs/seneca-entity-transaction)

| ![Voxgig](https://www.voxgig.com/res/img/vgt01r.png) | This open source module is sponsored and supported by [Voxgig](https://www.voxgig.com). |
|---|---|

## Install

```sh
npm install @seneca/entity-transaction
```

## Quick Example

```js
require('seneca')()
  .use('@seneca/entity-transaction')
```

## More Examples

See [test/](test/) for more usage examples.

## Motivation

A [Seneca.js](http://senecajs.org) plugin providing entity transaction support.

## Support

If you're using this module and need help, you can:

- Post a [github issue](https://github.com/senecajs/seneca-entity-transaction/issues)
- Tweet to [@senecajs](http://twitter.com/senecajs)
- Ask on the [Gitter](https://gitter.im/senecajs/seneca)

## API

See [source](https://github.com/senecajs/seneca-entity-transaction) for API details.

## Contributing

The [Senecajs org](https://github.com/senecajs/) encourages open participation. If you feel you can help in any way, be it with documentation, examples, extra testing, or new features please get in touch.

### Running tests

To run the tests:
```
# Build the services required by the automated tests.
docker-compose -f docker-compose.test.yaml build

# Run the services required by the automated tests.
docker-compose -f docker-compose.test.yaml up -d

# Run the tests.
npm run test
```

To sign in to the mysql test instance, e.g. to inspect the test db state:
```
docker-compose -f docker-compose.test.yaml exec mysql_test bash

# Once you are inside the container:
mysql -pmysql

# Once you are in the MySQL shell:
USE senecatest;
```

To sign in to the postgres test instance:
```
docker-compose -f docker-compose.test.yaml exec postgres_test bash

# Once you are inside the container:
psql -U postgres

# Once you are in the postgres shell:
\c senecatest
```

When you are done, stop the containers:
```
docker-compose -f docker-compose.test.yaml down
```



## Background

Part of the [Senecajs org](https://github.com/senecajs/).
