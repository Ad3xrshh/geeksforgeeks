## 01. Factorial

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/factorial5739/1)

### Problem Description

**Task:** Given a positive integer, n. Find the factorial of n.Examples :Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
24
```
- **Explanation:** 1 x 2 x 3 x 4 = 24

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C)

- **Submitted:** 2026-11-04 19:15:20
- **Status:** Correct
- **Marks:** 1

```c
int factorial(int n) {
    if (n==0) 
        return 1;
    if (n==1){
        return 1;
    }else
        return n*factorial(n-1);
}
```

*Generated on: 04/11/2026, 19:16:11*