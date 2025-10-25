# 🧩 What Is a Function in Solidity?

> A function in Solidity is a reusable block of code that performs a specific task — similar to other programming languages like JavaScript or Python.

**Functions can:**

- Read or modify the blockchain state
- Accept inputs (parameters)
- Return outputs
- Be restricted in who can call them
- Be optimized for gas or security

---

### 🧱 General Syntax

```solidity
function functionName(type parameter1, type parameter2, ...)
    visibility
    stateMutability
    returns (type returnVariable)
{
    // Function logic
}
```

### 🔍 Function Visibility

Visibility determines where the function can be called from.

| Visibility | Description                                     | Callable by               |
| ---------- | ----------------------------------------------- | ------------------------- |
| public     | Anyone and other contracts can call             | External + internal       |
| external   | Only from outside the contract                  | External only             |
| internal   | Only within this contract and derived contracts | Internal only             |
| private    | Only within this contract                       | Internal (no inheritance) |
