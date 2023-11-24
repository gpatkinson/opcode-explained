# Transaction Validation

The Bitcoin validation engine relies on two general types of scripts to validate transactions.
1. **locking script** (aka witness script)- this is the spending condition placed on an output, a condition that must be met to spend a given UTXO in the future.
2. **unlocking script** - script that satisfies the conditions made by the locking script.

To validate a transaction, nodes execute the locking and unlocking scripts together. First the unlocking script is executed and if executed without errors, the main stack is copied and locking script is then executed. If the end result of these operations is "TRUE", the unlocking script has satisfied the necessary conditions and the UTXO can be spent.
   
