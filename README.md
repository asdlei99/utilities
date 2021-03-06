[![Build Status](https://travis-ci.org/webrtc/utilities.svg?branch=master)](https://travis-ci.org/webrtc/utilities)
# WebRTC utilities #
Contains shared utilities, support tools and frameworks for the other WebRTC sub repositories.

## Install using npm ##
```
npm install webrtc-utilities --save-dev
```

## SeleniumLib ##
src/selenium/selenium-lib.js contains all that is needed to build a selenium webdriver driver for Chrome and Firefox (whatever is set in the BROWSER and BVER variables).

### node and commonjs ###
`require('webrtc-utilities').seleniumLib`

## start-tests.sh ##
src/testrunner/start-tests.sh that helps travis-multirunner to download and install Chrome and Firefox browser from stable, beta and unstable channels. Also starts the tests using node.

This will be added to node_modules/.bin and can be called on in package.json file, e.g.
```
"scripts": {
    "test": "start-tests"
},
```

## Development ##
Add new utilities under the src folder and add them to the main.js file in the project root with the appropriate module.export set.

Detailed information on developing in the [webrtc](https://github.com/webrtc) github repositories can be found in the [WebRTC GitHub repo developer's guide](https://docs.google.com/document/d/1tn1t6LW2ffzGuYTK3366w1fhTkkzsSvHsBnOHoDfRzY/edit?pli=1#heading=h.e3366rrgmkdk).
