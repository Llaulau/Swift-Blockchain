# Swift-Blockchain

This code is implementing a basic blockchain system using Swift. It defines various classes and protocols to represent different components of a blockchain.

The SmartContract protocol defines a method apply(transaction:) that applies certain rules to a transaction, such as calculating fees.

The TransactionTypeSmartContract class is a specific implementation of the SmartContract protocol that calculates fees based on the type of the transaction (domestic or international).

The TransactionType enum represents the types of transactions that can be made in this blockchain.

The Transaction class represents a single transaction with its from and to addresses and the amount of the transaction.

The Block class represents a block in the blockchain. It contains an index, previous hash, hash, nonce, and a list of transactions. It also has a method to generate the key for the block and another method to add a new transaction to the block.

The Blockchain class represents the entire blockchain. It contains a list of blocks, a list of smart contracts, and methods to add a block to the blockchain and get the next block in the chain. It also has a method to generate a hash for a given block.

Finally, there is a String extension that defines a method sha1Hash() that returns the SHA-1 hash of a string.

At the end of the code, a genesis block is created, followed by a blockchain object initialized with the genesis block. A single transaction is created and added to the blockchain, and the blockchain is printed as a JSON string.
