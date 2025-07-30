## 1️⃣ Top K Frequent (Heap + HashMap)

-  [Top K Frequent Elements (LC 347)](https://leetcode.com/problems/top-k-frequent-elements/)
    
-  [Top K Frequent Words](https://leetcode.com/problems/top-k-frequent-words/)
    
-  [Sort Characters by Frequency](https://leetcode.com/problems/sort-characters-by-frequency/)
    

**Pattern:**

- Count with HashMap → Use MinHeap of size k → Extract result.
    
- Often solvable with bucket sort for linear time.
    

---

## 2️⃣ K Closest Pattern

-  [Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements/)
    
-  [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin/)
    

**Pattern:**

- Use MaxHeap to maintain k closest based on distance.
    
- Alternatively: QuickSelect or two pointers if needed.
    

---

## 3️⃣ Other Heap Patterns

-  [Task Scheduler](https://leetcode.com/problems/task-scheduler/)
    
-  [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream/)
    
-  [Furthest Building You Can Reach](https://leetcode.com/problems/furthest-building-you-can-reach/)
    
-  [Course Schedule III](https://leetcode.com/problems/course-schedule-iii/)
    
-  [Last Stone Weight](https://leetcode.com/problems/last-stone-weight/)
    
-  [The K Weakest Rows in a Matrix](https://leetcode.com/problems/the-k-weakest-rows-in-a-matrix/)
    

**Pattern Notes:**

- Task Scheduler → Use MaxHeap for frequency-based greedy scheduling.
    
- Find Median → Two heaps (MaxHeap + MinHeap).
    
- Furthest Building → MinHeap to track bricks usage efficiently.
    
- Course Schedule III → Greedy + MaxHeap on durations.
    
- Last Stone Weight → MaxHeap for repeated extraction and pushback.
    
- K Weakest Rows → MinHeap/MaxHeap with custom comparator.
    

---

## 4️⃣ Kth Largest/Smallest

-  [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/)
    
-  [Kth Smallest Element in a Sorted Matrix](https://leetcode.com/problems/kth-smallest-element-in-a-sorted-matrix/)
    

**Pattern:**

- Use MinHeap of size k for Kth largest.
    
- Use MaxHeap of size k for Kth smallest if needed.
    
- Alternatively: QuickSelect for O(n) expected time.
    

---

## 🚀 Additional High-Quality Reference

- [Java 6ms Beats 95%: HashMap + PriorityQueue (min/max heap) explanation](https://leetcode.com/problems/top-k-frequent-words/discuss/2773643/java-6ms-beats-95-with-explanation-hashmap-priorityqueue-min-max-heap-solution)
    

---

## ✨ Usage

✅ **Review these patterns before contests.**  
✅ Systematically clear the list to **solidify heap intuition**.  
✅ Practice implementing from scratch to understand the mechanics of `heapq`, `PriorityQueue`, or custom heap comparisons.

---

If you need:

✅ A **7-day structured heap mastery challenge**  
✅ An **Obsidian/CSV Kanban for systematic tracking**  
✅ Or **concise intuition summaries for each pattern**

let me know anytime for your structured deepening on **heaps & priority queues**.

Ask ChatGPT