# EcoAppScore

EcoAppScore is a tool developped and maintained by the GreenIT Guild at bamlab. This tool gives your mobile application a score over 20 that represents how eco-designed it is. The documentation provided helps you to understand and measure the impact your app could have on the environment.

Our indicators are meant to evolve, we may have missed some parts and we know they aren’t perfect. For the moment, it is only a base on which to iterate. Sharing them is a way for us to improve this tool. If you are interested, do not hesitate to check the “How to contribute” part.

## How to compute my score

We separate the measure in 3 pillars : device durability, energy sobriety and responsible application. In each pillar you will find macro-indicators in which you will find one file per indicator. Each indicator has its own rating and weight. We also provide some documentation on how and why we decided to take the indicator in our measure.

> Historically, we use a Samsung J3 for all Android measurements. It works as a base for our indicators and all our grades are made for this device. The choice was made to use a low-performance phone to include as many users as possible.

For example, to compute the score for [app’s size][1]. Let’s say my app is 120Mb on iOS and 108Mb on android. If we go through the documentation for the app size indicator we read :

```
- A: ≤ 50 Mb
- B: ≤ 100 Mb
- C: ≤ 150 Mb
- D: > 150 Mb
```

We compute the average between iOS and Android, 114 and we give a note, here it is C.

To compute your score you have to go through our documentation, compute your app’s score for each indicator and compute the final score as follows :

```
(indicator1Rate * indicator1Weight + indicator2Rate * indicator2Weight + ...)/(total)
```

To give you an example, [here is the score computed with EcoAppScore of the Waze app](./WazeExample.md)

## How to contribute

This tool is only at its beginning. We are sharing the V1 and it is meant to be improved. We are opened to suggestions, either to add a new indicator or to improve one already existing, about its measures or its sources and data.

The easiest way to help us is to open an issue with your suggestions so that we can have access to it and decide to take it into account in our tool.

[1]: ./devicesDurability/storageUsage/appSize.md
