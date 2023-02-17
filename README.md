#  Arbitrage Bot

## Setup

**Prerequisites:**

* Node.js (v14.17.5)
* npm (6.14.14)
* Ganache CLI (v6.12.2)
* Truffle (v5.1.55)

Refer to `package.json` for specific package versions.

## Local Testing 

1. **Launch Ganache:**
   ```bash
   ganache-cli --fork <Ethereum-Node-URL>@13027545 --unlock 0xE8E8f41Ed29E46f34E206D7D2a7D6f735A3FF2CB 
   ```
   *(Note: Infura can replace the Ethereum Node. Block number is crucial.)*

2. **Run Truffle Tests:**
   ```bash
   truffle test
   ```


## Mainnet Deployment 

1. **Modify Contract:**
   Uncomment line 396 in `Flashy.sol` for miner fee functionality.

2. **Deploy:**
   ```bash
   truffle migrate --network ethereum_mainnet
   ```

   **Fee Split:** Consider a miner fee of 80% and a 20% profit share. Adjust as needed. 


## Recommendation

Explore [Foundry](https://github.com/foundry-rs/foundry) for future projects. It's superior to Truffle and Hardhat.

**Best of luck with your ventures!** 
