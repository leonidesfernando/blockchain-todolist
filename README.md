# Blockchain TodoList Project
This is a simple project to develop a smart contract to a task manager. You'll use it to connect to and deploy on the Goerli test networks.
Based on this tutorial from Microsoft learn: https://learn.microsoft.com/en-us/training/modules/blockchain-ethereum-networks

## Requirements
- Visual Studio Code to create the project.
- [Truffle](https://www.trufflesuite.com/truffle) to compile and deploy.
- The [Ganache CLI](https://github.com/trufflesuite/ganache-cli) as the blockchain development server.

- ~~Ropsten~~  Goreli, Sepolia
- Infura (you must create account)
- MetaMask wallet (you must create account)
    - wallet address: 0x95bD4EA0e6346b779568e19eCCFE224E5A268e1B
- HDWallet-Provider: `npm install @truffle/hdwallet-provider`
- fs: `npm install fs`

## Compile & Deploy
In this project we are going to use just command line. 

>### <span style="color:yellow">**Remember**</span>
>In Ethereum we need to have funds/gas :fuelpump: to run your smart contracts, so you need make sure you have enough funds in your wallet to execute yours smart contracts.

Thus, you need to:
1. Fill up your wallet with funds/gas :fuelpump:
    - _**Info**_: For develoment you can request funds on a Faucet web site.

    - _<sub>Currenty Seppoia is the most used and recommend TestNet network for develoment and testing.</sub>_

    - For Sepolia:
        - https://sepolia-faucet.pk910.de/
        - https://fauceth.komputing.org/
        - https://sepoliafaucet.com/
        - https://testnet.help/en/ethfaucet/sepolia
        - https://www.infura.io/faucet/sepolia

2. Start your develoment blockchain: _`ganache-cli`_

3. Compile your contracts: `truffle complile`

4. Deploy your contracts: `truffle migrate --reset`

5. Deploy your contract in the proper network: 
    - We are using Sepolia: `truffle migrate --network sepolia`
    - To other network: `truffle migrate --network <network_name>`

6. After that, In Sepolia Etherscan, enter the contract address. [Then inspect your contract](https://sepolia.etherscan.io/address/0x95bD4EA0e6346b779568e19eCCFE224E5A268e1B).