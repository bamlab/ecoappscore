# GPS Usage

## Problem

When it comes to conserving battery life, it's crucial to consider the impact of GPS data usage in mobile applications.

Using the GPS chip for position sharing significantly drains the device's battery. However, opting for an antenna chip instead of a GPS chip offers a compelling solution, resulting in a remarkable 90% reduction in power consumption related to location services. It's worth noting that using an antenna chip may lead to slightly less accurate positioning compared to GPS.

In certain scenarios, alternative methods such as location tracking through Wi-Fi or phone antennas can be sufficient. Despite these viable alternatives, GPS is often utilised, even when other options are available. By evaluating the specific needs of your app and considering the trade-offs between accuracy and power consumption, you can make informed decisions to optimise energy efficiency in location-based functionalities.

By prioritising power-efficient location services and exploring alternative positioning methods, we can significantly reduce the environmental impact associated with excessive battery consumption.

## Measure

For this indicator, we simply measure the use of the location in the app.

To check that the location is used, you have a status bar icon in both Android and iOS devices.

### Grading

- A: your app never uses location
- B: your app only uses an "imprecise" location (antenna / wifi)
- C: your app uses GPS occasionally
- D: your app uses GPS permanently

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
