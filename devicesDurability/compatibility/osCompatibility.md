# OS Compatibility

## Problem

Understanding the relationship between operating system (OS) support and device compatibility is crucial in the context of eco-design. Each OS version has a specific set of supported devices, and if your phone is not on the list, you are unable to update to the latest OS. However, not extending support to OS versions that are still in use contributes to the issue of phone obsolescence. Users who are unable to update their OS face the challenge of being unable to access updated applications. Regrettably, their only recourse often involves replacing their phone altogether. This presents a significant problem as approximately 80% of a phone's environmental impact stems from its manufacturing phase.

## Measure

For this indicator, we need the minimum version supported on both iOS and Android.

The API number for Android can be found in the build.gradle file: minSdkVersion parameter. For a public application, see on the store. Then the percentage of users having at least this version is displayed.

- Android 12.0 (API level 31, 32) - 30%

- Android 11.0 (API level 30) - 55%

- Android 10.0 (API level 29) - 74%

- Pie 9.0 (API level 28) - 83%

- Oreo 8 (API level 26, 27) - 88%

- Nougat 7 (API level 24, 25) - 90%

- Marshmallow 6.0 (API level 23) - 92.5%

- Lollipop 5.1 (API level 22) - 94.5%

- Lollipop 5.0 (API level 21) - 98%

- Kitkat 4.4 (API level 19) - 99,6%

- Older - 100%

The iOS version number can be read in the podfile or in the app store. Then the percentage of users who have at least this version is displayed.

- 16.X - 40%

- 15.X - 87%

- 14.X - 93%

- 13.X - 94%

- 12.X - 97,5%

- 10/11.X - 98,5%

- Older - 100%

Finally you compute your score based on the use of those device in the mondial population, but it could be adapted to your target user's.

(70% x android score) + (30% x iOS score).

### Grading

- A: your app is compatible with 95% or more of users
- B: your app is compatible with 85% or more of users
- C: your app is compatible with 80% or more of users
- D: your app is compatible with less than 80% of users

**Weight in the final calculation** : 3

## Other information

### Sources

- gs.statcounter.com - November 2022
- [https://blog.bam.tech/developer-news/improving-the-carbon-footprint-of-mobile-applications-a-word-on-compatibility](https://blog.bam.tech/developer-news/improving-the-carbon-footprint-of-mobile-applications-a-word-on-compatibility)
- [https://gs.statcounter.com/android-version-market-share/mobile-tablet/worldwide](https://gs.statcounter.com/android-version-market-share/mobile-tablet/worldwide)
- [https://david-smith.org/iosversionstats/](https://david-smith.org/iosversionstats/)
