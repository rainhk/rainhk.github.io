---
layout: post
title:  "Stack"
date:   2024-01-14 16:20:43 +0530
categories: DataStructure
---
Stack

<br>

# Stack
This is a fundamental data structure that follows Last In, First Out principle.\
The last element added to the stack and is the first one to be removed.\
![stack](/assets/images/stack.jpeg)

Key operations are...
1. Push\
    \* Adds an element to the top of the stack
2. Pop\
    \* Rmoves the element from the top of the stack
3. Peek or Top\
    \* Returns the element at the top of the stack without removing it
4. isEmpty\
    \* Checks if the stack is empty

<br>

## Call stack
This is a data structure that tracks the execution flow of a program when functions are called.\
Every time a function is called, its information is pushed onto the stack, and when the function returns, its information is popped off the stack.

<br>

Simple example of call stack

``` python
def func1():
    print("Function 1")
    func2()

def func2():
    print("Function 2")
    
func1()
```

When 'func1' is called, the information about the currently executing function along with the command to call 'func2' is pushed onto the call stack. \
When 'func2' is executed, its information is also added to the stack.\
As each function completes its execution, its information is popped off the stack.

For recursion, function keeps calls itself until base case.\
Once it reaches the base case, the stack (information) removes one by one.
