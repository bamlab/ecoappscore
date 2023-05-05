# Number of environments

## Problem

An environment (staging, preprod, prod) needs to be deployed on a server. Multiplying the staging environments to have different configurations means multiplying the number of hosted sites. For practical reasons, some projects have multiple staging environments for the different configurations that need to be tested.

## Measure

For this measure, we will count the number of environments deployed for the backend. The dev environment isn't to be counted because it usually comes on top of the staging environment.

### Grading

- A : 2 environments or less (usually staging and prod)
- B : 3 environments
- C : 4 environments
- D : More than 5 environments

**Weighting in the total calculation** : 1

## Other information

There are at least 2 ways to reduce the number of environments

- Try to group the tests on the same environment
- Use different configs in the app rather than different servers
