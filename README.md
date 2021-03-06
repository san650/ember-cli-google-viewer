# ember-cli-google-viewer

[![Latest NPM release][npm-badge]][npm-badge-url]
[![TravisCI Build Status][travis-badge]][travis-badge-url]
[![Ember Observer Score][ember-observer-badge]][ember-observer-badge-url]
[![License][license-badge]][license-badge-url]
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)


[npm-badge]: https://img.shields.io/npm/v/ember-cli-google-viewer.svg
[npm-badge-url]: https://www.npmjs.com/package/ember-cli-google-viewer
[travis-badge]: https://img.shields.io/travis/ntgussoni/ember-cli-google-viewer/master.svg?label=TravisCI
[travis-badge-url]: https://travis-ci.org/ntgussoni/ember-cli-google-viewer
[ember-observer-badge]: http://emberobserver.com/badges/ember-cli-google-viewer.svg
[ember-observer-badge-url]: http://emberobserver.com/addons/ember-cli-google-viewer
[license-badge]: https://img.shields.io/npm/l/ember-cli-google-viewer.svg
[license-badge-url]: LICENSE.md

An ember-cli addon to view documents using the google viewer.

[![Sample project][sample-project]][sample-project]

[sample-project]: sample.gif

## Installation

```
ember install ember-cli-google-viewer
```

## Usage
The usage is simple, you pass the URL of the file and you are good to go.

```html
  {{ember-cli-google-viewer
    url="http://path-to-your-file/"
  }}
```

If you wish, you can yield a loader that will be shown until the viewer finishes loading.

```html
  {{#ember-cli-google-viewer
    url="http://path-to-your-file/"
  }}
    Loading...
  {{/ember-cli-google-viewer}}
```

Additionally, you can call an action after the viewer loads

```html
  {{#ember-cli-google-viewer
    url="http://path-to-your-file/"
    onViewerLoad=(action "myAction")
  }}
    Loading...
  {{/ember-cli-google-viewer}}
```
