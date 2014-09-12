# Mobile Appmaker

Mobile Appmaker is a product exploring how to radically lower the entry to creating and distributing mobile applications through on-device authoring.

## Overview

Mobile Appmaker is structured around a number of lightweight composable CommonJS modules that provide abstractions for routing, XHR, IndexedDB, i18n, and MVVM. Bundling for distribution is handled by browserify. Testing is handled by mocha and phantomjs.

Views and components are the basic building blocks of Appmaker. Views are the highest level object and represent a discrete screen such as "Discover" or "App Details". Both are defined via the MVVM abstractions provided by Vue.js.
