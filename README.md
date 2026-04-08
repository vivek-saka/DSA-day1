# DSA-day1
ptod

# XOR After Queries

[![Language](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📝 Problem Statement

Given an integer array `nums` of length `n` and a 2D integer array `queries` of size `q`, where each query is `[li, ri, ki, vi]`, perform the following operations **in order** for each query:

1. Set `idx = li`
2. While `idx <= ri`:
   - Update: `nums[idx] = (nums[idx] * vi) % (10^9 + 7)`
   - Set `idx += ki`
3. Return the **bitwise XOR** of all elements in `nums` after processing all queries.

## 🔍 Examples

### Example 1
```cpp
Input: nums = [1,1,1], queries = [[0,2,1,4]]
Output: 4
