# Expo Linking.getInitialURL() - Intermittent null return on Android

This repository demonstrates a bug in Expo's `Linking.getInitialURL()` API on Android.  The issue is that the method sometimes returns `null`, even when a deep link has been successfully opened. This behavior is not consistent and is difficult to reliably reproduce, making debugging challenging.

The `bug.js` file shows the problematic code, and `bugSolution.js` offers a potential workaround.

## Reproduction Steps

1. Install the Expo Go app.
2. Run the app.
3. Open a deep link that should trigger the `Linking.getInitialURL()` call.
4. Observe that sometimes `Linking.getInitialURL()` returns null, even if the deep link successfully launched the app.