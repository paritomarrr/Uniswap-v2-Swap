# UNISWAP 
Uniswap V2 is a decentralized Exchange, running on the Ethereum Blockchain, used for trading ERC20 tokens. 


## What Does Uniswap Do?
There are 2 types of users:
- Liquidity Providers:
Liquidity Providers provide the pool with the 2 tokens that can be exchanged. We will call them Token0 and Token1. 
In return, they receive a third token that represents partial ownership of the pool called a Liquidity Token.


- Traders
Traders send one type of token to the pool and receive the other. The exchange rate is determined by the reltive number of Token0s and Token1s that the pool has. 
In addition, the pool takes a small percent as a reward for the liquidity pool. 

## Main fuctionalities
1. Swap between different tokens
2. Add liquidity to the market and get rewarded with pair exchange ERC-20 liquidity tokens
3. Brun ERC-20 liquidity tokens and get back the ERC-20 tokens that the air exchange allows traders to exchange.

## Interfaces Used
In the periphery contract (UniswapV2Router.sol)
- Identifies the amount that needs to be traded on each exchnge along the path
- Oterates over the path. For every exchange along the way it sends the input token and then calls the exchange's swap function. 


## How to test Uniswap Swap Functionality?
1. Clone this repo
2. Run command `npm i`
3. Create an '.env' file and add Alchemy API key and make sure you fork the mainnet
4. To deploy the contract, run the command, `npx hardhat run scripts/deploy.js`
5. Tp run the uniswap test, run the command, `npx hardhat test`


