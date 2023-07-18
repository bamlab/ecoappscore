# GPS Usage

## Problem

Using GPS data drastically increases battery consumption

- Using antenna chip instead of GPS chip allows a 90% reduction in power consumption related to position sharing. On the other hand, the position is less accurate.
- In some cases, location by wifi or by phone antenna could be sufficient, but we still use GPS.

## Measure

For this indicator, we simply measure the use of the location in the app.

To check that the location is used, you have a status bar icon in both Android and iOS devices.

### Grading

- A: I never use location
- B: I only use an "imprecise" location (antenna / wifi)
- C: I use GPS occasionally
- D: I use GPS permanently

**Weight in the final calculation** : 3

## Other information

### Application in my app

- Use location symbol to see when you use it
- Try to inject location only in pages that need it

### Sources

Comparison between GPS and other location systems: https://ieeexplore.ieee.org/document/6032390

More detailed explanation of the high consumption of the GPS: https://apple.stackexchange.com/questions/2876/why-does-gps-on-the-iphone-use-so-much-power

How to deactivate precise location (and consume less) :

- Android: https://www.macworld.com/article/3584940/how-to-toggle-location-precision-for-apps-in-ios-14-and-ipados-14.html

- iOS: https://developer.android.com/reference/android/Manifest.permission#ACCESS_COARSE_LOCATION
