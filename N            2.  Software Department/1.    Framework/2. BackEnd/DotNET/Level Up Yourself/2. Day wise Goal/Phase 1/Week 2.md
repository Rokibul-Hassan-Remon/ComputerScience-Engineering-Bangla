# ✅ Week 2 – Goal: Advanced C# Backend Mastery

**Outcome at end of Week 2:**  
✅ Async/Await, Task, Threading বোঝো → scalable, non-blocking code লিখতে পারো  
✅ LINQ master → database + collection query efficient করা পারো  
✅ IEnumerable vs IQueryable difference বুঝো → EF Core/Performance optimization সম্ভব  
✅ Deferred execution বুঝো → Lazy loading এর জন্য critical  
✅ Ready for Week 3 → ASP.NET Core Pipeline + Middleware

---

# ✅ Weekly Topics Breakdown (High-level)

|Day|Topic|Focus|
|---|---|---|
|Day 1|Async/Await basics|Task, async method, await keyword, deadlock concept|
|Day 2|Task Parallel Library (TPL)|Task.Run, Task.WhenAll, Task.WhenAny, Continuation|
|Day 3|LINQ basics & Query syntax|Filtering, Projection, Aggregate, Sorting|
|Day 4|LINQ Advanced + Deferred execution|IQueryable vs IEnumerable, Lazy evaluation|
|Day 5|Threading basics|Thread vs Task, ThreadPool, Synchronization basics|
|Day 6|Combining Async + LINQ + Threading|Practice real scenario: Async DB call simulation|
|Day 7|Mini Project + Self Test|Combine all learned → small library / service|

---

# ✅ Day-by-Day Detailed Plan

### **Day 1 (2-3 hours)**

**Topic:** Async/Await Basics  
**Learn:**

- Task class, async method signature
    
- await keyword, non-blocking call
    
- async void vs async Task
    
- Common deadlocks + how to avoid  
    **Resources:**
    
- YouTube: Nick Chapsas “Async Await Deep Dive”
    
- Docs: Microsoft – Async/Await in C#  
    **Practice:**
    
- Create a console app simulating multiple web requests asynchronously
    
- Compare synchronous vs asynchronous execution time
    

---

### **Day 2 (2-3 hours)**

**Topic:** Task Parallel Library (TPL)  
**Learn:**

- Task.Run, Task.Factory.StartNew
    
- Task.WhenAll vs Task.WhenAny
    
- Continuation (ContinueWith)  
    **Practice:**
    
- Launch multiple CPU-bound tasks using Task.Run
    
- Combine results using Task.WhenAll
    
- Error handling in multiple tasks
    

---

### **Day 3 (2-3 hours)**

**Topic:** LINQ Basics & Query Syntax  
**Learn:**

- IEnumerable + LINQ methods: Where, Select, OrderBy, GroupBy
    
- Aggregate, Sum, Count, FirstOrDefault, SingleOrDefault  
    **Practice:**
    
- Create a List<Product>
    
- Filter, sort, and group using LINQ
    
- Compare Query syntax vs Method syntax
    

---

### **Day 4 (2-3 hours)**

**Topic:** LINQ Advanced + Deferred Execution  
**Learn:**

- IQueryable vs IEnumerable → EF Core importance
    
- Deferred vs Immediate Execution
    
- Projection, Joins, Nested Collections  
    **Practice:**
    
- LINQ on List and LINQ to EF Core simulation (use in-memory DB)
    
- Check deferred execution using breakpoints / Console.WriteLine
    

---

### **Day 5 (2-3 hours)**

**Topic:** Threading Basics  
**Learn:**

- Thread vs Task
    
- ThreadPool
    
- Locks, Monitor, Mutex (basic understanding)  
    **Practice:**
    
- Simple multi-threaded console app
    
- Increment shared counter with and without lock → observe race condition
    

---

### **Day 6 (2-3 hours)**

**Topic:** Combining Async + LINQ + Threading  
**Practice Scenario:**

- Simulate async DB call returning product list
    
- Use LINQ to filter + sort
    
- Task.WhenAll multiple async calls
    
- Bonus: Try small deadlock scenario and resolve
    

---

### **Day 7 (2-3 hours)**

**Mini Project:** Async + LINQ + Threading Library  
**Requirements:**

- Async fetch simulation (can use Task.Delay)
    
- LINQ query to filter and sort results
    
- Thread-safe counter or cache
    
- Unit Test using xUnit for async method correctness
    

**Self-Test Checklist:**

- Can I explain async vs sync?
    
- Can I describe IEnumerable vs IQueryable?
    
- Can I demonstrate deferred execution?
    
- Can I launch multiple tasks and handle results?
    
- Can I avoid deadlocks in async code?
    

---

# ✅ Bonus / Recommended Resources (Week 2)

- **Book:** C# in Depth – Async/Await chapters (Jon Skeet)
    
- **YouTube:** Nick Chapsas – Async Await + TPL
    
- **Article:** Microsoft Docs – IEnumerable vs IQueryable, Deferred Execution
    
- **Practice:** LeetCode – Easy/Medium LINQ + Async simulation problems
    

---

# 🎯 Week 2 Outcome:

- তুমি এখন **High-Performance Backend Developer**
    
- EF Core + API + Async + LINQ + Threading ready
    
- Ready for **Week 3 → ASP.NET Core Middleware + Pipeline deep dive**
    
- Real-world project-ready mindset শুরু হয়েছে