# Vue Performance Devtool

Vue Performance Devtool is a browser extension for inspecting the performance of Vue Components. It statistically examines the performance of Vue components based on the measures which are collected by Vue using `window.performance` API.

<p align="center"><img src="https://raw.githubusercontent.com/vue-perf-devtool/vue-perf-devtool/master/media/logo.png" alt="logo"></p>

Initially started after reading [React Performance Devtool](https://github.com/nitin42/react-perf-devtool#using-the-browser-extension) and created from [Vue Devtool](https://github.com/vuejs/vue-devtools).

## Installation

The below extensions represent the current stable release.

- [Chrome extension](https://chrome.google.com/webstore/detail/vue-performance-devtool/koljilikekcjfeecjefimopfffhkjbne)
- [Firefox extension](https://addons.mozilla.org/en-US/firefox/addon/vue-performance-devtool/)

## Implementation

To use this performance devtool extension, you'll need to allow [vue-devtools inspection](https://vuejs.org/v2/api/#devtools) and [performance](https://vuejs.org/v2/api/#performance)

```js
// make sure to set this synchronously immediately after loading Vue
Vue.config.devtools = true
Vue.config.performance = true
```

## Uses

- Remove or unmount the component instances which are not being used.
- Inspect what is blocking or taking more time after an operation has been started.
- Examine which components are taking more time to load.

## Description

<p align="center"><img width="600px" src="https://raw.githubusercontent.com/vue-perf-devtool/vue-perf-devtool/master/media/background2.png" alt="demo"></p>

- **Init:** Time taken in "beforeCreated" and "created" of lifecycle.
- **Render:** Time taken to create the instance in javascript.
- **Patch:** Time taken to render in dom.

## Acknowledgments
Special thanks to [Evan You](https://github.com/yyx990803) and [vue-devtool contributors](https://github.com/vuejs/vue-devtools/graphs/contributors)

### License

[MIT](http://opensource.org/licenses/MIT)
