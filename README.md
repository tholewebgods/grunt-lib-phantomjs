# rzg-grunt-lib-phantomjs

Fork of the official [grunt-lib-phantomjs](https://github.com/tholewebgods/grunt-lib-phantomjs/tree/v0.7.1) package that does not use the [phantomjs npm](https://github.com/Medium/phantomjs) but expects an environment variable `PHANTOMJS_BIN` to be defined pointing to a PhantomJS binary.

## Difference

- Based on 0.7.1, comming 0.7.2 of grunt-lib-phantomjs
- The binary path is read from the environment variable `PHANTOMJS_BIN`
- If not defined, the path points to the *NIX standard path `/usr/bin/phantomjs`

## Usage

```
$ export PHANTOMJS_BIN="/opt/phantomjs-2.0.0/bin/phantomjs"
$ grunt whatever-uses-this-library-in-the-end
```
