# OP_RETURN_202
:::info
**Opcode number:** 202  
**Byte representation:**  `0xca`  
**Short description:** Fail the script immediately.
:::

`OP_RETURN_202` fails the script immediately, but it must be executed (for example it does not render a script invalid if it is in a branch of an if/else statement that doesn't get executed). It is a synonym for [OP_RETURN](./OP_RETURN.md).

`OP_RETURN_202` is part of a group of opcodes that are not defined directly in bitcoin core, (the `OP_RETURN_202` name comes from [rust-bitcoin](https://docs.rs/bitcoin/latest/src/bitcoin/blockdata/opcodes.rs.html)). Those opcodes are [`OP_RETURN_187`](./OP_RETURN_187.md) to [`OP_RETURN_254`](./OP_RETURN_254.md), and all render a script invalid if executed. This means that they essentially behave like [OP_RETURN](./OP_RETURN.md), but their use would make a script non-standard, and therefore a transaction that would include one of them would not be relayed by nodes by default.