```cs title:"Sanitize the Html attributes"
using Ganss.XSS;

var sanitizer = new HtmlSanitizer();
sanitizer.AllowedTags.Clear();

sanitizer.AllowedTags.Add("b");
sanitizer.AllowedTags.Add("i");
sanitizer.AllowedTags.Add("em");
sanitizer.AllowedTags.Add("strong");
sanitizer.AllowedTags.Add("p");
sanitizer.AllowedTags.Add("br");

string safeHtml = sanitizer.Sanitize(userInput);

```

## 2️⃣ Rich text input (Comment / Post / Description)

এই জায়গাগুলোতে **HtmlSanitizer MUST**
```cs title:"How to sanitize the user Input"

public string SanitizeHtml(string input)
{
    var sanitizer = new HtmlSanitizer();

    sanitizer.AllowedTags = new HashSet<string>
    {
        "b","i","u","em","strong","p","br","ul","ol","li"
    };

    sanitizer.AllowedAttributes.Clear();

    return sanitizer.Sanitize(input);
}

```