# ✅ Phase 1 – Week 1

## 🎯 Goal: C# Deep Dive (Advanced Language Features)

👉 এই সপ্তাহ শেষে তুমি C# কে শুধু syntax হিসেবে না, language হিসেবে ভিতর থেকে বুঝবে।  
👉 এটাই তোমার future architecture, performance, clean code, interview–সবকিছুর ফাউন্ডেশন।

---

# ✅ Weekly Topics Breakdown (High-level)

✅ Day 1-2: Value vs Reference Types + Memory (Stack vs Heap)  
✅ Day 3: Struct, Record, Tuple, Anonymous types  
✅ Day 4: Delegates, Func, Action, Predicate, Lambda  
✅ Day 5: Extension Methods + Partial classes + Indexers  
✅ Day 6: Nullable Reference Types + Nullability Handling + ?. ?? ??=  
✅ Day 7: Recap + Mini Practice + Self Test

**Now full Day-by-Day plan with exact tasks, resources, practice!**

---

# ✅ Day 1 (2-3 hours)

### 🎯 Topic: Value Type vs Reference Type + Stack vs Heap

**Why?** Performance, boxing/unboxing, memory optimization বুঝতে হবে।

### ✅ What to Learn:

- CLR কীভাবে memory manage করে
    
- Stack কী? Heap কী?
    
- Value type কোথায় store হয়?
    
- Reference type কোথায় store হয়?
    
- Boxing & Unboxing
    

### ✅ Resources:

- ✅ YouTube: “Value vs Reference Types in C# (Nick Chapsas / CodeOpinion)”
    
- ✅ Article: Microsoft Docs – Value Types vs Reference Types (official doc)
    

### ✅ Practice:

- int, string, custom class নিয়ে experiment
    
- Boxing/unboxing example code লিখো
    

---

# ✅ Day 2 (2-3 hours)

### 🎯 Topic: Immutability + string intern + StringBuilder

### ✅ What to Learn:

- string immutable কেন?
    
- string pool / intern concept
    
- String vs StringBuilder performance
    
- when to use StringBuilder
    

### ✅ Resource:

- YouTube: “String Interning in C#”
    
- Book: C# in Depth (selected topic)
    

### ✅ Practice:

- লুপে string concat vs StringBuilder test
    
- memory profiler দিয়ে difference দেখো (optional)
    

✅ **Day 1-2 শেষে Milestone Check:**  
✔ আমি Stack/Heap clear বুঝি  
✔ কেন string immutable বুঝি  
✔ value vs reference difference বুঝি

---

# ✅ Day 3 (2-3 hours)

### 🎯 Topic: Struct, Record, Tuple, Anonymous Types

✅ Struct = lightweight value type  
✅ Record = immutable reference type (C# 9+)  
✅ Tuple = lightweight grouping  
✅ Anonymous type = new { } at runtime

### ✅ Resources:

- “When to use Struct vs Class?” (YouTube / Blog)
    
- “Records in C# | Nick Chapsas”
    
- Microsoft Docs: Tuples & Records
    

### ✅ Practice:

- class vs struct performance test
    
- record vs class equality test
    
- tuple returns
    
- anonymous type usage
    

---

# ✅ Day 4 (2-3 hours)

### 🎯 Topic: Delegates + Func + Action + Lambda + Predicate

✅ এগুলো না জানলে async, event, LINQ, design pattern বুঝা যায় না।

### ✅ Learn:

- What is delegate?
    
- Func<>, Action<>, Predicate<>
    
- Lambda expression => arrow syntax
    
- Multicast delegates
    

### ✅ Resource:

- YouTube: “Delegates & Func Action Explained”
    
- Blog: Microsoft Docs – Delegates
    

### ✅ Practice:

- নিজে delegate declare করে function call করো
    
- Func<int,int,int> দিয়ে addition
    
- List filtering using Predicate
    

---

# ✅ Day 5 (2-3 hours)

### 🎯 Topic: Extension Method + Partial + Indexer + Params

✅ এগুলো তোমার code readability 10x করে দেবে।

### ✅ Learn:

- Extension method তৈরির নিয়ম
    
- Partial class split
    
- this[] indexer
    
- params keyword
    

### ✅ Resource:

- YouTube: “Extension Methods C#”
    
- Docs: “Indexer in C#”
    

### ✅ Practice:

- string.ToTitleCase() নিজের extension বানাও
    
- custom indexer class বানাও
    

---

# ✅ Day 6 (2-3 hours)

### 🎯 Topic: Nullable Reference Type (C# 8+)

✅ বাস্তব প্রজেক্টে NullReferenceException মারাত্মক সমস্যা → এটা প্রো-লেভেলে handle করতে হবে

### ✅ Learn:

- ? null-forgiving
    
- ?. null-conditional
    
- ?? null-coalescing
    
- ??= assign if null
    
- Nullable context enable in project
    

### ✅ Resource:

- Nick Chapsas: “Nullable Reference Types”
    
- Docs: Microsoft – Nullability in C#
    

### ✅ Practice:

- null সম্ভাবনা আছে এমন code rewrite করে safe করো
    

---

# ✅ Day 7 (2-3 hours)

### 🎯 Recap + Mini Project

1️⃣ Concepts revise  
2️⃣ নিজেকে test করো  
3️⃣ Write sample code combining:

- struct + record + delegate + extension method
    

✅ Mini Challenge:  
👉 Create a **“Smart Calculator Library”**

- Different operations using Func/lambda
    
- Record to store history
    
- Extension method to format result
    
- Nullable parameters safely handle
    

✅ Self-Test Questions:

- কখন struct vs class?
    
- record immutable কেন useful?
    
- Func vs Action vs Predicate?
    
- Extension method internal কীভাবে কাজ করে?
    
- string এবং StringBuilder কখন use করবো?