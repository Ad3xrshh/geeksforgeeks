## 01. Sum of Natural Number Cubes

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-of-first-n-terms5843/1)

### Problem Description

**Task:** Given an integer n, calculate the sum of series 1³ + 2³ + 3³ + 4³ + … till n-th term.Examples:Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
784
```
- **Explanation:** 1³ + 2³ + 3³ + 4³ + 5³ + 6³ + 7³ = 784

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-04 19:22:08
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    int sumOfSeries(int n) {
        
         
        int sumcube = n*n*(n+1)*(n+1)/4;
        return sumcube;
        
    }
}
```

*Generated on: 04/11/2026, 19:22:33*