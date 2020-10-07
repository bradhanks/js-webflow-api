# Webflow CMS API Client

## Requirements

* Node.js 4+
* NPM / YARN
* Webpack / Browserify (optional)

## Installation

Install the package via NPM or YARN:

```shell
$ npm install --save webflow-api

$ yarn add webflow-api
```

## Usage

```javascript
const Webflow = require('webflow-api');

// Initialize the API
const api = new Webflow({ token: 'api-token' });

// Fetch a site
async () => {
  console.log(await api.site({ siteId: "58e32bace1998d6e3fee8d71" }));
};
```

The `Webflow` constructor takes several options to initialize the API client:

* `token` - the API token **(required)**
* `version` - the version of the API you wish to use (optional)

All of the API methods are documented in the [API documentation](https://developers.webflow.com).

## Contributing

Contributions are welcome - feel free to open an issue or pull request.

## License

The MIT license - see `LICENSE`.
