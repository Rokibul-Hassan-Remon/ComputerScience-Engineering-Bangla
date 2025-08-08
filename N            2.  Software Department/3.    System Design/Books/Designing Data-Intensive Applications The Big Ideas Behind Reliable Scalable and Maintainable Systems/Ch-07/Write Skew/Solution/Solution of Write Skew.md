## ✅ সমাধানের দুটি উপায়:

### 1. **Serial Execution (Single-threaded Processing)**

- সব transaction একটার পর একটা হবে, একসাথে একাধিক নয়।
    
- অর্থাৎ, একই সময়ে কেবল **একটি transaction চলবে**, বাকিরা **queue-তে অপেক্ষা** করবে।
    
- একে বলা যায় **single-threaded বা strict serial execution**।
    
- এটি নিশ্চিত করে যে কেউ read করার পর অন্য কেউ তার আগে write করতে পারবে না।
    

✅ সহজ কিন্তু ধীর।  
❗ Scalability কম।

---

### 2. **Explicit Lock on Read Rows**

- শুধু যেই row-টি write করা হবে, সেটাতে নয় —  
    বরং **যেই row-গুলো transaction-টি read করছে**, সেগুলোতেও **lock নিতে হবে**।
    

📌 কারণ:

> যেই row আমরা read করেছি — ভবিষ্যতে সেটি পরিবর্তিত হতে পারে। তাই যদি আমরা সেই row-এ lock না নিই, অন্য কেউ সেটি modify করে দিলে inconsistent অবস্থা তৈরি হবে।

🛡️ উদাহরণ:

- যদি **transaction টি Alice ও Bob এর row দেখে** এবং সিদ্ধান্ত নেয়,
    
- তাহলে শুধু Alice বা Bob যার row-এ update করবে সেটাতে নয়,
    
- **উভয়ের row-এ lock নেওয়া উচিত**।
    

✅ এটি concurrency বজায় রেখে consistency রক্ষা করে।  
❗ কিন্তু একটু বেশি জটিল হতে পারে।

---

## 🧠 লেখকের মন্তব্য (DDIA অনুযায়ী):

> ❗ **Write Skew সমস্যাকে সম্পূর্ণরূপে প্রতিরোধ করতে হলে "True Serializable Isolation" দরকার।**

- Serializable isolation নিশ্চিত করে যে সব transaction এমনভাবে চলবে যেন তারা **serially** চালানো হয়েছে — যদিও বাস্তবে concurrently চলেছে।
    

---

## 📝 সংক্ষেপ:

| পদ্ধতি                     | কাজের ধরন                                        | ভালো দিক             | খারাপ দিক             |
| -------------------------- | ------------------------------------------------ | -------------------- | --------------------- |
| 1️⃣ Serial Execution       | একসাথে কেবল একটিই চলবে                           | সহজ, নিরাপদ          | ধীর, scale করা কঠিন   |
| 2️⃣ Lock Read Rows         | যেই rows read করা হয়েছে সেগুলোতেও lock           | concurrency + safety | জটিলতা বেশি           |
| 3️⃣ Serializable Isolation | ডেটাবেজ নিজেই serial execution-এর মতো behave করে | safest option        | performance কমতে পারে |
|                            |                                                  |                      |                       |
