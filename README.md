# Day 1: Implement a Stack Class

**Fork and then clone me!**

A stack is a data structure where items are processed in last-in-first-out order (LIFO). Similar to a stack of pancakes, where the last pancake placed on the stack is eaten first, the last item placed on the stack is removed and operated upon first. The last item on the stack is known as the **top**, and the first item that was pushed on the stack is known as the **base**. This means that the base is removed from the stack last.

![pancake stack](./pancakes.png)

We use stacks to solve certain algorithm problems. We also think of recursive problems in terms of a stack, since each recursive call results in a stack frame being added to the stack: those frames are then processed and removed in LIFO order! If you are tackling a problem and you see that it must be solved depth-first, this is a good clue that you'll either be using recursion or implementing a stack. Depth-first means that we go as deep as we can before we start processing data (LIFO order).

## Wait! This Sounds A Lot Like an Array!

We can actually implement a stack class using an Array as the underlying data structure! Arrays provide all of the methods we need for the core functionality of a stack. Some of the methods we'll be adding to our Stack class include: `push`, `pop`, `peek`, `isEmpty`, and `print`. Do any of those sound familiar?

## Implement the Stack Class

The Stack class already has two attributes: the `stack` itself (an Array) and a `limit`, which is an Integer representing the total number of items allowed in the Stack at one time.

Add the following methods to the Stack class:

### `push`

`push` adds an item to the top of the Stack. If the Stack is full, the item should not be pushed and an Error should be thrown.

### `pop`

`pop` removes the item at the top of the Stack.

### `peek`

`peek` returns the item at the top of the Stack without removing it.

### `isEmpty`

`isEmpty` returns `true` if the Stack is empty, otherwise `false`.

### `isFull`

`isFull` returns `true` if no more space is available in the Stack, otherwise `false`.

### `size`

`size` returns the number of items currently on the Stack.

### `search(target)`

`search` returns an Integer representing how far the target item is from the top of the stack. If the item is not in the Stack, return `-1`. Example:

```
// Stack = 1, 2, 3, 4, 5 <-top

stack.search(5) => 0
stack.search(4) => 1
stack.search(6) => -1
```

### `print`

`print` prints the contents of the stack. It does not return them! You may print them however you wish.

We've provided starter code for some languages. Choose whichever language you like. Once again, we recommend writing your own tests first and then running the test suites.

## How to run your own tests

### Ruby

1. `cd` into the ruby folder
2. `ruby <filename>.rb`

### JavaScript

1. `cd` into the javascript folder
2. `node <filename>.js`

## How to run our tests

### Ruby

1. `cd` into the ruby folder
2. `bundle install`
3. `rspec`

### JavaScript

1. `cd` into the javascript folder
2. `npm i`
3. `npm test`
