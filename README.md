# Expo Android Build Failure: IllegalViewOperationException with masked-view

This repository demonstrates a bug and its solution related to building an Android app using Expo CLI. The bug involves the `@react-native-community/masked-view` package and results in a build failure with the `com.facebook.react.uimanager.IllegalViewOperationException`. The solution involves carefully managing the versions of Expo and its associated native modules.

## Bug
The provided `bug.js` file shows a basic React Native component using `masked-view`. When this is built with Expo CLI on Android, the build will fail with the mentioned exception, due to underlying conflicts within the native modules.

## Solution
The `bugSolution.js` file offers a solution by checking for and managing the versions of the native modules to avoid the conflict. This may involve cleaning the build cache, updating packages, or potentially downgrading packages to resolve version mismatch.