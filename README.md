# @nuxtjs/partytown

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![Github Actions CI][github-actions-ci-src]][github-actions-ci-href]
[![Codecov][codecov-src]][codecov-href]
[![License][license-src]][license-href]

> [Partytown](https://github.com/BuilderIO/partytown/wiki) integration for [Nuxt](https://v3.nuxtjs.org)

## Features

- 👌 Zero-config required
- 🔥 Relocates resource intensive scripts into a web worker
- ⚡️ Speeds up your site
- 💯 Nuxt 3 and Nuxt Bridge support

## Quick setup

1. Add `@nuxtjs/partytown` dependency to your project

```bash
yarn add @nuxtjs/partytown # or npm install @nuxtjs/partytown
```

2. Add `@nuxtjs/partytown` to the `modules` section of `nuxt.config.js`

3. Add `type: 'text/partytown'` attribute to any scripts you want to be handled by partytown.

```js
import { defineNuxtConfig } from 'nuxt3'
export default defineNuxtConfig({
  meta: {
    script: [{ src: '/test-script.js', type: 'text/partytown' }],
  },
  modules: ['@nuxtjs/partytown'],
  partytown: {
    // module options
  },
})
```

## Development

- Run `yarn prepare` to generate type stubs.
- Use `yarn dev` to start [playground](./playground) in development mode.

## Licence

[MIT Licence](./LICENCE)

<!-- Badges -->

[npm-version-src]: https://img.shields.io/npm/v/@nuxtjs/partytown/latest.svg
[npm-version-href]: https://npmjs.com/package/@nuxtjs/partytown
[npm-downloads-src]: https://img.shields.io/npm/dm/@nuxtjs/partytown.svg
[npm-downloads-href]: https://npmjs.com/package/@nuxtjs/partytown
[github-actions-ci-src]: https://github.com/nuxt-community/partytown-module/workflows/ci/badge.svg
[github-actions-ci-href]: https://github.com/nuxt-community/partytown-module/actions?query=workflow%3Aci
[codecov-src]: https://img.shields.io/codecov/c/github/nuxt-community/partytown-module.svg
[codecov-href]: https://codecov.io/gh/nuxt-community/partytown-module
[license-src]: https://img.shields.io/npm/l/@nuxtjs/partytown.svg
[license-href]: https://npmjs.com/package/@nuxtjs/partytown