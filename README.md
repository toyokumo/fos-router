# @toyokumo/fos-router

This is a npm package based on the [js router]((https://github.com/FriendsOfSymfony/FOSJsRoutingBundle/blob/3.2.1/Resources/js/router.ts)) of [FOSJsRoutingBundle](https://github.com/FriendsOfSymfony/FOSJsRoutingBundle).
The purpose is to be able to install the js router of FOSJsRoutingBundle without PHP dependency.

## Usage

0. Generate routes files

Generate routes files in JSON format using the FOSJsRoutingBundle command.

```bash
bin/console fos:js-routing:dump --format json --target generated/routes.js
```

1. Install

```bash
npm i @toyokumo/fos-router
pnpm add @toyokumo/fos-router
yarn add @toyokumo/fos-router
```

2. Import

```javascript
import routes from './generated/routes.json';
import Router from '@toyokumo/fos-router';

Router.setRoutingData(routes);
```

See the [FOSJsRoutingBundle documentation](https://github.com/FriendsOfSymfony/FOSJsRoutingBundle/blob/master/Resources/doc/usage.rst) for details on how to use the bundle after import.
