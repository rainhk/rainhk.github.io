---
layout: post
title:  "Binary search"
date:   2024-01-11 22:42:33 +0530
categories: Algorithm
---
Binary search

<br>

# Binary search
This is an algorithm for finding a target value within a sorted array or list.

<br>

You will basically keep diving the list half and compare to your target number.

## Time complexity
The time complexity of this algorithm is O(log n) which makes significant faster than linear search as long as the list is sorted.



![binary](/assets/images/binary search.png)

\
\
Below is def of binary search

``` python
def binarySearch(list, item):
    low = 0
    high = len(list) - 1
    while low <= high:
        mid = (low + high)/2
        guess = list[mid]
        if guess == item:
            return mid
        if guess < item:
            low = mid + 1
        else:
            high = mid - 1
    return None
```
