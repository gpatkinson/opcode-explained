# Transaction Validation

Bitcoin validation relies on two general types of scripts:
1. **locking script** - the criteria that must be met in order to spend a UTXO
2. **unlocking script** - the script that satisfies the locking script, typically a cryptographic signagure
    
These script types are used together in transaction validation:

>Every bitcoin validating node will validate transactions by executing the locking and unlocking scripts together. Each input contains an unlocking script and refers to a previously existing UTXO. The validation software will copy the unlocking script, retrieve the UTXO referenced by the input, and copy the locking script from that UTXO. The unlocking and locking script are then executed in sequence. The input is valid if the unlocking script satisfies the locking script conditions ... All the inputs are validated independently, as part of the overall validation of the transaction.

## References

1. Antonopoulos, Andreas M. [_Mastering Bitcoin: Programming the Open Blockchain_](https://github.com/bitcoinbook/bitcoinbook). 2nd Ed, O'Reilly, 2017.
   
