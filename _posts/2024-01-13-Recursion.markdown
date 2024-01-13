---
layout: post
title:  "Recursion"
date:   2024-01-13 00:26:07 +0530
categories: Algorithm
---
Recursion

<br>

# Recursion
This is used to solve a smaller instance of the same problem.

<br>

\
\
Below is def of Recursion

``` python
def look_for_key(box):
    for item in box:
    if item.is_a_box():
        look_for_key(item)
    elif item.is_a_key():
        print("found the key!")
```
