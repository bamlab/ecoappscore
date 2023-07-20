# Screens Compatibility

## Problem

In today's mobile landscape, we witness a significant trend of increasing screen sizes. However, it's essential to remember that certain users may still utilise devices with specific formats or capabilities. Failing to consider these edge cases can lead to usability issues and disrupt the overall user experience.

As a developer, product owner, or UX/UI designer, it is paramount to account for these variations to ensure a seamless and enjoyable user experience. Let's explore some critical considerations:

- Notch: With the introduction of notched displays on newer devices, it's important to avoid placing crucial components or information in the notch area to ensure optimal visibility and usability.

- Curved screens: For devices with curved screens, it's crucial to prevent text or important UI elements from being distorted or difficult to read along the edges of the screen.

- Very small screens: In the case of devices with smaller screens, special attention should be given to ensure that no essential functionalities are lost or compromised due to limited screen real estate.

- Very large screens: Similarly, when designing for larger screens like iPads, it's vital to ensure that text and other UI elements are legible and properly adapted to the increased display size.

By taking these edge cases into account during the development and design process, we can deliver a seamless user experience across a wide range of devices.

## Measure

For this measure, we will test the app on multiple devices to evaluate the impact on the functionalities :

- Notch : test under iPhone > 10 (big notch)
- Small screen : test under iPhone SE 1st generation
- Large screen : test under tablet
- Curved screen : test under Xiaomi Mi 10

It is possible to test on simulators except for the last one that is only a nice to have.

### Grading

- A: your app proposes an optimal user experience on all screens, in all edge cases
- B: your app proposes a loss of user experience for some edge cases (text too small, curved ...)
- C: your app proposes a loss of minor functionalities on some edge cases
- D: your app proposes a loss of major functionalities of the application in some edge cases

**Weight in the final calculation** : 2

## Other information

To improve user experience on all screens, we recommend using a clear strategy concerning edge cases in design.
