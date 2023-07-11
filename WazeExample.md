# An example of measurement : Waze

Let's take Waze, a driver assistance app, as an example to compute a score.

## Device durability

### Battery consumption

- For the **bluetooth usage** indicator, looking at playstore permissions, Waze could be paired with Bluetooth Devices, which gives it the rating of C

- For the **colours usage** indicator, the app has a dark mode, the grade is then A

- For the **GPS usage** indicator, Waze needs to use the user location everywhere to work, its grade for this indicator is D

### Compatibility

- For the **functionnal compatibility** indicator, Waze could use a compass for some functionnalities, according to this, its grade is B

- For the **os compatibility** indicator, following the table and looking for the information on PlayStore and AppStore, we see a compatibility of 98% for android users and 94% for iOS users, the weighted average is above 95%, grading it at A

- For the **screen compatibility** indicator, Waze is optimized on all type of screens, grading it at A also

### Performances

- For the **janky frames percentage** indicator, we did the measurement with a samsung J3 and found 67% of janky frames, grading the app at D as it is above 50%.

- For the **launching duration** indicator, we also use a J3 and found a duration between 3 and 6 secondes, which corresponds to the grade B.

### Storage usage

- For the **app size** indicator, a freshly installed app weight 175Mb that is over 150Mb, the grade is then D

- For the **documents and data indicator**, after using the app for 10 minutes, the amount of data stored in our J3 is 83Mb, the according grade is C (between 30 and 100Mb)

## Energy Sobriety

### Consumed data volume

- For the **network data** indicator, we measure 66,26Mb of consumed Data in 10 minutes, which gives the grade C (between 50 and 100b)

### Host usage

- For the **environments number** and **host localisation** indicator, we couldn't find the information concerning Waze, we then skip those indicators

## Responsible Application

### Accessibility

- For the **accessibility** indicator, we had tested the buttons and images with voiceover and some are not well described, according to our indicator, this gives the grade D

### Addictive designs

- For the **addictive designs** indicator, we found those 5 categories in the app: Push Notifications, sharing options, advertisement, gamification (success or functionnality loss depending on the usage), and score system. This leads to the grade of C.

---

## Final Score

We make the ratio between our grades and the maximum grades, and we weight following the indicators. The minimum grade is 0 and the maximum is 3. In the order given above :

```
(3x3 + 3x3 + 0x3 + 2x3 + 3x3 + 3x2 + 0x3 + 2x3 + 0x2 + 1x3 + 1x3 + --- + --- + 0x1 + 1x3) / (3x3+3x3+3x3+3x3+3x3+3x2+3x3+3x3+3x2+3x3+3x3+3x1+3x3) = 48 / 105 = 0,45
```

Usually we score out of 20, which gives the final grade of **9,1/20**
