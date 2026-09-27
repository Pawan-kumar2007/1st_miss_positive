# 1st_miss_positive
**LeetCode 41 - First Missing Positive
Problem**

Given an unsorted integer array nums, find the smallest positive integer that is not present in the array.

**Approach**
First, sort the array using Arrays.sort().
Set expect = 1 because we need to find the smallest positive number.
Traverse the sorted array.
If the current element is equal to expect, increment expect.
If the current element is greater than expect, return expect.
After traversing the array, return expect.
**Example**

Input:
[3, 4, -1, 1]

After sorting:
[-1, 1, 3, 4]

Expected positive numbers:
1, 2, 3, 4...

1 is present, but 2 is missing.

Output:
2
