# 🎨 Solidity Template Monorepo 

[![Netlify Status](https://api.netlify.com/api/v1/badges/0f749563-48cc-40bf-beda-52573fd31cef/deploy-status)](https://app.netlify.com/sites/nifty-options/deploys)
 
# 🏄‍♂️ Quick Start (contracts)

Create the .env file in /packages/hardhat according to .env.template

```bash
yarn install 

cd packages/hardhat 

yarn build 
yarn test mainnet
```

 
## How to Deploy to Rinkeby

```
cd packages/hardhat 

yarn generate  (this generates a new account. It will make two files. One named mnemonic.txt and one with a public address. You need to set Rinkeby ETH to that public address)

yarn deploy --network rinkeby 

yarn verify --network rinkeby --license MIT 
```

## How to Deploy to Mainnet
```
cd packages/hardhat 

yarn generate  (this generates a new account. It will make two files. One named mnemonic.txt and one with a public address. You need to set Mainnet ETH to that public address)

yarn deploy --network mainnet 

yarn verify --network mainnet --license MIT 
```

## How to Run Frontend 

```
cd packages/hardhat 

yarn deploy 

yarn chain 
```

#### In a separate terminal

```
cd packages/react-app

yarn build 

yarn start 
```
 

🔏 Edit your smart contract `*.sol` in `packages/hardhat/contracts`

📝 Edit your frontend `App.jsx` in `packages/react-app/src`

💼 Edit your deployment scripts in `packages/hardhat/deploy`

📱 Open http://localhost:3000 to see the app
