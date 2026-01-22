# 📘 Daily Learning – Linked List (Insertion & Deletion)

## 📅 Date
22 January 2026

---

## 🧠 Topic
Singly Linked List – Add and Delete Elements (Java)

---

## 📌 What I Learned Today

Today I learned how to **insert and delete elements in a singly linked list** using Java.  
I understood how nodes are connected using references and how updating the `head` and `next` pointers changes the list.

---

## 🔹 Key Learnings

- A linked list stores data in **nodes**
- Each node has:
  - `data`
  - `next` reference
- Elements are **not stored in contiguous memory**
- Insertion and deletion are done by **changing links, not shifting data**

---

## 🔹 Operations Learned

### ➤ Insert at Beginning
- Create a new node
- Point new node’s `next` to current `head`
- Update `head`

### ➤ Insert at End
- Traverse to last node
- Set last node’s `next` to new node

### ➤ Delete from Beginning
- Move `head` to `head.next`

### ➤ Delete from End
- Traverse to second last node
- Set its `next` to `null`

---

## 💻 Java Code

```java
class Node {
    int data;
    Node next;

    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

class LinkedList {
    Node head;

    void insertAtBeginning(int data) {
        Node newNode = new Node(data);
        newNode.next = head;
        head = newNode;
    }

    void insertAtEnd(int data) {
        Node newNode = new Node(data);
        if (head == null) {
            head = newNode;
            return;
        }
        Node temp = head;
        while (temp.next != null) {
            temp = temp.next;
        }
        temp.next = newNode;
    }

    void deleteFromBeginning() {
        if (head != null) {
            head = head.next;
        }
    }

    void deleteFromEnd() {
        if (head == null || head.next == null) {
            head = null;
            return;
        }
        Node temp = head;
        while (temp.next.next != null) {
            temp = temp.next;
        }
        temp.next = null;
    }
}

