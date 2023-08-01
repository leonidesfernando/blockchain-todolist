# Blockchain TodoList Project
This is a simple project to develop a smart contract to a task manager. You'll use it to connect to and deploy on the Goerli test networks.
Based on this tutorial from Microsoft learn: https://learn.microsoft.com/en-us/training/modules/blockchain-ethereum-networks

## Requirements
- Visual Studio Code to create the project.
- [Truffle](https://www.trufflesuite.com/truffle) to compile and deploy.
- The [Ganache CLI](https://github.com/trufflesuite/ganache-cli) as the blockchain development server.

- ~~Ropsten~~  Goreli
- Infura (you must create account)
- MetaMask wallet (you must create account)
    - wallet address: 0x95bD4EA0e6346b779568e19eCCFE224E5A268e1B
- HDWallet-Provider: `npm install @truffle/hdwallet-provider`
- fs: `npm install fs`

## Compile & Deploy
You can compile and deploy using comand line.
Before that you must start the development blockchain: _`ganache-cli`_

- compile: `truffle complile`
- deploy: `truffle migrate --reset`

To deploy on Goerli network: `truffle migrate --network goerli`

After that, In Goerli Etherscan, enter the contract address. [Then inspect your contract](https://goerli.etherscan.io/address/0x95bD4EA0e6346b779568e19eCCFE224E5A268e1B).