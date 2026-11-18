## 01. Print n to 1 Without Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-n-to-1-without-loop/1)

### Problem Description

**Task:** Given an integer n, print all numbers from n to 1 in decreasing order, separated by spaces, without using any loops.Examples :Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
3 2 1
```
- **Explanation:** The numbers from 3 to 1 are printed in decreasing order

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-18 19:18:45
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int printNos(int n) {
        if (n==0){
            return 0;
        } else {
            System.out.print(n+" ");
        }
        return printNos(n-1);
    }
}
```

*Generated on: 18/11/2026, 19:19:13*