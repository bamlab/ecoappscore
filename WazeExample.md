# An example of measurement : Waze

Let's take Waze, a driver assistance app, as an example to compute a score.

Waze obtains the final grade of 🔴 **8.75 / 20** . 

Here is the detail of each indicator parts in the final grade:

| Category                | Indicator            | Weight | Grade | Score |
|----------------------|------------------------|--------|-------|-----|
| **DEVICES DURABILITY**   |                        |        |       |     |
| ***Battery consumption***|                    |        |       |     |
|                      | Colors usage within the app| 3    | A     | 9   |
|                      | Bluetooth usage        | 3      | C     | 3   |
|                      | GPS usage              | 3      | D     | 0   |
| ***Compatibilities***|                        |        |       |     |
|                      | Functional Compatibilities | 3  | B | 6 |
|                      | OS Compatibilities     | 3      | A     | 9   |
|                      | Screens Compatibilities| 2     | A     | 6   |
| ***Mobile performance***|                     |        |       |     |
|                      | Flashlight Score       | 3      | D     | 0   |
| ***Storage usage***  |                        |        |       |     |
|                      | App size               | 2      | D     | 0   |
|                      | Documents and data     | 3      | C     | 3   |
| **ENERGY SOBRIETY**      |                        |        |       |     |
| ***Consumed data volume***|                   |        |       |     |
|                      | Network data           | 3      | C     | 3   |
|***Host usage***      |                        |        |       |     |
|                      | Host localisation      | 3      |    -   |  -   |
|                      | Environments Number    | 1      |   -    |  -   |
| **RESPONSIBLE APPLICATION** |                     |        |       |     |
|                      | Accessibility          | 1      | D     | 0   |
|                      | Addictive designs      | 3      | C     | 3   |


## Device durability

### Battery consumption

- For the [**bluetooth usage**][1] indicator, looking at playstore permissions, Waze could be paired with Bluetooth Devices, without needing it on a constant basis according to its users. It gives it the rating of C

- For the [**colours usage**][2] indicator, the app has a dark mode, the grade is then A

- For the [**GPS usage**][3] indicator, Waze needs to use the user location everywhere to work, its grade for this indicator is D

### Compatibility

- For the [**functionnal compatibility**][4] indicator, Waze could use a compass for some functionnalities, according to this, its grade is B

- For the [**os compatibility**][5] indicator, following the table and looking for the information on PlayStore and AppStore, we see a compatibility of 98% for android users and 94% for iOS users, the weighted average is above 95%, grading it at A

- For the [**screen compatibility**][6] indicator, Waze is optimized on all type of screens, grading it at A also

### Performances

- For the **Flashlight score** indicator, we did the measurement with Flashlight cloud and found a score of 60, which gives the app a score of D.
![](./assets/WazeFlashlightScore.png)

### Storage usage

- For the [**app size**][9] indicator, a freshly installed app weight 175Mb that is over 150Mb, the grade is then D

- For the [**documents and data indicator**][10], after using the app for 10 minutes, the amount of data stored in our J3 is 83Mb, the according grade is C (between 30 and 100Mb)

## Energy Sobriety

### Consumed data volume

- For the [**network data**][11] indicator, we measure 66,26Mb of consumed Data in 10 minutes, which gives the grade C (between 50 and 100b)

### Host usage

- For the [**environments number**][12] and [**host localisation**](energySobriety/hostUsage/hostLocalisation.md) indicator, we couldn't find the information concerning Waze, we then skip those indicators

## Responsible Application

### Accessibility

- For the [**accessibility**][13] indicator, we had tested the buttons and images with voiceover and some are not well described, according to our indicator, this gives the grade D

### Addictive designs

- For the [**addictive designs**][14] indicator, we found those 5 categories in the app: Push Notifications, sharing options, advertisement, gamification (success or functionnality loss depending on the usage), and score system. This leads to the grade of C.

---

## Final Score

Once we have obtained the grades for each indicator, we convert them into numbers with the following equivalences.

- A = 3
- B = 2
- C = 1
- D = 0

Then, we add the weight of each indicator. In the order given above :

```
(3x3 + 3x1 + 0x3 + 2x3 + 3x3 + 3x2 + 0x3 + 0x2 + 1x3 + 1x3 + --- + --- + 0x1 + 1x3) / (3x3+3x3+3x3+3x3+3x2+3x3+3x3+3x2+3x3+3x3+3x1+3x3) = 42 / 96 = 0,45
```

Usually we score out of 20, which gives the final grade of **8.75/20**

[1]: devicesDurability/batteryConsumption/bluetoothUsage.md
[2]: devicesDurability/batteryConsumption/coloursUsage.md
[3]: devicesDurability/batteryConsumption/gpsUsage.md
[4]: devicesDurability/compatibility/functionalCompatibility.md
[5]: devicesDurability/compatibility/osCompatibility.md
[6]: devicesDurability/compatibility/screensCompatibility.md
[7]: devicesDurability/performances/jankyFramesPercentage.md
[8]: devicesDurability/performances/launchingDuration.md
[9]: devicesDurability/storageUsage/appSize.md
[10]: devicesDurability/storageUsage/documentsAndData.md
[11]: energySobriety/consumedDataVolume/networkData.md
[12]: energySobriety/hostUsage/environmentsNumber.md
[13]: responsibleApplication/accessibility/accessibility.md
[14]: responsibleApplication/addictiveDesigns/addictiveDesigns.md
