# BIG O Simplified

This repo is a "Cheat Sheet for Big O". It provides a simplified explanation on the BIg O (Time and Space Complexity).

## Time Complexity
How much more runtime do we need as the inputs get larger.

### RULES FOR BIG O (Time Complexity)
- Iterating over a collection or using **n** as a pointer within a for loop = **`O(n)`**
- Iterating over the same collection with nested for lopps = **`O(n^2)`**
- Iterating over the different collection with nested for lopps = **`O(n \* m)`**


#### Things To Remember
- Constants does not matter because Big O only matters when the data is very big ( worst case scenrio ). For example:
  - `O(12)`, `O(702)` are considered  `O(1)`
  - Similarly `O(2n) = O(n)`, and `O(n / 2) = O(n)`
  - `O(13n ^ 2) = O(n ^ 2)`
- Smaller Terms do not matter as + 10 in front of 1 Billion is negligible. For example:
  -  `O(123n + 10) = O(n)`
  - `O(n ^ 2 + 13n + 8) = O(n ^ 2)`

-   Arithmatic Operations have Constant Time Complexity (O(1)), this means, your processor takes same time to calculate ```1 + 1``` and ```10000000000 + 1```.
-   Variable Assignment have Constant Time Complexity (O(1)), this means, your processor takes same time to calculate ```var x = 1``` and ```var x = 10000000000```.


#### A.K.A's

- `O(1)` = Constant Time Complexity
- `O(n)` = Linear Time Complexity
- `O(n^2)` = Quadratic Time Complexity

---

## Space Complexity
How much more memory use (RAM) do we need as the inputs provided to the code gets larger


### RULES FOR BIG O (Space Complexity)
- Storing values in memory takes up Memory:
  - Most Premitives (Numbers, and Booleans) take O(1) / Constant space
    - `x = 100` takes same space as `x = 10000`
  - Strings, Arrays, Objects take O(n) / Linear space
    // array of 10 takes double space as array of 5, similarly, a string with 10 characters takes double space as compared to 5 chars.

- Prioritize Time Complexity Over Space Complexity because the cost to run processors is much higher as compared to rams. In other words, processors do the heavy lifting, that is why they cost more, so genrally time is more important.
- But in some scnerios, where space is limited, space can also be prioritised.
