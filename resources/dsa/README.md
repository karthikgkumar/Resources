---
description: Sliding window
---

# DSA

1.1 Concepts of Sliding Window Technique

#### Concepts of Sliding Window Technique

Imagine you are looking out of a moving train window 🚂. As the train moves, your view changes, but you can only see a fixed portion of the scenery at any given time. This is similar to the sliding window technique in programming.

**Definition:** The sliding window technique is a method used to solve problems that involve a contiguous subset of elements in an array or list. It involves maintaining a window that slides over the data structure to examine different parts of it.

**How It Works:**

1. **Initialization:** Start with a window of a fixed size or an initial position.
2. **Slide the Window:** Move the window one element at a time, updating the relevant variables (like sum, max, min) as you go.
3. **Optimization:** Use the properties of the window to optimize the solution, often reducing the time complexity from O(n^2) to O(n).

**Example:** Let's say you want to find the maximum sum of a subarray of size `k` in an array. Instead of calculating the sum for every possible subarray (which is inefficient), you can use the sliding window technique to keep track of the sum as you slide the window.

Here's a simple Python code snippet to illustrate this:

```python
def max_sum_subarray(arr, k):
    n = len(arr)
    if n < k:
        return -1
    max_sum = sum(arr[:k])
    window_sum = max_sum
    for i in range(n - k):
        window_sum = window_sum - arr[i] + arr[i + k]
        max_sum = max(max_sum, window_sum)
    return max_sum

# Example usage
arr = [1, 2, 3, 4, 5, 6, 7, 8, 9]
k = 3
print(max_sum_subarray(arr, k))  # Output: 24
```

In this example, the window slides over the array, updating the sum by subtracting the element that is left behind and adding the new element that comes into the window. This way, we efficiently find the maximum sum of any subarray of size `k`.

