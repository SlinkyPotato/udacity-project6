# Udacity Project 6 - Supply Chain

Truffle version: v5.1.55 <br>
Solidity version: 0.6.12 <br>
Node version: 12.18.4 <br>
Web3 version: 1.2.9 <br>
OpenZeppelin version: v3.2.0 <br>
SupplyChain Contract Address: 0x2609a497eB59972e2fD484b1615f7241282073BA <br>
FarmerRole Contract Address: 0x247624671dc18571709E8F1511F82BF39CFfD541 <br>
DistributorRole Contract Address: 0xd4AaB153E8115464521273Cfe386c979fB8Bf505 <br>
RetailerRole Contract Address: 0x9499826490F30F9c01DC859a57CB991e21618C6f <br>
ConsumerRole Contract Address: 0x6D7103059C56F09443aC8789C5eFF2D9FfA27E66 <br>

### SupplyChain.sol
This is the main contract that connects and makes use of the following contracts
 - ConsumerRole.sol
 - DistributorRole.sol
 - FarmerRole.sol
 - RetailerRole.sol
 - Roles.sol

This contract has the variablles
 - owner // owner of the contract
 - upc // the universal product code 
 - sku // the stock keeping unit
 - items // a list of Items mapping by unsigned ints
 - itemsHistory // an unsigned unit to Item class mapping of the items

The contract has
- Definitation of the State enum that describes the various status of the item.
- Events for when an items is havested, processed, packed, set for sale, sold, shipped, receieved, and purchased
- helper functions to process the item

### Building
Dependencies for the project can be downloaded by
```
> npm install
```

Contract compile
```
> truffle compile
```

Run tests
```
> truffle develop
truffle(develop)> test
```

App run in another terminal by
```
> npm run dev
```
