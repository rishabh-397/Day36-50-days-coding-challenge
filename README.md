# Day36-50-days-coding-challenge

# ✅ Problem 1: Sum of Root-to-Leaf Numbers in a Binary Tree

### 🚀 Problem Statement:
You are given a binary tree with digits (0-9). Each root-to-leaf path represents a number. Return the **sum** of all such numbers.

### 🔍 Approach:
- Use Depth First Search (DFS) to traverse the tree.
- For each root-to-leaf path, build the number by multiplying the current number by 10 and adding the node’s value.
- When a leaf node is reached, return that number.
- Accumulate the sum from all such paths.

### 🧪 Example:
Input: `[1,2,3]`  
- Path: 1→2 = 12  
- Path: 1→3 = 13  
Total = 12 + 13 = **25**

Input: `[4,9,0,5,1]`  
- Paths: 495, 491, 40 → Total = **1026**

### 🧠 Complexity:
- Time: `O(n)` — Visit each node once
- Space: `O(h)` — Height of the tree for recursive stack

---

## ✅ Problem 2: Reverse Vowels of a String

### 🚀 Problem Statement:
Given a string `s`, reverse only its vowels and return the new string.

### 🧩 Vowels to consider:
- Lowercase: a, e, i, o, u  
- Uppercase: A, E, I, O, U

### 🔍 Approach:
- Use two-pointer technique: one from start, one from end.
- When both point to vowels, swap them.
- Continue until they cross.

### 🧪 Example:
Input: `"IceCreAm"` → Vowels: [I, e, e, A] → Output: `"AceCreIm"`  
Input: `"leetcode"` → Output: `"leotcede"`

### 🧠 Complexity:
- Time: `O(n)` — Single pass through string
- Space: `O(n)` — String is immutable in Python, so we use a list
