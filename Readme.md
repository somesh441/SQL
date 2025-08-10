Problem link: https://www.hackerrank.com/challenges/binary-search-tree-1/submissions/code/416230857

Problem Statement
Given the root node of a binary tree, determine whether it is a valid Binary Search Tree (BST). 
A tree is a BST if all nodes in the left subtree are less than the current node’s value, and all nodes in the right subtree are greater.

Approach
Define a helper function isValid(node, min, max) that ensures the current node's value is within (min, max).

Recursively verify that all left subtree nodes are < node.data and all right subtree nodes are > node.data by updating the range at each call.

If any node fails the check, return False; otherwise, return True.

Complexity
Time Complexity: O(n) — each node is visited once during traversal.

Space Complexity: O(h) — recursion stack space (h = tree height).

Code
See solution 
