# test

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
