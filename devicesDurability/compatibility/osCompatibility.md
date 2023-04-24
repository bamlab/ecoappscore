# OS Compatibility

## Problem

Each version of the operating system supports a certain number of devices. If your phone is not on the list, you cannot update your operating system. Not supporting OS versions that are still in use plays a role in phone obsolescence. Users who can't update their OS find themselves unable to open their updated applications either. The only way out for them is to change their phone. This is a problem because 80% of the environmental impact of our phones is due to its manufacturing phase.

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

- A: 95% or more of users compatible
- B: 85% or more of users compatible
- C: 80% or more of users compatible
- D: Less than 80% of users compatible

**Weight in the final calculation** : 3

## Other information

### Sources

- gs.statcounter.com - November 2022
- [https://blog.bam.tech/developer-news/improving-the-carbon-footprint-of-mobile-applications-a-word-on-compatibility](https://blog.bam.tech/developer-news/improving-the-carbon-footprint-of-mobile-applications-a-word-on-compatibility)
- [https://gs.statcounter.com/android-version-market-share/mobile-tablet/worldwide](https://gs.statcounter.com/android-version-market-share/mobile-tablet/worldwide)
- [https://david-smith.org/iosversionstats/](https://david-smith.org/iosversionstats/)
