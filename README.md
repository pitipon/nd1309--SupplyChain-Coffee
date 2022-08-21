# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.



### UML

* Activity Diagram
![Activity Diagram](UML/ActivityDiagram.drawio.png)

* Sequence Diagram
![Sequence Diagram](UML/SequenceDiagram.drawio.png)

* State Diagram
![State Diagram](UML/StateDiagram.drawio.png)

* Class Diagram
![Class Diagram](UML/ClassDiagram.drawio.png)


### DEVELOPMENT


#### Version
```
Truffle v5.0.2 (core: 5.0.2)
Solidity v0.5.0 (solc-js)
Node v11.15.0
```


#### Dependencies
For this project, you will need to have:
1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)
```bash
# Check Node version
node -v
# Check NPM version
npm -v
```
Note: Use node 11


2. **Truffle v5.X.X** - A development framework for Ethereum. 
```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Specify a particular version
sudo npm install -g truffle@5.0.2
# Verify the version
truffle version
```



#### Run Test
![Class Diagram](images/test.png)



#### Deploy on testnet
Contract addresses are in ContractAddress.md

```
truffle deploy --network rinkeby
```

```
Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4
> Block gas limit: 29999916


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0x499c44335a15594de16c697c345008243f6a8639881fd4aaf2d99c4d06cea77c
   > Blocks: 0            Seconds: 13
   > contract address:    0xB812C8Cf12a71b4a66dd208AD982A261c2B1D083
   > account:             0x69d378367AB777d4d8Ac0803dc4420265444587e
   > balance:             0.171361222499171829
   > gas used:            245936
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00245936 ETH

2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x4e1049c78df339de2de360bcb8806995976d0d54195e508c8e3668101dd5e07a
   > Blocks: 1            Seconds: 10
   > contract address:    0xA4c2Caa92Dd45Ca1D31Bbc4731A8660E33Cc4ecf
   > account:             0x69d378367AB777d4d8Ac0803dc4420265444587e
   > balance:             0.167698852499171829
   > gas used:            320463
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00320463 ETH


   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x07371e8ea5f607e5ee24310b546b200838542dacf59cc4753e696da4a3bc88e0
   > Blocks: 0            Seconds: 5
   > contract address:    0xCCE513a2d81bc07076a6C7C051AC6F3D03E0a545
   > account:             0x69d378367AB777d4d8Ac0803dc4420265444587e
   > balance:             0.164494222499171829
   > gas used:            320463
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00320463 ETH

   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0x50fd4461c6eee48b018b5d265caf02367beda555c13b8dfb59947d0a66b14931
   > Blocks: 0            Seconds: 5
   > contract address:    0x39FbB487e92864dF72CE50c05478f6A740B4e182
   > account:             0x69d378367AB777d4d8Ac0803dc4420265444587e
   > balance:             0.161289352499171829
   > gas used:            320487
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00320487 ETH


   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x59d5efe58a4a1a5b3589b7a560e9a930658bfa7bc60e36e30a875144d1bc6a08
   > Blocks: 0            Seconds: 0
   > contract address:    0x5a38DDd8e1f7938f582c9105640bC050b545c0b2
   > account:             0x69d378367AB777d4d8Ac0803dc4420265444587e
   > balance:             0.158084722499171829
   > gas used:            320463
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00320463 ETH


   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0x4a099c34f7035ac9171e315166659d309d4761b5d5e19aa2c93623412debdd1f
   > Blocks: 0            Seconds: 5
   > contract address:    0x5715570133ae190306384E10ED089e0344400DE9
   > account:             0x69d378367AB777d4d8Ac0803dc4420265444587e
   > balance:             0.130294912499171829
   > gas used:            2778981
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.02778981 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.04060857 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.04306793 ETH

```