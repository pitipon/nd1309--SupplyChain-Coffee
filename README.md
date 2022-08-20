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



#### Run the application