---
sidebar_position: 1
description: Cosmostation extension support various chains.
---

# Provider



### Code using @cosmostation/extension-client

```typescript
import { cosmos, InstallError } from "@cosmostation/extension-client";

try {
  const provider = await cosmos();
} catch (e) {
  if (e instanceof InstallError) {
    console.log("not installed");
  }
}
```

### Vanilla Code

```javascript
window.onload = async () => {
  if (!window.cosmostation) {
    alert("Please install cosmostation extension");
  } else {
    // logic
  }
};
```
