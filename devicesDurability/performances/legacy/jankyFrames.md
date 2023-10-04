# Janky Frames

## Problem

The application needs to generate a sufficient number of frames per second (FPS) in order to have a pleasant user experience, both on the UI and JS side.

If there are too few FPS, the application may "freeze" visually. A JS freeze implies that data is not loaded. A UI freeze implies slow animations. This performance may cause the user to switch to another phone.

The goal is to have 60 FPS constant both for the UI and JS.

## Measure

For this measure, we will count the number of janky frames across the app.

### iOS

For the moment, it is not possible to perform this measure on iOS.

### Android

Use a Samsung J3.

- Connect the device to a computer. It is necessary to activate the developer mode on the phone
- Get the package name of the app in production (e.g. com.airbnb.airbnb)
- You can look for this value (if necessary) in the terminal by typing `adb shell pm list packages`
- Kill the app you're going to test
- Restart it, go through all the screens and then call in a terminal `adb shell dumpsys gfxinfo <packageDeLApp>`
- Read the percentage of janky frames

```
Stats since: 21842914294997ns
Total frames rendered: 2654
Janky frames: 1975 (74.42%)
```

### Grading

We have tested an application with 23% of janky frames. The user notices it but it isn't annoying. The indicator is rather subjective and arbitrary for the moment. It will evolve.

Score according to the number of junk frames observed :

- A < 15% : The user does not perceive the janky frames
- B < 30% : The user hardly notices the janky frames
- C < 50% : The janky frames are visible but it's not too annoying
- D > 50% : The user experience is degraded enough to annoy him

**Weighting in the total calculation** : 3

## Other information

### Sources

- [For Flutter apps](https://flutter.dev/docs/cookbook/testing/integration/profiling)
- [For React Native apps](https://github.com/bamlab/react-native-performance)
- [For native apps](https://developer.android.com/training/testing/performance)
