# vue_firebase_sample

> Sample Project using vue.js and firebase.

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## Settings
```bash:settings
? Project name vue_firebase_sample
? Project description Sample Project using vue.js and firebase.
? Author Masumi.M <masumi.lacrosse@live.jp>
? Vue build standalone
? Install vue-router? Yes
? Use ESLint to lint your code? No
? Set up unit tests No
? Setup e2e tests with Nightwatch? No
? Should we run `npm install` for you after the project has been created? (
recommended) npm
```

## Additional Code
### Firebase
1. `firebase init hosting`
```
? What do you want to use as your public directory? dist
? Configure as a single-page app (rewrite all urls to /index.html)? No
✔  Wrote dist/404.html
? File dist/index.html already exists. Overwrite? No
i  Skipping write of dist/index.html

i  Writing configuration info to firebase.json...
i  Writing project information to .firebaserc...

✔  Firebase initialization complete!
```

2. `firebase use --add`
```
? Which project do you want to add? vue-firebase-sample-d98cb
? What alias do you want to use for this project? (e.g. staging) staging

Created alias staging for vue-firebase-sample-d98cb.
Now using alias staging (vue-firebase-sample-d98cb)
```

## Sass
1. `npm install --save node-sass sass-loader axios`
2. Change the css file
```
<style scoped lang="scss">
    // CSS script here.
</style>
```

## Semantic-ui
1. `npm install semantic-ui-vue --save`
2. `npm install semantic-ui-css --save`
3. Add the next code in `src/main.js`.
```js:main.js
// The Vue build version to load with the `import` command
// (runtime-only or standalone) has been set in webpack.base.conf with an alias.
import Vue from 'vue'
import App from './App'
import router from './router'
import SuiVue from 'semantic-ui-vue';
import 'semantic-ui-css/semantic.min.css';

Vue.config.productionTip = false

/* eslint-disable no-new */
new Vue({
  el: '#app',
  router,
  components: {
    App
  },
  template: '<App/>'
})

Vue.use(SuiVue);
```

## Delete \#
1. Add `mode: 'history'` in `src/router/index.js`.
```
export default new Router({
  mode: 'history',
  routes: [{
    path: '/',
    name: 'HelloWorld',
    component: HelloWorld
  }]
})
```

## Bug
If your page doesn't update, check the `firebase.json`.
```
{
  "hosting": {
    "public": "dist",
    "ignore": [
      "firebase.json",
      "**/.*",
      "**/node_modules/**"
    ],
    "rewrites": [{
      "source": "**",
      "destination": "/index.html"
    }]
  }
}
```

