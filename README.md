# Expo env file error

Steps to reproduce

1. npm ci

2. Run expo normally and load the app onto your phone.

```
npx expo start -c
```

3. Run expo under a test environment and load the app onto your phone.

```
NODE_ENV=test npx expo start -c 
```

Then note the error

```sh
iOS Bundling failed 5165ms node_modules/expo-router/entry.js (1004 modules)
 ERROR  node_modules/expo-router/_ctx.ios.js: node_modules/expo-router/_ctx.ios.js:Invalid call at line 2: process.env.EXPO_ROUTER_APP_ROOT
First argument of `require.context` should be a string denoting the directory to require.
```
