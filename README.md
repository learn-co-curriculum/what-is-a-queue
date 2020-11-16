# Day 1: Implement a Stack Class

A stack is a data structure where items are processed in last-in-first-out order (LIFO). Similar to a stack of pancakes, where the last pancake placed on the stack is eaten first, the last item placed on the stack is removed and operated upon first. The last item on the stack is known as the **top**, and the first item that was pushed on the stack is known as the **base**. This means that the base is removed from the stack last.

![pancake stack](./pancakes.png)

We use stacks to solve certain algorithm problems. We also think of recursive problems in terms of a stack, since each recursive call results in a stack frame being added to the stack: those frames are then processed and removed in LIFO order! If you are tackling a problem and you see that it must be solved depth-first, this is a good clue that you'll either be using recursion or implementing a stack.

## Wait! This Sounds A Lot Like an Array!

We can actually implement a stack class using an Array as the underlying data structure! Arrays provide all of the methods we need for the core functionality of a stack. Some of the methods we'll be adding to our Stack class include: `push`, `pop`, `peek`, `isEmpty`, `isFull`, and `print`.

//  methods: push, pop, peek, isEmpty, isFull, print //