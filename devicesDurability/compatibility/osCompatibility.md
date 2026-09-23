# OS Compatibility

## Problem

Understanding the relationship between operating system (OS) support and device compatibility is crucial in the context of eco-design. Each OS version has a specific set of supported devices, and if your phone is not on the list, you are unable to update to the latest OS. However, not extending support to OS versions that are still in use contributes to the issue of phone obsolescence. Users who are unable to update their OS face the challenge of being unable to access updated applications. Regrettably, their only recourse often involves replacing their phone altogether. This presents a significant problem as approximately 80% of a phone's environmental impact stems from its manufacturing phase.

## Measure

For this indicator, we need the minimum version supported on both iOS and Android.

The API number for Android can be found in the build.gradle file: minSdkVersion parameter. For a public application, see on the store. Then the percentage of users having at least this version is displayed.

- Android 17.0 (API Level 37) - 1.0%
- Android 16.0 (API Level 36) - 26.7%
- Android 15.0 (API Level 35) - 43.6%
- Android 14.0 (API Level 34) - 56.7%
- Android 13.0 (API level 33) - 71.5%
- Android 12.0 (API level 31, 32) - 81.5%
- Android 11.0 (API level 30) - 89.9%
- Android 10.0 (API level 29) - 94.1%
- Pie 9.0 (API level 28) - 96.3%
- Oreo 8 (API level 26, 27) - 98.2%
- Nougat 7 (API level 24, 25) - 98.6%
- Marshmallow 6.0 (API level 23) - 99.2%
- Lollipop 5.0 (API level 21, 22) - 99.8%
- Kitkat 4.4 (API level 19) - 99.9%
- Older - 100%

The iOS version number can be read in the podfile or in the app store. Then the percentage of users who have at least this version is displayed.

- 27.X - 0.6%
- 26.X - 75.3%
- 18.X - 91.2%
- 17.X - 93.6%
- 16.X - 96.5%
- 15.X - 98.4%
- 14.X - 98.6%
- 13.X - 98.7%
- 12.X - 99.0%
- 11.X - 99.8%
- 10.X - 99.9%
- Older - 100%

Finally you compute your score based on the use of those device in the mondial population, but it could be adapted to your target user's.

(70% x android score) + (30% x iOS score).

### Grading

- A: your app is compatible with 95% or more of users
- B: your app is compatible with 90% or more of users
- C: your app is compatible with 80% or more of users
- D: your app is compatible with less than 80% of users

**Weight in the final calculation** : 3

## Other information

### Sources

- Last update of share's number for each OS: September 2026.
- Android vs iOS: [https://gs.statcounter.com/os-market-share/mobile/worldwide](https://gs.statcounter.com/os-market-share/mobile/worldwide)
- Android versions: [https://gs.statcounter.com/android-version-market-share/mobile-tablet/worldwide](https://gs.statcounter.com/android-version-market-share/mobile-tablet/worldwide)
- iOS versions: [https://gs.statcounter.com/os-version-market-share/ios/mobile-tablet/worldwide](https://gs.statcounter.com/os-version-market-share/ios/mobile-tablet/worldwide)
