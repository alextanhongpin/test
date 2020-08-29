# test ![Node.js Package](https://github.com/alextanhongpin/test/workflows/Node.js%20Package/badge.svg)

A simple github package under the scoped name `@alextanhongpin/test`.

To use the package, create a `.npmrc` file with this:

```
registry=https://npm.pkg.github.com/alextanhongpin
```

Then install the package:

```
$ npm i @alextanhongpin/test
```

Sample usage:

```js
const { greet } = require('@alextanhongpin/test')
console.log(greet)
```

## Updating and publishing packages

First you need to create the `GITHUB_TOKEN` and then follow the setup [here](https://docs.github.com/en/packages/using-github-packages-with-your-projects-ecosystem/configuring-npm-for-use-with-github-packages).

```bash
$ npm version minor|major|patch
$ npm publish
```

## Automating publishing

Github Action is set to publish the package to both `npm` and `Github Package` (though it fails for `npm` now due to auth error). In order to trigger the Github Action, we need to create a release manually.
