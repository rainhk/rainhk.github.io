---
layout: post
title:  "Quick Sort"
date:   2024-01-22 23:32:43 +0530
categories: Algorithm
---
Quicksort

<br>

# QuickSort
Quicksort is a sorting algorithm that follows the divide and conquer paradigm.
It works by selecting a 'pivot' element from the array and partitioning the other elements into two sub arrays according to whether they are less than or greater than the pivot.

![quicksort](/assets/images/quicksort.jpeg)

Steps are...
1. Select pivot\
    \* Choose a pivot element form the array. Usually first, last or middle element.
2. Paritioning\
    \* Reaarange the array elements such that elements less than the pivot are on the left, and elements greater than the pivot are on the right.
3. Recursion\
    \* Apply Quicksort recursively to the left and right sub arrays. Array will be sorted on this step.

<br>

## Time complexity
On average, it has O(n log n) time complexity.
Worst case happens when the pivot is smallest or largest element. Time complexity for worst case will be O(n^2)

<br>

Simple example quicksort

``` python
def quicksort(array):
    if len(array) == 1:
        return array
    pivot = array[0] # or middle or last element
    less = [i for i in array[1:] if i <= pivot]
    greater = [i for i in array[1: if i > pivot]
    return quicksort(less) + [pivot] + quicksort(greater)
```
