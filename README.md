# Delete Node in a Binary Search Tree

## Problem Description

Given a root node of a **Binary Search Tree (BST)** and an integer `key`, delete the node with the given `key` from the BST.  
Return the **root node** of the BST after deletion.

The deletion process works as follows:
1. If the node to be deleted has no children, remove it directly.
2. If the node has one child, replace it with its child.
3. If the node has two children, replace its value with its **inorder successor** (the smallest value in its right subtree), and then delete that successor.

---

## Examples

### Example 1:

**Input:**  
`root = [5,3,6,2,4,null,7], key = 3`  

**Output:**  
`[5,4,6,2,null,null,7]`  

---

### Example 2:

**Input:**  
`root = [5,3,6,2,4,null,7], key = 0`  

**Output:**  
`[5,3,6,2,4,null,7]`  

---

### Example 3:

**Input:**  
`root = [], key = 0`  

**Output:**  
`[]`  

---

## Constraints

* The number of nodes in the tree is in the range `[0, 10^4]`
* `-10^5 <= Node.val <= 10^5`
* Each node has a unique value
* `root` is a binary search tree
