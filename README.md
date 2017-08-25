[![Build Status](https://travis-ci.org/symphonyoss/extension-api-examples.svg)](https://travis-ci.org/symphonyoss/extension-api-examples)
[![Dependencies](https://www.versioneye.com/user/projects/578010725bb1390040177cb0/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/578010725bb1390040177cb0#tab-dependencies)

# Extension API Example


This repo contains examples of the Symphony Extension API. This API allows you to write applications
which users can install. Additionally, with the extension API you can add buttons throughout the UI,
and in turn your application can listen and react to click events on those buttons.


## Prerequisites


* Have `node` and `npm` installed.
* Have port 4000 available as we'll run the demo application on this port.
* If you are planning to use Chrome to run the Hello World app, you will need to first enable the #allow-insecure-localhost flag in Chrome. To do this, go to chrome://flags and enable the setting called "Allow invalid certificates for resources loaded from localhost". 

## Run the example project


* Clone this repo and `cd` into the directory
* Run `npm i webpack -g`
* Run `npm i webpack-dev-server -g`
	* If you have trouble running the webpack-dev-server over HTTPS, check out the --https option described here: https://webpack.github.io/docs/webpack-dev-server.html
* Run `npm i`
* Run `npm run watch`
* Ensure the sample app is running by visiting https://localhost:4000/app.html
* Append "bundle=https://localhost:4000/bundle.json" as a URL param to your pods Symphony address
    * For example https://corporate.symphony.com/client/index.html?bundle=https://localhost:4000/bundle.json
* Accept the "Warning: Unauthorized App(s)" dialog
* Click on the "Applications > App Store" entry in your left nav to install the Hello World app

## Now what?

You've successfully installed the Hello World application. You'll notice a new entry on the left nav
titled "Hello." Click on this to open the app in the Symphony grid. Explore the source code in
`src/javascript` to understand how the application works.

