# Decentralized Voting (dVoting/Blockchain Voting)

A decentralized voting system based on Ethereum blockchain technology.

# Project Demo
https://github.com/samriddhide/Blockchain_voting/assets/100946305/9f20bc2f-ea38-43bb-95c2-bd0b1790fe61

### Requirements

- [Node.js]
- [Truffle]
- [Ganache]
- [Metamask]

#### Getting the requirements

1. Download and install **NodeJS**

   Download and install NodeJS from [here](https://nodejs.org/en/download/ "Go to official NodeJS download page.").

1. Install **truffle** and **ganache-cli** using node packager manager (npm)

   ```shell
   npm install -g truffle
   npm install -g ganache-cli
   ```

1. Install **metamask** browser extension

### Configuring the project for development

1. Clone this repository

   ```shell
   git clone https:
   cd dVoting
   ```

2. Run local Ethereum blockchain

   ```shell
   ganache-cli
   ```

   > Note: Do not close `ganache-cli` (the blockchain network needs to be running all the time)

3. Configure metamask on the browser with the following details

   New RPC URL: `http://127.0.0.1:8545` *(use `port: 7545` for **ganache gui**, update it in the file:`truffle-config.js` as well)*

   Chain ID: `1337`

4. Import account(s) using private keys from ganache-cli to the metamask extension on the browser

5. Deploy smart contract to the (local) blockchain network (i.e ganache-cli)

   ```shell
   # on the dVoting directory
   truffle migrate
   ```

   > Note: Use `truffle migrate --reset` for re-deployments
