﻿# zkSync-Era-contract

Prerequisites
Download and install Node. https://nodejs.org/en/download
Download and install  https://github.com/nvm-sh/nvm#installing-and-updating  
nvm  to change the running Node version to v16.16.0 with command nvm use 16.

Use the yarn or npm package manager.https://yarnpkg.com/getting-started/install
We recommend using yarn. To install yarn, follow the Yarn installation guide.

A wallet with sufficient Göerli ETH on L1 to pay for bridging funds to zkSync and deploying smart contracts.
ERC20 tokens on zkSync are required for the testnet paymaster. We recommend using the faucet from the zkSync portal.
https://goerli.portal.zksync.io/faucet

You know how to get your private key from your MetaMask wallet
https://support.metamask.io/hc/en-us/articles/360015289632-How-to-export-an-account-s-private-key


STEP 1.   
Initialize the project and install the dependencies, with the following command.

yarn init -y
yarn add -D typescript ts-node ethers@^5.7.2 zksync-web3 hardhat @matterlabs/hardhat-zksync-solc @matterlabs/hardhat-zksync-deploy


STEP 2. 
Compile the contract with the following command:
  
 yarn hardhat compile


ADD YOUR PRIVATE KEY TO THE SECRET FILE //  *** add  screct to gitignore file before pushing to github ... 

STEP 4.
Deploy the contract with the following command:

yarn hardhat deploy-zksync


You should see something like this:
Running deploy script for the Greeter contract
The deployment is estimated to cost 0.0265726735 ETH
constructor args:0x000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000094869207468657265210000000000000000000000000000000000000000000000
Greeter was deployed to 0xE84774C41F096Ba5BafA1439cEE787D9dD1A6b72

Congratulations! You have deployed a smart contract to zkSync Era Testnet 🎉

https://explorer.zksync.io/  



