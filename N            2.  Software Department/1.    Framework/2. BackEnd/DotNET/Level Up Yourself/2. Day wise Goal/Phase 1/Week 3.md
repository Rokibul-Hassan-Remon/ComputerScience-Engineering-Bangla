# ✅ Week 3 – Goal: ASP.NET Core Deep Dive

**Outcome at end of Week 3:**  
✅ ASP.NET Core request pipeline 100% বোঝো  
✅ Middleware তৈরি ও customize করতে পারো  
✅ Routing + Model Binding internal কাজ বোঝো  
✅ MVC থেকে API migration সহজে করতে পারো  
✅ Real-world project-ready backend confidence

---

# ✅ Weekly Topics Breakdown (High-level)

|Day|Topic|Focus|
|---|---|---|
|Day 1|ASP.NET Core Architecture Overview|Program.cs, Startup.cs, Hosting, ServiceProvider|
|Day 2|Middleware Basics|What is middleware, order, request/response flow|
|Day 3|Custom Middleware|Writing custom middleware, Use vs UseMiddleware|
|Day 4|Routing Basics|Endpoint routing, Attribute vs Conventional routing|
|Day 5|Model Binding & Validation|How ASP.NET binds data, custom model binders, validation attributes|
|Day 6|Filters in ASP.NET Core|ActionFilter, ResourceFilter, ExceptionFilter, AuthorizationFilter|
|Day 7|Mini Project + Self Test|Small API project with Middleware, Routing, Model Binding, Filters|

---

# ✅ Day-by-Day Detailed Plan

### **Day 1 (2-3 hours)**

**Topic:** ASP.NET Core Architecture Overview  
**Learn:**

- Program.cs vs Startup.cs (Hosting Model)
    
- IWebHostBuilder, HostBuilder
    
- Dependency Injection in ASP.NET Core
    
- Service lifetimes (Transient, Scoped, Singleton)
    
- Request pipeline flow (Request → Middleware → Controller → Response)
    

**Resources:**

- YouTube: Nick Chapsas – ASP.NET Core Architecture
    
- Docs: Microsoft – ASP.NET Core fundamentals
    

**Practice:**

- Create empty ASP.NET Core app
    
- Add simple controller and service via DI
    

---

### **Day 2 (2-3 hours)**

**Topic:** Middleware Basics  
**Learn:**

- What middleware is and why it matters
    
- Built-in middleware: UseRouting, UseAuthentication, UseAuthorization
    
- Middleware order importance
    
- Terminal middleware
    

**Practice:**

- Add console logging middleware
    
- Observe request-response flow with breakpoints
    

---

### **Day 3 (2-3 hours)**

**Topic:** Custom Middleware  
**Learn:**

- Create custom middleware class
    
- Use `Invoke` or `InvokeAsync`
    
- Inject services into middleware
    
- Use vs UseMiddleware differences
    

**Practice:**

- Create middleware to log request time
    
- Create middleware to block requests conditionally
    

---

### **Day 4 (2-3 hours)**

**Topic:** Routing Basics  
**Learn:**

- Conventional routing (`MapControllerRoute`)
    
- Attribute routing (`[Route("api/[controller]")]`)
    
- Route constraints & defaults
    
- Route order and conflicts
    

**Practice:**

- Add multiple controllers
    
- Apply attribute routing
    
- Test route conflicts and resolution
    

---

### **Day 5 (2-3 hours)**

**Topic:** Model Binding & Validation  
**Learn:**

- How ASP.NET Core binds JSON, query, form, route data
    
- Custom model binders
    
- Validation attributes (`[Required]`, `[Range]`, `[EmailAddress]`)
    
- ModelState.IsValid usage
    

**Practice:**

- Create POST API
    
- Validate input using attributes
    
- Test invalid input → proper response
    

---

### **Day 6 (2-3 hours)**

**Topic:** Filters in ASP.NET Core  
**Learn:**

- ActionFilter, ResourceFilter, ExceptionFilter, AuthorizationFilter
    
- Global vs Controller vs Action filters
    
- How filters integrate with middleware
    

**Practice:**

- Add ExceptionFilter for global error handling
    
- Add ActionFilter for logging execution time
    
- Add AuthorizationFilter for role-based check
    

---

### **Day 7 (2-3 hours)**

**Mini Project:** Simple API with Middleware + Routing + Filters + Model Binding

**Requirements:**

- 2 controllers (Product, Order)
    
- Logging middleware (request/response)
    
- ExceptionFilter globally
    
- POST & GET endpoints
    
- Model validation
    
- Attribute + Conventional routing mix
    

**Self-Test Checklist:**

- Can I explain ASP.NET Core request pipeline?
    
- Can I write custom middleware?
    
- Can I implement proper routing + model binding?
    
- Can I add filters for logging & error handling?
    
- Am I ready for Week 4 → MVC → Web API migration?
    

---

# ✅ Bonus / Recommended Resources (Week 3)

- **Book:** ASP.NET Core in Action (Second Edition) – Chapters on Pipeline + Middleware + Routing
    
- **YouTube:** Nick Chapsas – Middleware & Routing in depth
    
- **Docs:** Microsoft – ASP.NET Core Fundamentals