RingCentral 3-Legged OAuth Demo in JavaScript
=============================================

## Overview

This is a quick 3-legged OAuth demo that runs using client-side JavaScript with the [RingCentral JavaScript SDK](https://github.com/ringcentral/ringcentral-js) v3.x.

## Installation

*Note*, please make sure `bower` is installed.

```bash
$ $ git clone https://github.com/ringcentral-tutorials/oauth-js-demo
$ cd oauth-js-demo
$ bower install ringcentral#~3.x --save
```

## Configuration

Edit the `./public/config.js` file to configure your client ID, client secret and redirect URL, etc.

```bash
$ cd ./public
$ cp config-sample.js config.js
$ vi config.js
```

In the [Developer Portal](http://developer.ringcentral.com/), ensure the redirect URI in your config file has been entered in your app configuration. By default, the URL is set to the following for this demo:

```
http://localhost:8080/oauth2callback.html
```

## Usage

Serve the static page with `http-server`:

```bash
$ npm install -g http-server
$ http-server public
```

You can also serve the static pages with **nginx** or **apache** as you like.

Go to the URL:

```
http://localhost:8080
````

Then click the <input type="button" value="Login with RingCentral"> button to authorize the demo app and view the access token.
