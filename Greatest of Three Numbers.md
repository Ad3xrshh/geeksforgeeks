## 01. Greatest of Three Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/greatest-of-three-numbers2520/1)

### Problem Description

**Task:** Given three numbers a, b and c. Find the greatest number among them.Examples:Input: a = 10, b = 3, c = 2

#### Examples

##### Example 1

- **Output:**
```text
-2
```
- **Explanation:** -2 is greatest among the three

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C)

- **Submitted:** 2026-11-04 19:17:50
- **Status:** Correct
- **Marks:** 1

```c
#include <stdio.h>

int main() {
    int a, b, c;
    scanf("%d %d %d", &a, &b, &c);

    if (a>b&&a>c)
        printf("%d",a);
    else if (b>c&&b>a)
        printf("%d",b);
    else 
        printf("%d",c);
    

    return 0;
}
```

*Generated on: 04/11/2026, 19:18:15*