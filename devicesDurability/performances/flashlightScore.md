# Flashlight score

## Problem

The performance of an application can be measured through multiple metrics such as:

- Average FPS
- Average CPU usage
- High CPU usage time
- Average RAM usage
- Time to interact

Measuring all of them manually can be difficult and lead to false or imprecise results. Flashlight can solve this issue by running automated tests, measure and write a report with the results of the tests.

A bad score is the reflection of bad performances. The worst a score is, the more the user will find painful to use the application possibly because of:

- Long time to boot
- Lags
- High power consumption
- Processor degradation

All these reasons might lead the user to change his phone because he doesn't find it performing well.

## Measure

For this measure, we will use Flashlight, an open source project developed by BAM. We follow the steps written [here](https://docs.flashlight.dev/) to measure in live the performance of the app or [here](https://docs.flashlight.dev/test/getting-started) if we want to automatise some tests. We can even use [the cloud version](https://docs.flashlight.dev/cloud/intro).

### Grading

- A: The score is ≥90
- B: The score is ≥80
- C: The score is ≥70
- D: The score is <70

**Weighting in the total calculation** : 3

### Sources

- [Flashlight, an open source project](https://github.com/bamlab/flashlight)
- Flashlight cloud uses Samsung A10s to perform the tests and measuring.