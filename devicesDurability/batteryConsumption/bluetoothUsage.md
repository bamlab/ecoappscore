# Bluetooth Usage

## Problem

When it comes to conserving battery life, it's important to consider the impact of Bluetooth usage. Bluetooth serves as a means to exchange data between devices in close proximity. However, it's worth noting that using Bluetooth can significantly drain your device's battery.

In 2010, Bluetooth Low Energy (BLE) was introduced as a variant that consumes less power but offers a lower bandwidth compared to traditional Bluetooth. On the other hand, Near Field Communication (NFC) enables data transfer at approximately 425 kb/s, which is lower than both BLE and regular Bluetooth. If the information exchange doesn't require a higher bandwidth, it's advisable to opt for NFC. Additionally, NFC facilitates short-range exchanges while consuming a similar amount of power as BLE. NFC is particularly useful when one of the parties involved is passive, such as a card terminal (active) and a credit card (passive).

By being mindful of these factors and choosing the appropriate wireless technology for your specific use case, you can optimise battery usage and promote energy efficiency in your app's functionality.

## Measure

For this measure, we will grade what type of short range communication the app uses.

### Grading

- A: your app doesn't use short range communication
- B: your app uses BLE / NFC
- C: your app uses Bluetooth from time to time
- D: your app uses Bluetooth in constant exchange

**Weight in the final calculation** : 3

## Other information

### Application in React Native

NFC: https://github.com/revtel/react-native-nfc-manager
BLE: https://github.com/dotintent/react-native-ble-plx

Bluetooth has the advantage of being compatible with all phones, but it is more consuming. If possible, try to implement the BLE version or NFC for compatible devices.

### Sources

Bluetooh Low Energy: https://en.wikipedia.org/wiki/Bluetooth_Low_Energy
NFC comparison with Bluetooth: https://en.wikipedia.org/wiki/Near-field_communication#Bluetooth_comparison
