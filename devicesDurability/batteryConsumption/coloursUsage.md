# Colours Usage

## Problem

This indicator concerns AMOLED screens.
The colour of a pixel rendered impacts power consumption: Black < Green < Red < White < Blue. The higher the screen brightness the greater the difference in consumption.
Then, setting up a "dark mode" can decrease the power consumption of an app.

For LCD type screens, the colour filters are "added" after the rendering of a white pixel. Thus the impact between the colours is less.

## Measure

For this measure, we will take into account:

- the presence of a dark mode

- the colours used by the theme (especially background colour)

### Grading

- A : your app has a single dark theme or two possible modes (dark/light)
- D : your app has a single theme that is not dark

**Weight in the final calculation** : 3

## Other information

### What solution to increase my grade ?

- Try to provide a dark mode in addition to your light mode

- When using a light mode, focus on colours based on their consumption (Black < Green < Red < White < Blue)

### Sources

- [https://www.xda-developers.com/google-wants-developers-to-add-dark-themes-to-save-battery-life/](https://www.xda-developers.com/google-wants-developers-to-add-dark-themes-to-save-battery-life/)
- [https://greenspector.com/en/should-you-switch-your-wallpaper-to-affect-less-the-battery-life-of-your-smartphone/](https://greenspector.com/en/should-you-switch-your-wallpaper-to-affect-less-the-battery-life-of-your-smartphone/)
