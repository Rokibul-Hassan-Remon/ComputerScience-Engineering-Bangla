# ✅ Week 4 – Goal: MVC → Web API + Professional API Design

**Outcome at end of Week 4:**  
✅ MVC থেকে Web API migration বুঝবে  
✅ REST API Best Practices apply করতে পারো  
✅ Routing, Versioning, Status Codes, Error Handling mastery  
✅ Global Exception Handling + Custom Response Model implement করতে পারো  
✅ Mini real-world API project ready

---

# ✅ Weekly Topics Breakdown (High-level)

|Day|Topic|Focus|
|---|---|---|
|Day 1|MVC → API Transition|Differences, ControllerBase, IActionResult|
|Day 2|REST API Best Practices|Status codes, endpoint naming, HTTP verbs|
|Day 3|API Versioning + Routing|Route prefixes, versioning strategies|
|Day 4|Model Validation & Response|DTOs, AutoMapper, Input/Output models|
|Day 5|Exception Handling|Global exception middleware, custom exceptions|
|Day 6|Security Basics for API|JWT Authentication, Role-based Authorization|
|Day 7|Mini Project|Full CRUD API with validation, exception handling, versioning|

---

# ✅ Day-by-Day Detailed Plan

### **Day 1 (2-3 hours)**

**Topic:** MVC → API Transition  
**Learn:**

- Controller vs ControllerBase
    
- IActionResult / ActionResult<T>
    
- From MVC Views → returning JSON only
    
- Attribute routing importance
    

**Resources:**

- YouTube: “ASP.NET Core MVC vs API – Nick Chapsas”
    
- Docs: Microsoft – Web API fundamentals
    

**Practice:**

- Convert existing MVC CRUD app → API only (ControllerBase)
    
- Replace ViewResult with IActionResult / JsonResult
    

---

### **Day 2 (2-3 hours)**

**Topic:** REST API Best Practices  
**Learn:**

- HTTP verbs (GET, POST, PUT, PATCH, DELETE)
    
- Resource-based endpoints
    
- Proper status codes (200, 201, 204, 400, 404, 500)
    
- Query params, filtering, pagination basics
    

**Practice:**

- Refactor API endpoints to follow resource naming
    
- Add proper status codes for each action
    
- Implement simple pagination & filtering
    

---

### **Day 3 (2-3 hours)**

**Topic:** API Versioning + Routing  
**Learn:**

- Route prefixing (e.g., /api/v1/products)
    
- Microsoft.AspNetCore.Mvc.Versioning
    
- Attribute routing for versioned endpoints
    
- Backward compatibility concept
    

**Practice:**

- Create v1 and v2 of ProductController
    
- Add minor change in v2 (new field / output model)
    
- Test both endpoints
    

---

### **Day 4 (2-3 hours)**

**Topic:** Model Validation + DTOs + AutoMapper  
**Learn:**

- DTO (Data Transfer Object) concept
    
- AutoMapper setup and usage
    
- FluentValidation (optional)
    
- ModelState.IsValid + custom response structure
    

**Practice:**

- Create ProductDTO
    
- Map between Entity ↔ DTO
    
- Add validation attributes + return consistent error response
    

---

### **Day 5 (2-3 hours)**

**Topic:** Exception Handling  
**Learn:**

- Global exception handling middleware
    
- Custom exceptions (NotFound, BadRequest, ValidationError)
    
- Logging exceptions (Serilog optional)
    

**Practice:**

- Implement global exception middleware
    
- Throw custom exceptions in service layer
    
- Return uniform API response for errors
    

---

### **Day 6 (2-3 hours)**

**Topic:** Security Basics for API  
**Learn:**

- JWT Authentication setup
    
- Role-based Authorization
    
- Policy-based Authorization concept
    
- Secure endpoints
    

**Practice:**

- Protect GET/POST endpoints with JWT
    
- Add Admin/User role restriction
    
- Test unauthorized requests
    

---

### **Day 7 (2-3 hours)**

**Mini Project:** Professional Product API  
**Requirements:**

- CRUD for Product
    
- DTO + AutoMapper
    
- Validation
    
- Versioned endpoints (v1 & v2)
    
- Global Exception Handling
    
- JWT secured endpoints (Admin vs User)
    

**Self-Test Checklist:**

- Can I migrate MVC → API confidently?
    
- Can I design RESTful endpoints?
    
- Can I implement versioning + proper status codes?
    
- Can I handle exceptions globally?
    
- Can I secure API with JWT & roles?
    

---

# ✅ Bonus / Recommended Resources (Week 4)

- **Book:** ASP.NET Core in Action – Chapters on Web API
    
- **YouTube:** Nick Chapsas – REST API + JWT + Versioning
    
- **Docs:** Microsoft – API Controllers, Versioning, Model Validation
    

---

# 🎯 Week 4 Outcome:

- তুমি এখন **Junior → Mid-level API Developer**
    
- Real-world API standards, security, exception handling সব ready
    
- Ready for **Week 5 → EF Core Deep Dive + Performance Optimization + Advanced Queries**