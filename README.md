Notes (CommonJS Webpack) Full
=============================

A version of Notes written using CommonJS, built with [Webpack][webpack].

## Sources

The relevant pages for this project are:

* [`app/index.html`](app/index.html): Notes application.
* [`test/jasmine/test.html`](test/jasmine/test.html):
  Jasmine test runner.
* [`test/mocha/test.html`](test/mocha/test.html):
  Mocha test runner.

and available as source in the directory:

```
app/                // Application directory.
  js/               // JS sources (not served in prod)
  js-dist/          // Production bundle
test/
  jasmine/          // Jasmine test directory
  mocha/            // Mocha test directory
```

## Development

```
$ npm install
$ node server/init-db.js
$ gulp dev
```

## Production

```
$ npm install --production
$ npm run-script build
```
