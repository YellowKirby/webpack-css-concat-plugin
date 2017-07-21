# webpack-css-concat-plugin
A webpack plugin to concat all css files in your bundle (and any dependent ones)

## Usage

```javascript
# webpack.config.js
const CssConcatPlugin = require('webpack-css-concat-plugin');

module.exports = {
    // The rest of your webpack config

    plugins: [
        new CssConcatPlugin({

            // The filename for the emitted CSS file
            filename: String?,

            // Any additional modules to include in the CSS file.
            modules: [ String ] ?
        })
    ]
}
```

## TODO

- [ ] Dynamically determine the styles/modules to include based on the dependency tree.