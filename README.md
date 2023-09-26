# ****Stacks & Queues Exercises****

## **Queues**

Make a ***Queue*** class. It should include methods for enqueuing, dequeuing, peeking, and checking if the queue is empty.

Make it throw an error if you try to dequeue from an empty queue.

## **Stacks**

Make a ***Stack*** class. It should include methods for pushing, popping, peeking, and checking if the stack is empty.

Make it throw an error if you try to pop from an empty stack.

## **Further Study: Composition**

You’ve probably noticed that your ***Stack*** and ***Queue*** classes involve a lot of duplicate code compared to your ***LinkedList*** class. One way to avoid this problem is to use a ***LinkedList*** class internally to manage your stack or your queue:

```jsx
class Queue {
  constructor() {
    this.size = 0;
    this.first = null;
    this.last = null;
    this._list = new LinkedList();
  }
}
```

Re-implement your classes by using a ***LinkedList*** internally to manage the data structure. Then make a new version using an array instead of a linked list. Which do you prefer?