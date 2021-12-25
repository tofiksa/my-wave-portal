# Basic Sample Hardhat Project

Smart contract that keeps a message and counts of :wave:

## To run the smart contract

```shell
npx hardhat run scripts/run.js
```
## To deploy the smart contract

```shell
npx hardhat run scripts/deploy.js --network rinkeby
```

This application uses https://www.alchemy.com/ to deploy to the ethereum network. You can get the Alchemy api key and private key by registering and using alchemyapi.

```javascript
module.exports = {
  solidity: "0.8.4",
  networks: {
    rinkeby: {
      url: process.env.STAGING_ALCHEMY_KEY,
      accounts: [process.env.PRIVATE_KEY],
    },
  },
};
```