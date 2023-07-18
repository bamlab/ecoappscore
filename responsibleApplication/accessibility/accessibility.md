# Accessibility

## Problem

In the realm of responsible application design, it is paramount to ensure usability for all users, regardless of any impairments they may have. Every individual should be able to access and engage with applications, aiming to minimise any negative impact on their experience.

By prioritising accessibility, we can create inclusive app experiences that cater to diverse user needs. Incorporating features such as screen readers, adjustable font sizes, high contrast modes, and closed captions for multimedia content can greatly enhance accessibility for users with visual or hearing impairments.

By striving to make applications universally accessible, we empower individuals with disabilities to fully engage with digital experiences.

## Measure

For this measure, we will use a list of different criteria. For each criteria we note if it is met or not, or if it doesn't concern the app. At the end, the grade is based on which criteria are not met.

### General

- My app is fully translated for my users.
- All pages have a title.
- Each form element has a label and not only a placeholder.
- There is no intrusive popup (exception: native permissions request).

### Visually impaired users

- The interactive elements (e.g. buttons) all have an explicit description (what it does and current state), available in all languages of the application. They are not used as incomprehensible ID tests.
  - to check when activating VoiceOver on iPhone: are all buttons described aloud when clicked (and in a note at the bottom of the screen)?
- Essential images have alternative text translated into the users' language. Decorative elements have no text.
- Essential audio and video content has an audio description, in the users' language.
- The font grows when you increase the text size in the settings.
- I have a minimum rating of AA everywhere on my app in color contrast.
  - Download the Pika app for Mac and check the sensitive buttons of the app (on mockup or simulator).
  - The criteria is not met if at least one button has a bad text contrast.

### Hearing impaired users

- Essential audio and video content has subtitles in the user's language.

### Motor disability

- If I have complex gestures in my app (e.g. shake the phone), the user can replace them by others in the accessibility settings.

### Grading

- A: your app respects all accessibility criteria (or "not concerned")

- B: your app does not respect criterias only among "growing text" and "color contrast"

- C: your app does not respect criterias only among "page title", "intrusive popup", "phone shake gesture", "form label"

- D: your app does not respect criterias "button with description" or "essential image with description"

**Weight in the final calculation** : 1

## Other information

### Sources

[https://www.w3.org/WAI/](https://www.w3.org/WAI/)

[https://www.numerique.gouv.fr/publications/rgaa-accessibilite/methode-rgaa/criteres/#topic12](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/methode-rgaa/criteres/#topic12)

[https://www.atalan.fr/agissons/fr/](https://www.atalan.fr/agissons/fr/)

[https://reactnative.dev/docs/accessibility](https://reactnative.dev/docs/accessibility)

[https://reactnative.dev/docs/text#allowfontscaling](https://reactnative.dev/docs/text#allowfontscaling)
