# PupperCoin Crowdsale

## Introduction

For this assignment we were asked to create a crowdsale, open to the public, that will sell the PupperCoin Token in order to fund network development. The network will be used to track the dog breeding activity across the globe in a decentralized way, and allow humans to track the genetic trail of their pets.

## PupperCoin Token

The first step is to create the PupperCoin as an ERC20Mintable token, the technical standard for smart contracts on the Ethereum blockchain.

The decimal points for the token are set to 18 decimals because all of the math done in the contract is done on the smallest currency unit, which is 1 wei (1 ETH === 10^18 wei).

## PupperCoin Crowdsale Contract

The contract that we used for the crowdsale inherits from the following OpenZeppelin contracts:

- Crowdsale
- MintedCrowdsale
- CappedCrowdsale
- TimedCrowdsale
- RefundablePostDeliveryCrowdsale

## PupperCoin Deployment Contract

The deployment contract is contained in the same file as the crowdsale contract and can delpoy to our local blockchain or a testnet.

## Testing the Crowdsale

We deployed the contract to our local blockchain first to test it using the following steps:

- Step one is to deploy the PupperCoinSale Deployer Contract:

![step_1](screenshots/step_1.png)

- Step two is to copy the token_sale_address and deploy the PupperCoinSale contract:

![step_2](screenshots/step_2.png)

- Step three is to copy the token_address and deploy the PupperCoin:

![step_3](screenshots/step_3.png)

- Step four is to buy tokens using other addresses:

![step_4](screenshots/step_4.png)

- Step five is to confirm that the time has run out and the contract is no longer open:

![step_5](screenshots/step_5.png)

- Step six is to finalize the contract:

![step_6](screenshots/step_6.png)

## Deploy to Ropsten Testnet

Using the deploy tab in Remix, we deployed the contract in the same manner as above except it was deployed to the Ropsten testnet. 

![ropstem_deploy](screenshots/ropstem_deploy.png)

The Gas Fee for the local blockchain appears to be higher than it is to deploy the contract to the testnet:

![ropsten_gas](screenshots/ropstem_gas.png)

![local_gas](screenshots/local_gas.png)

The remaining steps are the same as above, except all the transactions are conducted on the testnet.

## MyCrypto

The custom tokens can be added to your MyCrypto Wallet:

![local_gas](screenshots/my_crypto.png)












