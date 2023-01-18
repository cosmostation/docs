---
sidebar_position: 3
description: Using Cosmostation Extension accounts
---

# Accounts



## Get Accounts

### Code using @cosmostation/extension-client

```javascript
const account = await provider.getAccount("cosmoshub-4");
```

### Vanilla Code

```javascript
const accoutn = await window.cosmostation.cosmos.request({
  method: "cos_account",
  params: { chainName: "cosmoshub-4" },
});
```

> #### If connected successfully, it will look like below.
>
> <img src="../../../img/developer/extension/2-provider-connected.png" alt="Provider" data-size="original">

#### Response

```typescript
type AccountResponse = {
  name: string;
  address: string;
  publicKey: Uint8Array;
  isLedger: boolean;
};
```

```json
{
  "name": "account name",
  "address": "cosmos1wgeoiheoighwoighwioeghoweghoiweghiow",
  "publicKey": [
    3, 77, 9, 189, 251, 249, 150, 235, 192, 56, 51, 98, 56, 242, 12, 102, 144,
    211, 89, 42, 187, 170
  ],
  "isLedger": false
}
```

## Request Account (Popup)

### Code using @cosmostation/extension-client

```typescript
try {
  // ...
  const account = await provider.requestAccount("cosmoshub-4");
} catch (e) {
  if (e instanceof InstallError) {
    console.log("not installed");
  }

  if (e.code === 4001) {
    console.log("user rejected request");
  }

  // exception
}
```

### Vanilla Code

```javascript
const accoutn = await window.cosmostation.cosmos.request({
  method: "cos_requestAccount",
  params: { chainName: "cosmoshub-4" },
});
```

#### Response

```typescript
type RequestAccountResponse = {
  name: string;
  address: string;
  publicKey: Uint8Array;
  isLedger: boolean;
};
```

```json
{
  "name": "account name",
  "address": "cosmos1wgeoiheoighwoighwioeghoweghoiweghiow",
  "publicKey": [
    3, 77, 9, 189, 251, 249, 150, 235, 192, 56, 51, 98, 56, 242, 12, 102, 144,
    211, 89, 42, 187, 170
  ],
  "isLedger": false
}
```
