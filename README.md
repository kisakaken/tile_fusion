# TileFusion: 

a captivating rendition of the classic 2048 game, now infused with blockchain technology and an extra layer of challenge. Developed on the innovative Sui.

TileFusion operates through a smart contract, empowering players to generate a game that unfolds directly on the blockchain. Through the front-end interface, transactions are submitted to the Sui blockchain, triggering calculations for the subsequent state of the game board. The updated state can relayed back to a front end, dynamically animating and showcasing the evolving game board. 

## Sui

This project is built on the Sui blockchain, which provides the performance necessary for a great game experience. Every move is a transaction that is recorded on-chain, making the gameplay verifiable, shareable, and transferable. Each game is an NFT that can be sent to anyone and will display in a web3 wallet.

## The Smart Contract

The SUI 8192 smart contract is written Sui Move for deployment on the Sui blockchain. It consists of three parts:

1. **Game:** Primarily entry functions for making moves and recording the overall game state.

2. **Game Board:** Most of the game logic.

3. **Leaderboard:** A shared object that accepts games, sorting them into order based on top tile and score.



### Working With The Smart Contract

From the `move` folder:

#### Build Contract

`sui move build`

#### Test Contract

`sui move test`

or

`sui move test --filter SUBSTRING`

#### Deploy Contract

`sui client publish --gas-budget 10000`

You will need to update the contract and leaderboard address in `constants.ts` with the values provided when you publish the contract.
