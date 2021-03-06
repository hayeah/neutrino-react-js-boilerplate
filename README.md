
Clone repo:

```
git clone https://github.com/hayeah/neutrino-react-js-boilerplate.git my-project
```

Install dependencies:

```
yarn
```

Start Neutrino dev server on port 3000:

```
PORT=3000 yarn start
```

Open http://localhost:3000, and edit `src/index.js` for live-reload.

For styling, edit `src/index.css`.

Edit the [html](https://github.com/hayeah/neutrino-react-ts-boilerplate/blob/727d23b260935edd7a3b2c56d8e05ef616cec31c/.neutrinorc.js#L10) options to customize the HTML template. See [html-webpack-template](https://github.com/jaketrent/html-webpack-template/tree/624dd3931cc2ffaeed03962b25c61af81c2997e2#basic-usage).

# JS Constants

You may need to configure different constants depending on which build environment you are using.

You can add or override JavaScript global constants by modifying the files in the [config](https://github.com/hayeah/neutrino-react-ts-boilerplate/tree/master/config) directory.

See [config npm module](https://www.npmjs.com/package/config) for details.

# Other Tips

Generating sourcemap may slow down project rebuilding. Webpack provide other sourcemap types that can speed up project building.

In particular, the `eval` sourcemap is quite faster.

```
SOURCEMAP=eval PORT=3000 yarn start
```

See [devtool](https://webpack.js.org/configuration/devtool/#devtool`) for a list of sourcemap types.
