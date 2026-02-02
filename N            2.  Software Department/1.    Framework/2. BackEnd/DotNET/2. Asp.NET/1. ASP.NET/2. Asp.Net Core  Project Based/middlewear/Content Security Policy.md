
### Way - 1: 
```cs title:"CSP configuration"
app.Use(async (context, next) =>
{
    context.Response.Headers.Add(
        "Content-Security-Policy",
        "default-src 'self'; " +
        "script-src 'self'; " +
        "style-src 'self'; " +
        "img-src 'self'; " +
        "object-src 'none';"
    );

    await next();
});

```

### Way - 2:
```cs 
app.Use(async (context, next) =>
{
    await next();

    // Content Security Policy (CSP)
    context.Response.Headers["Content-Security-Policy"] =
        "default-src 'self'; " +
        "script-src 'self'; " +
        "style-src 'self'; " +
        "img-src 'self'; " +
        "object-src 'none'; " +
        "frame-ancestors 'none'; " +
        "form-action 'self';";
});
```

## `Add()` vs `Headers["key"]` – Critical difference 🔥

### ❌ `Headers.Add()`

- Header আগে থেকেই থাকলে → **Exception throw করে**
    
- Same middleware twice run হলে crash হতে পারে
    

### ✅ `Headers["key"] = value`

- থাকলে overwrite
    
- না থাকলে add
    
- **No exception**
    

📌 **Production-grade code-এ `Add()` avoid করাই best practice**
## 🧠 CSP directive বুঝে রাখো

| Directive            | মানে                 |
| -------------------- | -------------------- |
| `default-src 'self'` | সব নিজের domain থেকে |
| `script-src`         | JS কোথা থেকে         |
| `style-src`          | CSS                  |
| `img-src`            | Image                |
| `object-src 'none'`  | Flash, object block  |

## Extra Security for Cookie :
```cs title:"Extra bit of security for cookies"
// Custom Security Headers Middleware
app.Use(async (context, next) =>
{
    await next();

    // Content Security Policy (CSP)
    context.Response.Headers["Content-Security-Policy"] =
        "default-src 'self'; " +
        "script-src 'self'; " +
        "style-src 'self'; " +
        "img-src 'self'; " +
        "object-src 'none'; " +
        "frame-ancestors 'none'; " +
        "form-action 'self';";

    // Clickjacking protection
    context.Response.Headers["X-Frame-Options"] = "DENY";

    // MIME sniffing protection
    context.Response.Headers["X-Content-Type-Options"] = "nosniff";

    // Referrer policy
    context.Response.Headers["Referrer-Policy"] = "strict-origin-when-cross-origin";
});
```



