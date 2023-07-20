# Functional Compatibility

## Problem

It's important to acknowledge that not all applications can function on every device due to hardware limitations. With each passing year, new smartphones introduce innovative technologies that were nonexistent five or ten years ago. Consequently, if an app relies on these cutting-edge features, users with older devices may face limitations and be unable to fully experience the app's intended functionalities.

By evaluating the presence and importance of these features within an app, we can better understand the extent to which hardware limitations may affect user experience and functionality. This analysis allows us to make informed decisions in balancing cutting-edge technologies with broader device compatibility, ensuring a seamless and inclusive app experience for all users.

## Measure

For this measure, we will quantify the utilisation and significance of various features. The following features are taken into consideration:

- NFC (Near Field Communication) - Such as Apple Pay, enabling convenient contactless payments.
- ARKit - Augmented Reality framework that unlocks immersive and interactive experiences.
- Touch ID - Fingerprint recognition for secure authentication.
- Face ID - Advanced facial recognition for enhanced device security.
- Compass - Accurate directional capabilities for navigation and orientation.

### Grading

- A: your app proposes a full experience without blocking any features

- B: your app proposes a good experience but the full experience with bonuses requires some innovative technologies

- C: your app proposes a partial experience since some parts of the application are missing

- D: your app is unusable on phones that don't have the required technologies

**Weight in the final calculation** : 3

## Other information

### Sources

- [https://developer.apple.com/support/required-device-capabilities](https://developer.apple.com/support/required-device-capabilities/)
- [https://developer.android.com/guide/topics/manifest/uses-feature-element#hw-features](https://developer.android.com/guide/topics/manifest/uses-feature-element#hw-features)
- [https://developer.android.com/guide/practices/compatibility](https://developer.android.com/guide/practices/compatibility)
