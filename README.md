# 75. Sort Colors

## Problem

Given an array `nums` containing only `0`, `1`, and `2`, sort the array in-place so that all `0`s come first, followed by all `1`s, and then all `2`s.

- `0` → Red
- `1` → White
- `2` → Blue

## Approach - Built-in Sorting

Use Java's built-in `Arrays.sort()` method to sort the array in ascending order.

Since the array contains only `0`, `1`, and `2`, sorting automatically arranges the colors in the required order.

## Code

```java
class Solution {
    public void sortColors(int[] nums) {
        Arrays.sort(nums);
    }
}
```

## Dry Run

Input:

```text
nums = [2,0,2,1,1,0]
```

After sorting:

```text
[0,0,1,1,2,2]
```

Output:

```text
[0,0,1,1,2,2]
```

## Complexity Analysis

- Time Complexity: O(n log n)
- Space Complexity: O(log n) (depends on the sorting implementation)

## Key Concept

`Arrays.sort()` uses Java's optimized sorting algorithm to arrange elements in ascending order. Since `0 < 1 < 2`, the colors are automatically grouped together after sorting.

## Note

Although this solution is simple and accepted in many environments, the problem specifically asks for a one-pass constant-space solution. The optimal approach is the Dutch National Flag Algorithm, which runs in O(n) time and O(1) extra space.
