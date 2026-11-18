## 01. Power Using Recursion

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/power-using-recursion/1)

### Problem Description

**Task:** You are given two numbers n and p. You need to find n^p.

#### Examples

##### Example 1

- **Input:**
```text
n = 9, p = 9
```
- **Output:**
```text
387420489
```
- **Explanation:** 9 raised to power 9 is 387420489.

##### Example 2

- **Input:**
```text
n = 2, p = 9
```
- **Output:**
```text
512
```
- **Explanation:** 2 raised to power 9 is 512.

#### Constraints

- **1.** `1 ≤ n ≤ 100 ≤ p ≤ 9`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(p)
- **Expected Auxiliary Space Complexity:** O(p)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-18 19:27:47
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int recursivePower(int n, int p) {
        if (p==0){
            return 1;
        } 
        return n*recursivePower(n,p-1);
    }
}
```

*Generated on: 18/11/2026, 19:28:14*