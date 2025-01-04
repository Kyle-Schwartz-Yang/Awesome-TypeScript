---
tags:
  - aliases
  - Aliases
  - type_aliases
---
---
- Тепер є можливість зберегти перебір [[Union Types]] у зміну 
- Це и буде мати назву [[Type Aliases]]
---
```typescript
  type Status = "success" | "error" | "loading";

    function checkStatus(status: Status) {
      // status может быть только "success", "error", или "loading"
    }
```

> 📌 Type Aliases доступні тільки в момент розробки та будуть видалені при компеляції 💡
