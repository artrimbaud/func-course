
# Concept of Contracts and Accounts

###### tags: `Chapter 1`

**Account as Smart Contract**
- Accounts are smart contracts on TON, serving multiple purposes beyond fund storage.
- Various entities, including tokens, are also implemented as smart contracts.
- Contracts serve as low-level building blocks.

**Understanding Contracts**
- Contracts have their own state: code, data, and Toncoin balance.
- Identity is established via secure cryptographic addresses derived from initial code and data.
- Contracts process messages, emit messages, and transform state.

**Contract Functions**
- Wallet contracts manage Toncoins and assets, verifying signatures and forwarding messages.
- Token contracts handle transfers via messages containing logic for ownership changes.

**TON Blockchain and Token Balances**
- TON doesn't track token balances directly; contracts communicate through messages.
- Users attribute meaning to contracts, valuing tokens based on ownership.

**Execution Cost and Risks**
- Contracts pay for execution with gas fees, impacting their balance.
- Expensive operations consume more balance; insufficiency leads to failed operations.
- Money is deducted from the balance and used as transaction fees.

**Rent Payment for Storage**
- Contracts pay rent for storage, based on data size and time.
- Regular funding required for long-term tokens like stablecoins.
- Ensuring contract's balance avoids potential pitfalls.

**Token Strength and Scalability**
- Long-term tokens need continuous funding to remain operational.
- Strong tokens ensure scalability and protection against denial of service.
