## Stack Implementation Using Linked List

### Concept

A **Stack** is a linear data structure that follows the **LIFO (Last In First Out)** principle.
The element inserted last will be removed first.

Example:

Push: `10 → 20 → 30`

Stack:

Top → 30
20
10

When **pop()** is called, **30** will be removed first.

---

### Basic Stack Operations

* **push(x)** → Insert element at the top
* **pop()** → Remove the top element
* **peek()** → Return the top element without removing it
* **isEmpty()** → Check if stack is empty

---

### Implementation Idea

In the **Linked List implementation of Stack**:

* Each element is stored inside a **Node**
* Each node contains:

  * `data`
  * `next` pointer
* The **top pointer represents the head of the linked list**

---

### Java Implementation

```java
class Stack {

    class Node {
        int data;
        Node next;

        Node(int data) {
            this.data = data;
            this.next = null;
        }
    }

    Node top;

    void push(int x) {
        Node newNode = new Node(x);

        newNode.next = top;
        top = newNode;
    }

    int pop() {
        if (top == null) {
            System.out.println("Stack Underflow");
            return -1;
        }

        int value = top.data;
        top = top.next;

        return value;
    }

    int peek() {
        if (top == null) {
            return -1;
        }

        return top.data;
    }

    boolean isEmpty() {
        return top == null;
    }
}
```

---

### Key Points

* Stack follows **LIFO principle**
* Linked List implementation allows **dynamic memory allocation**
* No fixed size limitation like arrays

