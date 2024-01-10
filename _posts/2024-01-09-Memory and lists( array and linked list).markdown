---
layout: post
title:  "Arrays and linked lists"
date:   2024-01-09 20:56:58 +0530
categories: Algorithm
---
Linked list or Array?

\
<br>

# Linked List
\
Items can be stored in anywhere in memory.
Each item stores the address of the next item in the list.

![LinkedList](/assets/images/linked list.jpg)

With Linked list, there is no need to move items.

Linked list is good for insertions.

<br>

# Array
\
Linked list is not a best list to use if you need to keep jump around items.\
It is good if you are getting all the items in the list.
\
\
But an array is different.\
You won't know addresses of the items in list for the linked list.\
But you will know addresses of the items in the array.\
\
Lists start from 0. Then for the array, what would be the address of 4th item in array of 5?\
\
The address or index will be '3'.
\
<br>

## Inserting into the middle of a list

**Linked list**\
It is pretty easy with linked list.\
All you need to do is just changing what previous element points to..
\
![linked insert](/assets/images/linked insert.jpg)

**Array**\
If there is no available space or memory, you might need to copy everything to a new location that can fit with a new item.
\
![array insert](/assets/images/array insert.jpg)

## Run time of array and linked list
\
![runtime](/assets/images/runtime array linked.jpg)


<!--Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].-->
<!---->
<!--[jekyll-docs]: https://jekyllrb.com/docs/home-->
<!--[jekyll-gh]:   https://github.com/jekyll/jekyll-->
<!--[jekyll-talk]: https://talk.jekyllrb.com/-->
