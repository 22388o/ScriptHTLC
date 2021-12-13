# ScriptHTLC

# Experimental Atomic Swap

Atomic swaps can be executed between many blockchains, but not all. For the scheme to work, both chains need some kind of relative timelock operation (like OP_CHECKSEQUENCEVERIFY), as well as the ability to hash a blob of data and check against a given hash. In this guide we'll be focusing on just Bitcoin and Bitcoin Cash, using the bcoin and bcash libraries respectively. It's a bit of a game: the rules can't be broken, but you still have to pay attention. The magic machine at the core of the atomic swap is called the Hash Time-Locked Contract, or HTLC.
