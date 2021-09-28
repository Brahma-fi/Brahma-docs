---

Aastra is a set of open-source smart contracts designed to simplify the launch of market-making strategy vaults on uniswap v3. Aastra aims to improve the yield earned by liquidity providers by abstracting out the market-making strategies execution using vault structure. Using this as our starting point there are 3 stakeholders involved in the interaction of contracts.

1. Users who deposit their funds to be used for liquidity provision on uniswap v3.
2. Strategy Manager who moves the user deposited funds across uniswapv3 lp position.
3. Aastra protocol governs the vault funds to ensure the safety of funds.

The vulnerability assessment is limited to the scope of the following Contracts of Aastra:

- Vault.Sol
- Router.Sol
- Factory.Sol

**The following phases and tools were used by us during this self audit:**

- ✅ Research into architecture, purpose, and use of ERC20 Token.
- ✅ Smart Contract manual code read and walkthrough.
- ✅ Graphing out functionality and contract logic/connectivity/functions (surya)
- ✅ Manual Assessment of use and safety for the critical solidity variables and functions in scope to identify any arithmetic related vulnerability classes.
- ✅ Scanning of solidity files for vulnerabilities, security hotspots, or bugs. (MythX)
- ✅ Static Analysis of security for scoped contract, and imported functions. (Slither)
- ✅ Testnet deployment (Hardhat, Ethersjs, Infura)
