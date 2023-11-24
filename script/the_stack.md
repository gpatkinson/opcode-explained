# The Stack

Script's stack allows for only two operations: push and pop. 
- push adds something to the top of the stack
- pop removes an item from the top of the stack. 

As you may have noticed, only the top item from the stack can be manipulated.

All of the opcodes listed on this website are specific variants of these two operations. For example, [OP_ADD](/opcodes/OP_ADD.md) pops two consecutive items from the stack, adds them together, and then pushes the result to the stack. Opcodes are the fundamental building blocks of transactions and, in various combinations, represent the full expressivity of the Bitcoin network. From time-to-time, [new opcodes are proposed](https://github.com/jamesob/bips/blob/jamesob-23-02-opvault/bip-0345.mediawiki) to give Bitcoin more capabilities. 
