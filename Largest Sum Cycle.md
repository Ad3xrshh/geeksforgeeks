## 01. Largest Sum Cycle

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/largest-sum-cycle--170645/1)

### Problem Description

**Task:** Given an array edge[] of size n, there are n cells numbered from 0 to n - 1. Each cell has at most one outgoing edge.For every cell i:edge[i] is the cell reached from i in one step.edge[i] = -1 means that cell i has no outgoing edge.A cycle is a sequence of cells where, by following the outgoing edges, we eventually return to the starting cell. The sum of a cycle is the sum of the indices of all cells in that cycle.Return the maximum cycle sum. If there is no cycle, return -1.Examples:Input: edge[] = [1, 2, 0, -1]Output: 3Explanation: There is only one cycle in the graph i.e. 0 - > 1 - > 2 - > 0. Sum of the cell index in that cycle = 0 + 1 + 2 = 3.Input: edge[] = [2, 0, -1, 2]Output: -1Explanation: There is no cycle in the graph. The edges are 1 - > 0 - > 2 < - 3. Hence, 2 has no outgoing edge, so no cycle exists.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-02 23:40:15
- **Status:** Correct
- **Marks:** 8

```java
class Solution {
    public int largestSumCycle(int[] edge) {
        int n = edge.length;
        boolean[] visited = new boolean[n];
        long maxSum = -1;

        for (int i = 0; i < n; i++) {
            if (visited[i]) {
                continue;
            }

            HashMap<Integer, Integer> map = new HashMap<>();
            int curr = i;
            int step = 0;

            while (curr != -1 && !visited[curr]) {
                visited[curr] = true;
                map.put(curr, step++);

                curr = edge[curr];

                if (curr != -1 && map.containsKey(curr)) {
                    long sum = 0;
                    int node = curr;

                    do {
                        sum += node;
                        node = edge[node];
                    } while (node != curr);

                    maxSum = Math.max(maxSum, sum);
                    break;
                }
            }
        }

        return (int) maxSum;
    }
}
```

*Generated on: 02/11/2026, 23:44:06*