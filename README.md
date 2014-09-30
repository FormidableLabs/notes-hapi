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

Navigate to: http://127.0.0.1:3000/

And *don't* break the build ;)

We test all changes with [Travis CI][trav]. Here's our current
[build status][trav_site]:

[![Build Status][trav_img]][trav_site]

[trav]: https://travis-ci.org/
[trav_img]: https://travis-ci.org/FormidableLabs/notes-hapi.svg
[trav_site]: https://travis-ci.org/FormidableLabs/notes-hapi

## Production

```
$ npm install --production
$ npm run-script build
```
