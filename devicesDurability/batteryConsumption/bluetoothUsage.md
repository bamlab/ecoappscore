# Bluetooth Usage

## Problem

Using Bluetooth drastically increases battery consumption.

Bluetooth is a way to exchange data between devices in close proximity. There is a variant called Bluetooth Low Energy, introduced in 2010, which consumes less power but has a lower bandwidth.

NFC allows a transfer of ~425 kb/s, less than its counterpart BLE and even less than Bluetooth. If the exchange of information does not need to be more important than that, it is better to use NFC. It also allows short-range exchanges with a similar consumption as BLE. NFC works if one of the parties is passive (e.g. card terminal (active) and credit card (passive))

## Measure

For this measure, we will grade what type of short range communication the app uses.

### Grading

- A: no short range communication
- B: BLE / NFC
- C: Bluetooth from time to time
- D: Bluetooth in constant exchange

**Weight in the final calculation** : 3

## Other information

### Application in React Native

NFC: https://github.com/revtel/react-native-nfc-manager
BLE: https://github.com/dotintent/react-native-ble-plx

Bluetooth has the advantage of being compatible with all phones, but it is more consuming. If possible, try to implement the BLE version or NFC for compatible devices.

### Sources

Bluetooh Low Energy: https://en.wikipedia.org/wiki/Bluetooth_Low_Energy
NFC comparison with Bluetooth: https://en.wikipedia.org/wiki/Near-field_communication#Bluetooth_comparison
