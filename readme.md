# ee-gitpage

Publish files to a git repo branch(based on gh-pages).

## Getting Started

```shell
npm install ee-gitpage --save-dev
```

This module requires Git `>=1.7.6`.

## Basic Usage

```js
var ghpages = require('ee-gitpage');
var path = require('path');

ghpages.publish(path.join(__dirname, 'dist'), function(err) { ... });
```

## Dependencies
Note that this plugin requires Git 1.7.6 or higher (because it uses the `--exit-code` option for `git ls-remote`). 