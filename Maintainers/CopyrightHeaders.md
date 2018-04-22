# Copyright Headers and Licenses

Some open source licenses require copyright headers. Some organizations require copyright headers. In any case, the way the copyright headers are worded can have unexpected consequences.

## An anecdote about copyright headers

[React Native Windows](https://github.com/Microsoft/react-native-windows) is an open source platform plugin that allows you to build Universal Windows apps with [React Native](https://github.com/facebook/react-native), a hybrid app framework that renders [React.js](https://github.com/facebook/react) components using native UI instead of HTML.

Part of the extensibility model for React Native is a bundler called [Metro](https://github.com/facebook/metro), which allows you to override core modules in the React Native core library using a `@providesModule` attribute and a global module namespace.

There are a number of JavaScript modules overridden in React Native Windows, and the typical process is to copy the module from React Native, modify the source code, and commit to the React Native Windows repo. Copying source code in open source is typically not a problem, presuming you provide the correct attribution.

In the case of React Native, the project was using a BSD license that required us to keep the copyright headers of the original source code intact when copying it over. These copyright headers included the following verbage:

```nil
This source code is licensed under the BSD-style license found in the
LICENSE file in the root directory of this source tree.
```

The problem with this copyright header was specifically the words "in the
LICENSE file in the root directory of this source tree". The copyright header required that the correct license file exist in the root directory of the source tree. This meant that React Native Windows, which was being licensed under the MIT license per Microsoft best practices, would need to have a BSD license file in the canonical license location.

Moral of the story, be careful of the implications of your copyright headers.
