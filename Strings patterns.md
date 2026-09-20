## 🧵 Strings

> Sequence of characters and common string manipulation patterns.

This category covers two core patterns that show up repeatedly in string problems: **Two-Pointer** techniques for symmetric/palindrome-style checks, and **Sliding Window** techniques for substring/subarray optimization.

---

### 🔁 Two-Pointer (Palindrome)

- **What it is:** Uses two indices — typically starting from both ends of the string (or array) and moving inward — to compare, swap, or validate elements symmetrically. Ideal for problems involving mirrored structure or in-place reversal.
- **How to solve it:** Initialize `left = 0` and `right = length - 1`. Move both pointers toward the center, comparing or modifying characters at each step, and stop when they meet or cross. Handle edge cases like case-sensitivity, spaces, and non-alphanumeric characters before comparing.

**Example problems:**
- [125. Valid Palindrome](https://leetcode.com/problems/valid-palindrome/)
- [5. Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)
- [680. Valid Palindrome II](https://leetcode.com/problems/valid-palindrome-ii/)
- [344. Reverse String](https://leetcode.com/problems/reverse-string/)

---

### 🪟 Sliding Window (String)

- **What it is:** Maintains a "window" (a contiguous substring) defined by two pointers that expand or shrink dynamically based on a condition — commonly used for problems mentioning *longest*, *shortest*, *substring*, *at most K*, or *exactly K*.
- **How to solve it:** Expand the window by moving the `right` pointer and updating a frequency map/count as you go. When the window violates the condition, shrink it by moving the `left` pointer until it's valid again, tracking the best result along the way.

**Example problems:**
- [3. Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)
- [76. Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/)
- [438. Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string/)
- [340. Longest Substring with At Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/)
