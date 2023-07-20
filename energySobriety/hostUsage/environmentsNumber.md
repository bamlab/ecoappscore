# Number of environments

## Problem

Setting up different environments (such as staging, preprod, and prod) on servers is a necessary step in the app development process. However, it's important to consider the implications of multiplying staging environments for various configurations.

Each additional staging environment requires hosting resources and contributes to an increased number of hosted sites. While having multiple staging environments may be necessary to test different configurations, it's crucial to strike a balance between practicality and resource efficiency.

By optimising the setup and management of staging environments, we can minimise unnecessary resource consumption. This can include implementing strategies such as utilising shared resources, optimising configurations, or adopting efficient virtualisation techniques. Such practices not only reduce the environmental impact associated with hosting multiple sites but also promote cost-effectiveness and streamline the development process.

## Measure

For this measure, we will count the number of environments deployed for the backend. The dev environment isn't to be counted because it usually comes on top of the staging environment.

### Grading

- A: your app uses 2 environments or less (usually staging and prod)
- B: your app uses 3 environments
- C: your app uses 4 environments
- D: your app uses more than 5 environments

**Weighting in the total calculation** : 1

## Other information

There are at least 2 ways to reduce the number of environments

- Try to group the tests on the same environment
- Use different configs in the app rather than different servers
