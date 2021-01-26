# vue-svg-example

This is a plain vue.js starter app with the preconfigured support for importing `.svg` files. The demo displays a Vue.js svg logo instead of png image.

## Project setup
 
This example uses `vue-svg-loader` webpack plugin, which you can install to your app with 
```
yarn add --dev vue-svg-loader
```

... once plugin is installed, you just need to create `vue.config.js` (if it doesn't already exist) file with the following contents:
```js
module.exports = {
  chainWebpack: config => {
    config.module.rules.delete("svg");
  },
  configureWebpack: {
    module: {
      rules: [
        {
          test: /\.svg$/,
          loader: ["vue-svg-loader"]
        }
      ]
    }
  }
};

```

Have a look in `src/App.vue` for an example usage.

For more info, please refer to the [official documentation](https://github.com/visualfanatic/vue-svg-loader).
