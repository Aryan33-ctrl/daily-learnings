# Day 5 — Linked List Basics

## What I Learned Today

### ✅ What is a Linked List?

A Linked List is a linear data structure where elements are stored in **nodes** rather than in contiguous memory like an array.

Each node contains:

* **Data**
* **Reference (pointer) to the next node**

This makes linked lists dynamic in size and flexible for insertion and deletion.

---

## Types of Linked Lists

1. **Singly Linked List**
   Each node points only to the next node.

2. **Doubly Linked List**
   Each node has two pointers:

   * Previous
   * Next

3. **Circular Linked List**
   The last node points back to the first node, forming a loop.

---

---

## Advantages

* Dynamic size (no need to predefine length)
* Easy insertion and deletion
* Efficient memory usage compared to fixed arrays

## Disadvantages

* No direct access by index (cannot use arr[i])
* Extra memory required for storing pointers

---

## Key Takeaway

👉 **Arrays** = fast access, fixed size
👉 **Linked List** = flexible size, better for insert/delete operations
