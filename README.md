coverage-percentage
===================

Tiny utility for turning a coverage report in various formats into a numerical percentage.  Built for use with [https://www.github.com/ppvg/node-coverage-badge].

## Example

```json
"scripts": {
  "test": "istanbul test _mocha --report lcov -- -R spec",
  "badge": "coverage-badge `./bin/coverage-percentage ./coverage/lcov.info --lcov` badge.png"
}
```

Then simply:

```
npm test --coverage
npm run-script badge
```
