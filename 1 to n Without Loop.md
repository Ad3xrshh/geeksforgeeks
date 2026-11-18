## 01. 1 to n Without Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-1-to-n-without-using-loops3621/1)

### Problem Description

**Task:** Given an positive integer n, print numbers from 1 to n without using loops. Implement the function printTillN() to print the numbers from 1 to n as space-separated integers.Examples Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
1 2 3 4 5 6 7 8 9 10
```
- **Explanation:** We have to print numbers from 1 to 10.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-18 19:14:04
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    void printTillN(int n) {
        if (n == 0) {
            return;
        }

        printTillN(n - 1);
        System.out.print(n + " ");
    }
}
```

*Generated on: 18/11/2026, 19:14:28*