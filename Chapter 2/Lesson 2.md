# Messages types and computation phases

###### tags: `Chapter 2`

This lesson delves into the transaction lifecycle within contract execution. It introduces the distinction between internal and external messages, where external messages originate from users and internal messages circulate within contracts. 

Transactions encompass multiple phases:

1. **Storage Phase:** Deducts storage fees based on bytes stored by the contract since the last transaction. If there are insufficient funds, the contract transitions to a frozen state, preserving its state for a limited time.

2. **Credit Phase:** Credits incoming coins from internal messages to the contract's balance. This phase highlights the difference between internal and external messages, where internal messages can carry coins.

3. **Computation Phase:** Executes the contract's code using the TVM (Ton Virtual Machine), recording side effects as actions. These actions determine the contract's behavior.

4. **Action Phase:** Processes actions, including updating the contract's state or sending outgoing messages to other contracts or shards.

5. **Bounce Phase:** If enabled by a flag in the incoming message, automatically returns incoming funds minus fees in case of contract failure. This safeguards users against unintended losses.

Additionally, it touches upon gas payments, which track the cost of operations, and the importance of setting limits to avoid running out of coins during execution.
