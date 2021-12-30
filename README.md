# babel-config-react

A Babel configuration addon for React projects.

## How to Use

First, install this library with `yarn install --dev @craigmiller160/babel-config-react`. If you need to merge this with other configs, also install the `config-mege` library with `yarn install --dev @craigmiller160/config-merge`.

Then, create a `babel.config.js` file in the root of your project.

If only using this config (unlikely), use it with:

```javascript
module.exports = require('@craigmiller160/babel-config-react');
```

If combining it with other configs, whether from libraries or locally, use it with:

```javascript
const babelConfig= require('@craigmiller160/babel-config-react');
const configMerge = require('@craigmiller160/config-merge');

module.exports = configMerge(babelConfig, moreConfig1, moreConfig2);
```
