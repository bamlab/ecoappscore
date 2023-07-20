![](./assets/BannerEcoAppScore.png)

# EcoAppScore

Developed and maintained by the GreenIT Guild at [BAM.tech](https://www.bam.tech/), EcoAppScore provides your mobile app with a score out of 20 in less than 30 minutes, providing a comprehensive assessment of its eco-design.

The digital world, including mobile devices, is responsible for a significant portion of global carbon emissions. In fact, it currently accounts for 4% of the world's total emissions. Surprisingly, 80% of a mobile device's carbon footprint comes from its production, with only 20% attributed to its usage. These numbers highlight the urgent need for sustainable practices in the digital eco-system.

EcoAppScore evaluates your app's eco-design based on three essential pillars: [device durability](./devicesDurability/devicesDurability.md), [energy sobriety](./energySobriety/energySobriety.md) and [responsible application](./responsibleApplication/responsibleApplication.md/). By assessing these factors, EcoAppScore helps you understand and reduce the environmental impact of your app.

We are sharing this first version and it’s still evolving as we field-test it on the apps we are currently developing.Are you passionate about making a positive impact on the environment? We invite you to explore the "How to contribute" section, where you can actively participate in shaping the future of sustainable mobile applications. Join us and make a difference! 🌱

![](./assets/EcoAppScoreFramework.png)

## How to compute my score

Each pillar contains macro-indicators, which contain indicators. Each indicator has its own markdown describing its grading and weight. We also provide some documentation on how and why we decided to take the indicator in our measure.

> Historically, we use a Samsung J3 for all Android measurements. It works as a base for our indicators and all our grades are made for this device. The choice was made to use a low-performance phone to include as many users as possible.

For example, to compute the score for [app’s size][1]. Let’s say my app is 120 Mb on iOS and 108 Mb on android. If we go through the documentation for the app size indicator we read :

```
- A: ≤ 50 Mb
- B: ≤ 100 Mb
- C: ≤ 150 Mb
- D: > 150 Mb
```

We compute the average between iOS and Android, 114 and we give a note, here it is C.

To obtain the score of your apps, you have to evaluate each indicator and obtain the associated grade. Then, you convert it into numbers with the following equivalences:

- A = 3
- B = 2
- C = 1
- D = 0

Finally, multiply the weight of each indicator with his grade and apply the following formula :

```
20 * (indicator1Grade * indicator1Weight + indicator2Grade * indicator2Weight + ...)/(total)
```

To give you an example, [here is the score computed with EcoAppScore of the Waze app](./WazeExample.md)

## How to contribute

This tool is only at its beginning. We are sharing the V1 and it is meant to be improved. We are opened to suggestions, either to add a new indicator or to improve one already existing, about its measures or its sources and data.

The easiest way to help us is to open an issue with your suggestions so that we can have access to it and decide to take it into account in our tool.

[1]: ./devicesDurability/storageUsage/appSize.md
