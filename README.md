# Ray Dex Oracle TWAP

A Uniswap V3 TWAP Price on PulseChain. Onchain oracle sending price feeds from Polygon to other chains over the deBridge protocol.

UNI V3 Contract Pools on Polygon

WETH/USDC >> 0x45dda9cb7c25131df268515131f647d726f50608
WBTC/USDC >> 0x847b64f9d3A95e977D157866447a5C0A5dFa0Ee5

# Compile Smart Contract

```shell
npx hardhat compile

```

# Test Smart Contract

```shell
npx hardhat test
```

# Deploy TWAP on Polygon and Binance for PulseChain

```shell
npx hardhat run --network matic scripts/deploy.ts
npx hardhat run --network testnet scripts/deploy.ts
npx hardhat run --network bsc scripts/deploy.ts
```

Then, copy the deployment address and paste it in to replace `DEPLOYED_CONTRACT_ADDRESS` in this command:

# Etherscan verification

```shell
npx hardhat verify --network matic DEPLOYED_CONTRACT_ADDRESS
```
