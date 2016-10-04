# setting-up-eslint

Here are some basic instructions for setting up [`eslint`](https://github.com/eslint/eslint) for for a project that uses `ES5` and `ES6`.

The assumption is that you already have your own project, with its own `package.json` file.

## Install `npm` packages

Inspect the `package.json` file in this project, and copy all the `devDependencies` it contains into your own `package.json` file.

Then run `npm install` to retrieve the required `npm` packages.

## Check the linting rules

This project includes a sample `.eslintrc` file.

To keep things simple, it uses `airbnb` rules as a base, and adds several rule modifications.

So you might like to check the `"rules"` section of `.eslintrc` to see if they match your requirements.

## Specify files to lint

The `package.json` file in this project contains a very simple `"eslint"` script to run &ndash; it simply calls the `eslint` binary, with a single argument, which is the filespec for the JS files to lint.

Add this to the `"scripts"` section of your `package.json` file, and modify this filespec to match the files you want to lint.

## Lint away

Now you can run `eslint` against your files:

``` sh
$ npm run eslint
```
