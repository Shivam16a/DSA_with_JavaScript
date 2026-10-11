## What is Sorting in DSA?

 **Sorting** is the process of arranging data elements in a particular order, usually **ascending** or **descending** order.

 For example:

 Before sorting:\
 `5, 2, 8, 1, 3`

 After sorting in ascending order:\
 `1, 2, 3, 5, 8`

 Sorting makes it easier to **search, analyze, and organize data**.

 ## Types of Sorting Algorithms

 There are many sorting algorithms in DSA. The commonly used ones are:

 1. **Bubble Sort** – Repeatedly compares adjacent elements and swaps them if they are in the wrong order.
2. **Selection Sort** – Finds the smallest/largest element and places it in its correct position.
3. **Insertion Sort** – Takes elements one by one and inserts them into their correct position.
4. **Merge Sort** – Divides the array into smaller parts, sorts them, and then merges them.
5. **Quick Sort** – Selects a pivot and partitions the array around it.
6. **Heap Sort** – Uses a heap data structure to sort elements.
7. **Counting Sort** – Sorts elements by counting the occurrences of each value.
8. **Radix Sort** – Sorts numbers digit by digit.
9. **Bucket Sort** – Distributes elements into buckets and sorts each bucket.

 ### In short

 **Sorting = Arranging data in a specific order.**

 The **most important sorting algorithms for beginners** are **Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, and Quick Sort**.

 ## What is Hash Table
 * A **hash table** (also called a **hash map**) is a data structure used to store and retrieve data very quickly using **key–value pairs.**

```
Key       Value
"John"    25
"Alice"   30
"Bob"     22
```
A **hash function** converts each key into an index (location) in an array:

## What is Map in DSA with JavaScript

* In DSA with JavaScript, **Map** is a built-in data structure used to store key-value pairs.

In **DSA (Data Structures and Algorithms)**, a **Set** is a data structure that stores **unique values**.

 ### Example

```
const set = new Set();

set.add(10);
set.add(20);
set.add(10);

console.log(set);
```

 Output:

```
Set { 10, 20 }
```

 The second `10` is ignored because a Set **does not allow duplicates**.

 ### Important operations

```
set.add(5);       // Add
set.has(5);       // Check → true
set.delete(5);    // Remove
set.size;         // Number of elements
```

 ### Simple definition

 > **Set = a collection of unique elements.**

 In DSA, Sets are commonly used for **removing duplicates, fast lookup, finding duplicates, and checking whether an element exists**.
 
 
# Linked List in JavaScript

## Definition
A **Linked List** is a linear data structure in which elements, called nodes, are connected using references. Each node contains data and a reference to the next node.

## Example

```javascript
class Node {
  constructor(data) {
    this.data = data;
    this.next = null;
  }
}

const first = new Node(10);
const second = new Node(20);
const third = new Node(30);

first.next = second;
second.next = third;

// Traverse the linked list
let current = first;

while (current !== null) {
  console.log(current.data);
  current = current.next;
}
```

**Output:**
```text
10
20
30
```

## Types of Linked Lists

- **Singly Linked List:** Each node points to the next node.
- **Doubly Linked List:** Each node points to both the previous and next nodes.
- **Circular Linked List:** The last node points back to the first node.

## Advantages

- Dynamic size.
- Efficient insertion and deletion when the required position is known.
- Does not require contiguous memory locations.

## Disadvantages

- Extra memory is required to store references.
- Elements must be accessed sequentially.
- More complex to implement than arrays.

## Time Complexity

| Operation | Time Complexity |
|---|---|
| Access by index | O(n) |
| Search | O(n) |
| Insert at the beginning | O(1) |
| Delete from the beginning | O(1) |

## Conclusion

A linked list is useful when frequent insertions and deletions are required. Unlike arrays, linked lists do not provide direct access to elements by index.