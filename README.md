This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

### don't forget

Webpack config to be loaded from react-scripts.
e.g.

Loading webpack config from:
../react-app/node_modules/react-scripts/config/webpack.config.js

You need to inject in react-scripts by adding webpackConfig to:<br />
  ...<br />
  plugins: [<br />
    new webpack.ProvidePlugin({<br />
      $: "jquery",<br />
      jQuery: "jquery",<br />
      "window.jQuery": "jquery",<br />
      "window.Tether": 'tether'<br />
    }),<br />
  ...

