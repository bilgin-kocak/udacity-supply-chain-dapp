
#  Ethereum Dapp for Tracking Items through Supply Chain
This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

## Project write-up - UML

### Activity
![Activity](UML/activity-diagram.jpg)

### Sequence
![Sequence](UML/sequence-diagram.jpg)

### State
![State](UML/state-diagram.jpg)

### Classes (Data Model)
![Data-Model](UML/data-model-diagram.jpg)

## Project write-up - Libraries
The `Roles` library was used by different access control contracts for easy add and remove in the supply chain 
`truffle-hd-wallet-provider` to sign transactions for addresses.

## IPFS
IPFS is not used in this project

## Program Versions numbers
Node: v14.15.4
Solidity: v0.4.24
Truffle: v5.0.25
Web3.js: v1.0.0-beta37 

## Contract address on the Rinkeby test network (Etherscan):
https://rinkeby.etherscan.io/address/0xD30c6d4B48050a901c23c53Fca5BEd56253E2b14



1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0x9ff9f22fd0c5f95074212fe16009a7388fa4b2859c2e0568e33e721ae13f329b
   > Blocks: 1            Seconds: 4
   > contract address:    0x2d22594634Eb614fC542C0BE65f0974886995fb5
   > block number:        8877307
   > block timestamp:     1625396854
   > account:             0xF9C0e027224764f98608d5571327C1DC8A6BF152
   > balance:             18.900398727
   > gas used:            239894 (0x3a916)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00239894 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00239894 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x581d0b197cb0e4eb150fa11682c0d37c570092f7ba5660e0c62d87a92d0f960b
   > Blocks: 1            Seconds: 12
   > contract address:    0x3Bc21B0A90f89188ff465848BB756aba8c18DC81
   > block number:        8877309
   > block timestamp:     1625396884
   > account:             0xF9C0e027224764f98608d5571327C1DC8A6BF152
   > balance:             18.895425167
   > gas used:            451608 (0x6e418)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00451608 ETH


   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x9e3e6f5823fe45ba56fc7648efd0a49815bc255532bfbd6bfea49b47cd22f582
   > Blocks: 0            Seconds: 8
   > contract address:    0x53dB13b1079983DAC3Ce91030a7452aa78e619A1
   > block number:        8877310
   > block timestamp:     1625396899
   > account:             0xF9C0e027224764f98608d5571327C1DC8A6BF152
   > balance:             18.890908247
   > gas used:            451692 (0x6e46c)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00451692 ETH


   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0xfb469cc9719145c64825654fd26752ce70b2e7e7d192eb21d6813c3ff59a7043
   > Blocks: 1            Seconds: 8
   > contract address:    0x69dDADc5e5A44470C10dC3Efc327eF92cA715e96
   > block number:        8877311
   > block timestamp:     1625396914
   > account:             0xF9C0e027224764f98608d5571327C1DC8A6BF152
   > balance:             18.886391447
   > gas used:            451680 (0x6e460)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.0045168 ETH


   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x3ebc2aba92d384dcfe61f57b3a40f5dd803481c9425ee9456ee5434ebd9fc4fe
   > Blocks: 0            Seconds: 8
   > contract address:    0xfDA729590B89f370F6B8DcD45399fa3327Ea6B17
   > block number:        8877312
   > block timestamp:     1625396929
   > account:             0xF9C0e027224764f98608d5571327C1DC8A6BF152
   > balance:             18.881874887
   > gas used:            451656 (0x6e448)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00451656 ETH


   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0xa9640b1db1b6422f128419c42e462b9479b9779318ed98f3ba0ce777fbfb5b95
   > Blocks: 0            Seconds: 8
   > contract address:    0xD30c6d4B48050a901c23c53Fca5BEd56253E2b14
   > block number:        8877313
   > block timestamp:     1625396944
   > account:             0xF9C0e027224764f98608d5571327C1DC8A6BF152
   > balance:             18.848844147
   > gas used:            3303074 (0x3266a2)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.03303074 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:           0.0510971 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.05349604 ETH


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.


### Installing

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/bilgin-kocak/udacity-supply-chain-dapp
```

```
npm install
```

Launch Ganache:

```
ganache-cli 
```

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS

## Licensing, Authors
I would like to thank Udacity for creating a platform to learn and upscale my data science skills. 
[https://www.bilginkocak.com/](https://www.bilginkocak.com/)enter link description here

