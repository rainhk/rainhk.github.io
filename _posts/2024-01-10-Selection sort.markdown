---
layout: post
title:  "Selection sort"
date:   2024-01-10 20:22:38 +0530
categories: Algorithm
---
Selection sort

<br>

# Selection sort
This sort selects the smallest or biggest element from the unsorted list and move to sorted portion of list

<br>
## Time complexity
O(n) time means you see every element in a list once.\
So seeing a whole list is O(n)


![n^2](/assets/images/n2.jpg)

This takes O(n \* n) time or O(n^2)
\
\
Below is def to find index of smallest item.

``` python
def findSmallest(arr):
    smallest = arr[0]
    smallest_index = 0
    for i in range(1, len(arr)):
        if arr[i] < smallest:
        smallest = arr[i]
        smallest_index = i
    return smallest_index
```

By using the findSmallest function, you can perform selection sort
``` python
def selectionSort(arr):
    newArr = []
    for i in range(len(arr)):
        smallest = findSmallest(arr)
        newArr.append(arr.pop(smallest))
    return newArr
```
