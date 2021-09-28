---

These are the contract addresses that are deployed to the Ethereum mainnet.

### **Core Contracts v1**

| Contract      | Address                                    |
| ------------- | ------------------------------------------ |
| Factory       | 0xBAD59D2BA9A532242F1287DeaBc4227E8150D074 |
| Router        | 0x34511BE0a5eB24183B077682cBec5c7a9C9c5ADb |
| Periphery     | 0xd47eE04a6f3c9739007D311962279eb5b2c856C5 |
| ETH-PUT Vault | 0xd47eE04a6f3c9739007D311962279eb5b2c856C5 |

## **System Roles**

Currently, the protocol has a few privileged roles that help bootstrap the protocol at its initial development.

| Role       | Description                                                                                                                                                |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Governance | Controls the functions which require governance. Like `emergencyWithdraw` during unforeseen circumstances. And creation of new vaults using `createVault`. |
| Strategy   | Controls the movement of funds in Vault to and fro from Uniswap Pool.                                                                                      |
| Router     | Used by strategy managers to easily move funds in a vault.                                                                                                 |
| User       | Has access to deposit and withdraw assets in Vault.                                                                                                        |
