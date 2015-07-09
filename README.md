# my .eslintrc (ES5 related)

A fork of [the AirBnB JavaScript style guide](https://github.com/airbnb/javascript/blob/master/linters/.eslintrc) rules for [eslint](https://github.com/eslint/eslint), with the following changes:

- removed ES6 / babel / react stuff
- vars can be declared everywhere, not only at the top
- strict mode set to global (because Node && browserify => every module is wrapped into its own closure so it's ok; also I prefer not to use plugins that automatically add that)
- disabled `new-cap` since a lot of contructors use the `instanceof` check trick

## license

[MIT](http://alessioalex.mit-license.org/)
