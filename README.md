# Blind 75: Pattern-Oriented Learning Plan for Meta L5 Interviews

This guide restructures the Blind 75 problem set around **core patterns**, enabling you to develop intuition and transferable techniques. Ideal for ** Software Engineer** interviews, the focus is on solving problems by recognizing and applying patterns, not memorizing solutions.

---

## 🧠 Hashing & Frequency Maps
**Goal**: Master lookup, counting, and grouping with hash tables.

- [Two Sum](https://leetcode.com/problems/two-sum/) – Find complements using hash map  
- [Contains Duplicate](https://leetcode.com/problems/contains-duplicate/) – Detect repeats using hash set  
- [Valid Anagram](https://leetcode.com/problems/valid-anagram/) – Count characters using hash maps  
- [Group Anagrams](https://leetcode.com/problems/group-anagrams/) – Group by sorted string hash  
- [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements/) – Frequency map + heap/bucket  

### Techniques:
- Use maps for constant-time access
- Count frequency and compare maps
- Leverage hash structure for groupings

---

## 🪟 Sliding Window
**Goal**: Dynamically track elements in a fixed or growing window

- [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) – Set + two pointers  
- [Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement/) – Max frequency window  
- [Permutation in String](https://leetcode.com/problems/permutation-in-string/) – Sliding window compare frequency  
- [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/) – Expand-contract technique with maps  
- [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) – Track min/max within a window  

### Techniques:
- Two pointers expanding/shrinking window
- Track conditions (frequency, sum, uniqueness)
- Maintain constant space within window

---

## 🧮 Two Pointers
**Goal**: Efficient linear scans with dual indices

- [3Sum](https://leetcode.com/problems/3sum/) – Sort + skip duplicates with i, l, r  
- [Container With Most Water](https://leetcode.com/problems/container-with-most-water/) – Maximize area by moving inward  
- [Valid Palindrome](https://leetcode.com/problems/valid-palindrome/) – Compare ends moving inward  
- [Remove Duplicates from Sorted Array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/) – Fast/slow pointer  

### Techniques:
- Use sorted arrays to avoid brute force
- Use relative movement based on comparisons

---

## 📚 Binary Search
**Goal**: Find targets or bounds in log(n) time

- [Binary Search](https://leetcode.com/problems/binary-search/) – Basic mid comparison  
- [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/) – Identify sorted half  
- [Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/) – Pivot-based binary search  
- [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/) – Binary search over answer space  
- [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/) – Partitioned binary search  

### Techniques:
- Search conditionally over sorted space
- Treat answer space as monotonic function

---

## 🔢 Dynamic Programming (DP)
**Goal**: Optimize overlapping subproblems via recursion/memo/tabulation

- [Climbing Stairs](https://leetcode.com/problems/climbing-stairs/) – Fibonacci bottom-up  
- [House Robber](https://leetcode.com/problems/house-robber/) – Skip or include decision  
- [Coin Change](https://leetcode.com/problems/coin-change/) – Minimum coins for total  
- [Word Break](https://leetcode.com/problems/word-break/) – DP over substring validity  
- [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence/) – DP with binary search  
- [Edit Distance](https://leetcode.com/problems/edit-distance/) – 2D DP with operations  
- [Decode Ways](https://leetcode.com/problems/decode-ways/) – Ways to decode digits  

### Techniques:
- Identify state: f(i), f(i,j), etc.
- Define transition: f(i) = f(i-1) + f(i-2), etc.
- Base case initialization

---

## 🌲 Tree Traversal (DFS, BFS)
**Goal**: Traverse and operate over tree nodes recursively or iteratively

- [Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/) – DFS count depth  
- [Invert Binary Tree](https://leetcode.com/problems/invert-binary-tree/) – Swap children recursively  
- [Same Tree](https://leetcode.com/problems/same-tree/) / [Subtree of Another Tree](https://leetcode.com/problems/subtree-of-another-tree/) – Compare structure recursively  
- [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal/) – Queue-based BFS  
- [Lowest Common Ancestor](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/) – Post-order return target match  
- [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/) – DFS/BFS encoding  

### Techniques:
- Recursive and iterative traversal
- Use base cases to prune tree recursion

---

## 🌐 Graph Traversal (DFS/BFS, Union-Find)
**Goal**: Explore or validate graph structures

- [Number of Islands](https://leetcode.com/problems/number-of-islands/) – DFS or BFS flood-fill  
- [Clone Graph](https://leetcode.com/problems/clone-graph/) – DFS with visited map  
- [Course Schedule](https://leetcode.com/problems/course-schedule/) – Topological sort + cycle detection  
- [Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow/) – DFS from ocean edges  
- [Graph Valid Tree](https://leetcode.com/problems/graph-valid-tree/) – Union-find or DFS with cycle check  

### Techniques:
- Build adjacency list
- Track visited state
- Detect cycles or reachability

---

## 🧱 Stack & Monotonic Stack
**Goal**: LIFO operations or maintain increasing/decreasing order

- [Valid Parentheses](https://leetcode.com/problems/valid-parentheses/) – Match open/close brackets  
- [Min Stack](https://leetcode.com/problems/min-stack/) – Stack with constant-time min tracking  
- [Daily Temperatures](https://leetcode.com/problems/daily-temperatures/) – Monotonic decreasing stack  
- [Car Fleet](https://leetcode.com/problems/car-fleet/) – Process in reverse with arrival times  
- [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/) – Index stack for height-area calc  

### Techniques:
- Stack of values or indices
- Track max/min/condition with each push/pop

---

## 🛠 Design / System Implementation
**Goal**: Implement core data structures with constraints

- [LRU Cache](https://leetcode.com/problems/lru-cache/) – Hash Map + Doubly Linked List  
- [Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1/) – Map + dynamic array  
- [Word Search](https://leetcode.com/problems/word-search/) – Backtracking on 2D grid  
- [Design Add and Search Word](https://leetcode.com/problems/add-and-search-word-data-structure-design/) – Trie + DFS  
- [Time-based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store/) – Hash Map + Binary Search  

### Techniques:
- Combine multiple structures for performance
- Backtracking and trie usage for dynamic queries

---

## 🎯 Learning Strategy

- Master 2–3 problems per pattern before moving to next  
- Build template solutions and pattern recognition  
- Time yourself on second pass through each pattern  
- Record time/space complexity + decisions taken  

---

