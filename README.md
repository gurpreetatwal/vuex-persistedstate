# vuex-persistedstate

Persist [Vuex](http://vuex.vuejs.org/) state with [localStorage](https://developer.mozilla.org/nl/docs/Web/API/Window/localStorage).

[![NPM version](https://img.shields.io/npm/v/vuex-persistedstate.svg?style=flat-square)](https://www.npmjs.com/package/vuex-persistedstate)
[![Build Status](https://img.shields.io/travis/robinvdvleuten/vuex-persistedstate.svg?style=flat-square)](https://travis-ci.org/robinvdvleuten/vuex-persistedstate)

### Installation

```bash
$ npm install vuex-persistedstate
```

### Usage

```js
import createPersistedState from 'vuex-persistedstate'

const store = new Vuex.Store({
  // ...
  plugins: [createPersistedState()]
})
```

### API

#### `createPersistedState([options])`

Creates a new instance of the plugin with the given options. The following options
can be provided to configure the plugin for your specific needs:

- `key <String>`: The key to store the persisted state under. (default: __vuex__)
- `paths <Array>`: An array of any paths to partially persist the state. If no paths are given, the complete state is persisted. (default: __[]__)

### License

[MIT](http://opensource.org/licenses/MIT)
