# Screens Compatibility

## Problem

Nowadays, screen sizes are increasing a lot, but some of the users may use some devices that have certain formats or capabilities. This can cause some troubles with the usage of the app.
As developer and/or Product Owner and/or UX/UI designer, it is important to take these edge cases into account so that we avoid disturbing the user experience :

- Notch : no components at the notch location on new devices
- Curved screens : no text too distorted on the edges of the screen
- Very small screens : no lost functionalities on a too small screen
- Very large screen : no unreadable text on iPad screen

## Measure

For this measure, we will test the app on multiple devices to evaluate the impact on the functionalities :

- Notch : test under iPhone > 10 (big notch)
- Small screen : test under iPhone SE 1st generation
- Large screen : test under tablet
- Curved screen : test under Xiaomi Mi 10

It is possible to test on simulators except for the last one that is only a nice to have.

### Grading

- A: I have no loss of user experience, it is optimal on all screens, in all edge cases
- B: I have a loss of user experience for some edge cases (text too small, curved ...)
- C: I have a loss of minor functionalities on some edge cases
- D: I have a loss of major functionalities of the application in some edge cases

**Weight in the final calculation** : 2

## Other information

To improve user experience on all screens, we recommend using a clear strategy concerning edge cases in design.
