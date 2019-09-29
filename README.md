# @pushrocks/smartserve
easy serving of static files

## Availabililty and Links
* [npmjs.org (npm package)](https://www.npmjs.com/package/@pushrocks/smartserve)
* [gitlab.com (source)](https://gitlab.com/pushrocks/smartserve)
* [github.com (source mirror)](https://github.com/pushrocks/smartserve)
* [docs (typedoc)](https://pushrocks.gitlab.io/smartserve/)

## Status for master
[![build status](https://gitlab.com/pushrocks/smartserve/badges/master/build.svg)](https://gitlab.com/pushrocks/smartserve/commits/master)
[![coverage report](https://gitlab.com/pushrocks/smartserve/badges/master/coverage.svg)](https://gitlab.com/pushrocks/smartserve/commits/master)
[![npm downloads per month](https://img.shields.io/npm/dm/@pushrocks/smartserve.svg)](https://www.npmjs.com/package/@pushrocks/smartserve)
[![Known Vulnerabilities](https://snyk.io/test/npm/@pushrocks/smartserve/badge.svg)](https://snyk.io/test/npm/@pushrocks/smartserve)
[![TypeScript](https://img.shields.io/badge/TypeScript->=%203.x-blue.svg)](https://nodejs.org/dist/latest-v10.x/docs/api/)
[![node](https://img.shields.io/badge/node->=%2010.x.x-blue.svg)](https://nodejs.org/dist/latest-v10.x/docs/api/)
[![JavaScript Style Guide](https://img.shields.io/badge/code%20style-prettier-ff69b4.svg)](https://prettier.io/)

## Usage

Use TypeScript for best in class instellisense.

```javascript
import { SmartServe } from '@pushrocks/smartserve';

let mySmartserve = new SmartServe('/some/path/to/webroot', 8080);
mySmartserve.start().then(() => {
  // this is executed when server is running guaranteed
  mySmartserve.stop(); // .stop() will work even if not waiting for server to be fully started
});

mySmartserve.reload(); // reloads all connected browsers of this instance
```

For further information read the linked docs at the top of this readme.

> MIT licensed | **&copy;** [Lossless GmbH](https://lossless.gmbh)
| By using this npm module you agree to our [privacy policy](https://lossless.gmbH/privacy)

[![repo-footer](https://lossless.gitlab.io/publicrelations/repofooter.svg)](https://maintainedby.lossless.com)
