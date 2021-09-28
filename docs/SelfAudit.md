---

Brahma represents a suite of open-source products that aims to generate yield and increase capital efficiency in the DeFi ecosystem. The first set of smart contracts are being launched under AASTRA. **AASTRA** aims to generate structured yield on top of AMMs via liquidity provisioning, starting with Uniswap V3.

With this in mind, the development of **AASTRA** has happened in stages, the rollout will happen in stages, so as to control any unforeseen security concerns and corner cases. Brahma has tried to implement and create a new standard for protocols for self-auditing and peer review, before the commercial audits.

### **Description from the Users Point of View**

A typical DeFi user will be using Aastra instruments by depositing their stable coins and get exposure to different assets (including synths in the future) and positions to earn a yield. The UX is similar to Yearn vaults and Token sets.

### **Tokens and Platforms used for V1**

Platforms interacted with: Uniswap V3 both the core contracts (here) and periphery contracts (here)
Tokens issued: Aastra issues ERC-20 based tokens on user's shares in a yield Instrument. ERC-20 standard used (Github)

## **Executive Overview**

**Auditors: Bapireddy Karri, 0xKali**

**Type:** Put Selling Strategies

**Timeline:** The audit was started on 1/9/21 done on commit id `ee73ee8ba7417a9c208035d2f97d788cb54ca630` on repository [https://github.com/Brahma-fi/aastra](https://github.com/Brahma-fi/aastra)

**EVM:** London

**Languages:** Solidity, Python, JS

**Method:** All the public functions of contracts are documented with natspec specification and unit tested. You can check the code-coverage reporting [here](https://github.com/Brahma-fi/aastra/tree/master/coverage). Other than this the contract is tested for re-entrancy bugs and buffer overflow attacks using _**slither**_. You can check the report for this here (github link).

Along with this the team has tested the contracts on the previous hack that happened on other protocols with similar architecture. All the issues found during such comparison are shared **link**

**Tools used:** Slither, Surya, MythX, DOT

**Source Code:** [https://github.com/Brahma-fi/aastra](https://github.com/Brahma-fi/aastra)

**Total Issues:** 14 (2 High + 3 Critical + 6 Medium + 3 Low)

**Governance:** 0x48AC9CAd3DA5752eB1276d650BF321342dF6cd0c

**Peer Reviews:** In progress
