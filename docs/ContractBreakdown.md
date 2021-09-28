# Contract Breakdown and Review

---

The following vulnerability assessment is limited to the scope of following contracts of Aastra:

- Vault.Sol
- Router.Sol
- Factory.Sol

# Overview of Contracts:

## **Vault.sol**

The following contract controls the access of funds deposited by users who are depositing for earning liquidity fees on Uniswap v3. It has a function that involves:
- Depositing funds in Uniswap v3 for LP'ing 
- Claim fees from Uniswap for corresponding LP position 
- Swapping assets from one token to another token on Uniswap
- Issuance/claim of erc20 tokens indicative of share the user holds
- Movement of funds across different tick ranges of Uniswap v3 pool.

[Issues of Vault.sol](https://www.notion.so/0d35e76cbe5d40f6ab928d5e56d526e2)

classification of vulnerabilities guide: [here](https://immunefi.com/severity-system/)

Check the spec guide [here](https://cwe.mitre.org/data/definitions/699.html)

## **Router.sol**

The following contract is designed to be used by the strategy managers to move their vault funds to new tick ranges. The strategy manager can easily get the state of the current vault and move funds with less complexity. The contract gets the corresponding wallet of the strategy manager using the state stored in the factory contract.

[Issues of Router.sol](https://www.notion.so/d035fc8bb5124bf690d41929b3b4aff5)

## **Factory.sol**

The following contract is designed to use by the store the state of vaults and their corresponding strategy managers. This contains important governance which can alter the state

[Issues of Factory.sol](https://www.notion.so/033f4d2045c6473a8b46a0ddfebafe17)
