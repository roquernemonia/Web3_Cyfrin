## Concepts

+ `Blockchain` - Bitcoin was one of the first protocols to use this revolutionary technologies called Blockchain. The Bitcoin white paper written by Satoshi Nakamoto, outlined how Bitcoin can make peer-to-peer transactions in a decentralized network. This network was powered by cryptography and decentrality. People were able to make transactions without any censorchip or control from a central authority. Due to its features, people started using it as a superior digital store of value (a better store of value over something like Gold). Thats'y people also refer to Bitcoin as Digital Gold. Similar to Gold, there is a limited amount of Bitcoin available on the planet.

    Few years after the Bitcoin whitepaper was released, Vitalik Buterin released a whitepaper on a protocol called Ethereum, which allowed people to not only make decentralized transactions but also decentralized agreements, organizations etc.

+ `Smart Contracts` - A smart contract is an agreement (a set of instructions) deployed on a decentralized blockchain. Once a smart contract is deployed, it **cannot be altered (immutable)**, is **automatically executed** and **everyone can view** the terms of the agreement / contract. The code execution is done by a group of people, so no single entity can alter the terms of the agreement.

    > In case of traditional contracts, whoever owns the contract can switch off the contract. But this cannot be done in case of smart contracts.

    Smart Contracts are like unbreakable promises and are also called `Trust Minimized Agreements`.

+ `Oracle` - Suppose a smart contract, needs **data from the real world**. But they themselves cannot interact with the internet and fetch data. So to solve this problem we have oracles. Oracles bridge the gap between the internet and the blockchain. Example of an oracle is - [Chainlink](https://chain.link/). Like the blockchain, oracles can be decentralized too which keeps our applications **truly decentralized**.

    > The combination of onchain decentralized logic and offchain oracles gives rise to `hybrid smart contracts`.

+ `Dapp` - Dapp stands for Decentralized Application. A Decentralized Application is usually a collection of smart contracts.

+ `EIP and ERC` - EIP stands for **Ethereum Improvement Protocol** and represents a proposal which can enhance the behaviour of the Ethereum blockchain. Once an EIP gets enough attention, it is standardized by creating an ERC. ERC stands for `Ethereum Request for Comments`. One such ERC is **ERC-20**. ERC-20 speaks about how tokens should be created using smart contracts. You can read more about ERC20 here - https://ethereum.org/en/developers/docs/standards/tokens/erc-20/.

+ `DAO(Decentralized Autonomous Organization)` - DAO represents a group that is governed by a set of rules represented by a smart contract. Example of DAO which is a DeFi platform. Now if the Compound maintainers want to do any kind of change to the platform, they need to create a `proposal` here - https://compound.finance/governance. Here is one such proposal - https://compound.finance/governance/proposals/141. The proposal creator **needs to perform a transaction** to create that proposal. After the proposal is created, it becomes active after some time and the platform users can then start voting for or against the proposal. After some time, based on the voting result, the proposal is **failed** or is **succeded and is queued for execution**. If the proposal is queued, it is then implemented.
    > Sometimes along with the voting system, a discussion hub is also present.

    The architecture of voting mechanism is crucial. There can be 2 types of voting mechanism :

    - **Onchain voting** - The voter needs to call a vote function from a smart contract and send a signed transaction. But in case of onchain voting, the cost of the process becomes soo high because of the gas consumed during sending the signed transactions. To solve this problem, there is a method called `Governer C`.

    - **Offchain voting** - In this case, we sign the transaction, but we dont send it to the blockchain. Instead we **store the signed transactions in a decentralized database like IPFS**. Then we count the votes and deliver the result to the blockchain using a decentralized system of oracles. So throughout the voting process, the number of transactions sent to the blockchain is just 1. This mechanism saves lots of gas and also gives a more efficient way to store the voting transactions.

    The voting mechanism can also be broken down to subtypes from different perspectives.

    

+ `NFTS (Non Fungible Tokens)` - NFTs (also known as `ERC721s`) are a token standard created on the Ethereum platform. **They are unique and not interchangeable (unlike USD or Eth)**. Currently, they are mostly represented as digital pieces of art that have a permanent history of who has deployed and owned them.

    NFTs are deployed to smart contract platforms and then can be viewed and traded in NFT platforms / marketplaces like `Opensea` (note - they can also be viewed and traded without the help of these NFT marketplaces).

+ `IPFS (Inter Planatery File System)` - IPFS is `a distributed decentralized data storage system`, that is not exactly a blockhain system but is similar to a blockchain system.

    Our IPFS node hashes our data to get a unique hash. The hash is then linked to the data. Every IPFS node in the planet has the same hashing function. The IPFS node then hosts the data mapped to the unique hash.

    Our IPFS node is connected to a massive network of other IPFS nodes. The hash and the data gets replicated to some of those other IPFS nodes.

    An IPFS node is very lightweight compared to a blockchain node, since it supports only data storage and not any smart contract execution. Each IPFS node can choose which data it will replicate. So an IPFS node can be of size few MBs to several TBs or more.

    Now what if, no other IPFS node has replicated the data hosted in our IPFS node? We can use [Pinata cloud](https://www.pinata.cloud) - a service which will replicate our host our data, so that it remains available, even when our IPFS node goes down.

