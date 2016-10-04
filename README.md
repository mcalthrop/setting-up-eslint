# setting-up-eslint

Here are some basic instructions for setting up `eslint` for for a project that uses `ES5` and `ES6`.

## `npm` packages

Inspect the `package.json` file in this project, and make sure that all the `devDependencies` it contains are also in your `package.json` file.

Then run `npm install` to retrieve the required `npm` packages.


## Configuration

### Check the linting rules

This project includes a sample `.eslintrc` file.

To keep things simple, it uses `airbnb` rules as a base, and adds several rule modifications.

So you might like to check the `"rules"` section of `.eslintrc` to see if they match your requirements.

### Specify files to lint

The `package.json` file in this project contains a very simple `"eslint"` script to run &ndash; it simply calls the `eslint` binary, with a single argument, which is the filespec for the JS files to lint. Modify this filespec to match the files you want to lint.
