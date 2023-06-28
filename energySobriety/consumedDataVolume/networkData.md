# Network data

## Problem

The number of requests (HTTP, SQL, etc.) necessary for the app to function partly determines the physical resource requirements. It is therefore a key technical indicator to measure the impact of the software layer on the physical infrastructure.

Reducing the number of requests per page is crucial to reduce the number of HTTP servers needed to run the app, and thus the associated environmental impacts.

## Measure

For this measure, we will use both iOS and Android devices.

### iOS

- In Settings > Cellular Data reset the statistics of consumed data
- Turn off the Wi-Fi
- Use the app for about 10 minutes (time yourself by going through the features; if it takes less than 10 minutes, normalize the result later)
- In Settings > Cellular data, watch the volume of data consumed

### Android

- Uninstall the app and reinstall it
- Turn off the Wi-Fi
- Use the app for about 10 minutes
- Hold down the app button > Mobile data and Wi-Fi, note total

### Grading

- A: <25Mb, messaging type without video calls, weather, translation
- B: <50Mb, image search type such as Pinterest
- C: <100Mb, social network type such as instagram
- D: >100Mb, video or streaming service type

**Weight in the final calculation** : 3

## Other information

### Sources

- [Bonne pratique n°9](https://collectif.greenit.fr/ecoconception-web/115-bonnes-pratiques-eco-conception_web.html)
