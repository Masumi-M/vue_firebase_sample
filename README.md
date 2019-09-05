# vue_firebase_sample
Sample Project using vue.js and firebase.
Hosting Site: https://vue-firebase-sample-d98cb.firebaseapp.com/

## Build Setup

```bash
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
```bash
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
```bash
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
```bash
? Which project do you want to add? vue-firebase-sample-d98cb
? What alias do you want to use for this project? (e.g. staging) staging

Created alias staging for vue-firebase-sample-d98cb.
Now using alias staging (vue-firebase-sample-d98cb)
```

## Sass
1. `npm install --save node-sass sass-loader axios`
2. Change the css file
```html
<style scoped lang="scss">
    // CSS script here.
</style>
```

## Delete \#
1. Add `mode: 'history'` in `src/router/index.js`.
```js
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
```json
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

