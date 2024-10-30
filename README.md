# DEPRECATED

The Repo I merged this from (https://github.com/itinance/react-native-sha256) now supports sha1 using an undocumented feature:

```js
import { sha1 } from 'react-native-sha256';
```

This makes this library obsolete.

# react-native-sha1
sha1 natively for react-native

Speed is king, especially for javascript-driven applications with react-native!
This library provides native sha1-hashes for a string on both iOS and Android
natively.

# Installation
```
yarn add react-native-sha1
react-native link
```

## Adding with CocoaPods

Add the RNSha1 pod to your list of application pods in your Podfile, using the path from the Podfile to the installed module:

```
pod 'RNSha1', :path => '../node_modules/react-native-sha1'
```

Install pods as usual:
```
pod install
```

# Usage

Import the lib into your project:

```javascript
import { sha1 } from 'react-native-sha1';
```

Build a sha1-hash:

```javascript
sha1("Test").then( hash => {
    console.log(hash);
})
```

# File-Hashes

If you need to calculate SHA-1 hashes from a file, use this method of react-native-fs:
(https://github.com/itinance/react-native-fs#hashfilepath-string-algorithm-string-promisestring)