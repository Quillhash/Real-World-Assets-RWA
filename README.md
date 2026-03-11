# Real World Assets (RWAs)

Welcome to the Real World Assets (RWAs) GitHub repository by QuillAudits!

This repository serves as a resource hub for developers, enthusiasts, and researchers interested in exploring, developing, and understanding RWAs on the blockchain. Here, you'll find code examples, smart contract templates, technical guides, and relevant resources to help you navigate the exciting world of RWAs.


## RWA Development Handbook

> **Start here if you want to truly understand how RWA systems are designed, built, and regulated.**


<p align="center">
  <img src="./public/RWA_handbook.png" alt="rwa_handbook_image" />
</p>

We've published a full-length handbook at:

#### [research/rwa-development](https://www.quillaudits.com/research/rwa-development)

This handbook goes far beyond surface-level explanations. It is written for builders, auditors, founders, and protocol architects who need a complete mental model of RWA systems, from off-chain custody and legal structures to on-chain token standards, settlement flows, and compliance enforcement. Every chapter is built around real architectures, real constraints, and real tradeoffs. Just deep, implementation-ready knowledge for anyone serious about building or securing RWA protocols.

### Understanding Real World Assets on Blockchain :

Tokenized real-world assets (RWAs) are blockchain-based digital tokens that represent physical and traditional financial assets, such as cash, commodities, equities, bonds, credit, artwork, and intellectual property. The tokenization of RWAs marks a significant shift in how these assets can be accessed, exchanged, and managed, unlocking an era of new opportunities for both blockchain-powered financial services and a wide variety of non-financial use cases underpinned by cryptography and decentralized consensus. RWAs can be tokenized on blockchain networks, allowing for fractional ownership, increased liquidity, and enhanced accessibility to traditionally illiquid assets.

### Types of RWAs :

Real World Assets (RWAs) encompass a wide range of tangible and intangible assets with intrinsic value. These are just a few examples of the diverse range of assets that can be tokenized on the blockchain.

1. Real Estate: This includes residential, commercial, and industrial properties. Real estate tokenization allows investors to own fractional shares of properties, providing liquidity and diversification.

2. Commodities: Physical commodities such as precious metals (gold, silver), agricultural products (grains, coffee), energy resources (oil, natural gas), and others can be tokenized to facilitate trading and investment.

3. Art and Collectibles: Tokenization of art, rare collectibles, and memorabilia enables fractional ownership and investment opportunities in traditionally illiquid markets.

4. Intellectual Property (IP): This includes patents, copyrights, trademarks, and other forms of intellectual property rights. Tokenization allows creators to monetize their IP assets and investors to participate in revenue-sharing agreements.

5. Equity and Securities: Shares of private companies, stocks, bonds, and other financial instruments can be tokenized to increase liquidity, streamline transactions, and enable global access to capital markets.

6. Revenue-Generating Contracts: Contracts with predictable revenue streams, such as leases, royalties, and licensing agreements, can be tokenized to provide investors with recurring income opportunities.

7. Deeds and Titles: Tokenization of deeds, titles, and ownership certificates for real estate, vehicles, and other assets can streamline transfer processes and enhance transparency in ownership records.

8. Carbon Credits and Renewable Energy Assets: Environmental assets such as carbon credits, renewable energy certificates (RECs), and carbon offsets can be tokenized to facilitate trading and investment in sustainable initiatives.

9. Luxury Assets: High-value luxury items such as yachts, private jets, and luxury watches can be tokenized to fractionalize ownership and broaden access to exclusive markets.

### Key Components and Considerations in RWAs :

![Categories of RWAs](https://assets-global.website-files.com/5f75fe1dce99248be5a892db/65675d919a0831972f6deee3_6552522f392cb9f529f5a318_652562d7832838b219cbf4f2_RWAs-in-DeFi_V2_16x9.png)

Developing a Real World Asset (RWA) on the blockchain involves several steps and considerations to ensure compliance, security, and efficiency.

1. Define the Asset: Determine the real-world asset you want to tokenize on the blockchain. This could include real estate, commodities, art, intellectual property, or any other asset with tangible or intrinsic value.

2. Legal and Regulatory Compliance: Understand the legal and regulatory requirements for tokenizing the chosen asset. Depending on the jurisdiction and type of asset, you may need to comply with securities regulations, property laws, anti-money laundering (AML) regulations, and know-your-customer (KYC) requirements.

3. Choose the Blockchain Platform: Select a suitable blockchain platform for tokenizing the asset. Ethereum and other smart contract platforms are commonly used for tokenization due to their programmability and established ecosystem. Alternatively, consider private or permissioned blockchains for specific use cases.

4. Token Standards: Choose or develop a token standard that best suits the characteristics of the asset. For example, ERC-20, ERC-721 (NFTs), or ERC-1400 (Security Tokens) are common standards used for tokenizing assets on Ethereum.

5. Collateralization: Many tokenized RWAs are backed by collateral, which could be the asset itself (in the case of direct backing) or other assets and financial instruments (in the case of indirect backing). The collateralization process ensures that the on-chain token maintains a stable and defined value relative to the off-chain asset it represents.

6. Smart Contract Development: Develop smart contracts to represent and manage the asset on the blockchain. These contracts should define token issuance, transfer rules, ownership rights, and any other functionalities required to manage the asset's lifecycle.

7. Oracles and Data Feeds: Integrate oracles or data feeds to bridge the gap between the blockchain and the real world. Oracles provide external data, such as asset valuations, ownership records, or regulatory compliance information, ensuring transparency and accuracy.

8. Tokenization Process: Tokenize the asset by minting digital tokens on the blockchain. Each token represents ownership or fractional ownership of the underlying asset. Ensure that the tokenization process follows legal requirements and is properly documented.

9. Security and Audits (we're here for it :D): Conduct security audits of smart contracts and overall system architecture to identify and mitigate potential vulnerabilities or attack vectors. Implement best practices for secure smart contract development and deploy contracts on testnets for thorough testing.

## Categorisation of RWAs

![Categories of RWAs](./public/cover.png)

We can tokenize real-world assets by combining any of the following traits:

1. Asset location: On-chain or Off-Chain
2. Collateral location: On-chain or Off-Chain Collateral
3. Backing type: Direct backing or Indirect (synthetic)

-   Asset location - refers to the location of the asset which is being tokenised.

    -   Example: Real estate & Gold are Off-chain assets whereas BTC & ETH are On-chain assets.

-   Collateral location - refers to the location of the collateral

    -   Example: PAXG is a digital token backed by physical gold (Off-chain collateral) & DAI stablecoin requires On-chain collateral

-   Backing type - refers to the type of the collateral backing the asset.
    1. Direct backing - Collateral backing the asset is the same as the asset.
    -   Example: PAXG token is directly backed by gold. Similarly, USDC is also directly backed by actual USD.
    2. Synthetic (Indirect) backing - Collateral backing the asset is not the same as the asset.
    -   Example: DAI coin by MakerDAO is backed by on-chain collateral assets which can consist of other crypto tokens but not USDT(since DAI is a stablecoin).

Since we have 3 categories each with 2 options, we can have 8 different types of RWAs. Having 8 possible categories of RWAs doesn't necessarily mean that all of them have being implemented till now.

We'll be focusing on the five majorly used categories of RWAs:

1. On-Chain Asset with On-Chain Collateral and Direct Backing
2. On-Chain Asset with On-Chain Collateral and Synthetic (Indirect) Backing
3. Off-Chain Asset with Off-Chain Collateral and Direct Backing
4. Off-Chain Asset with Off-Chain Collateral and Indirect Backing
5. Off-Chain Asset with On-Chain Collateral and Indirect Backing

## On-Chain Asset with On-Chain Collateral and Direct/Indirect Backing

Wrapped ETH (WETH) and Wrapped BTC (WBTC) are examples of on-chain assets which are directly/indirectly backed by on-chain collateral.

-   WETH: Ether (ETH), the native cryptocurrency of Ethereum, doesn't conform to the ERC-20 token standard, which is a widely adopted standard for Ethereum tokens. This discrepancy can cause compatibility issues with ERC-20 based dApps. WETH was introduced as a solution to this problem, allowing ETH to be "wrapped" into an ERC-20 compatible format. To obtain WETH, users send ETH to a WETH smart contract, which locks the ETH and issues an equivalent amount of WETH in return. This process is reversible; users can convert their WETH back to ETH by sending the WETH back to the smart contract. The value of WETH is directly backed by ETH at a 1:1 ratio, ensuring that each WETH token is always equivalent to one ETH. The ETH used as collateral is held securely in the smart contract.

-   WBTC: WBTC brings Bitcoin's liquidity to the Ethereum ecosystem, allowing Bitcoin holders to interact with Ethereum's DeFi applications without selling their BTC. WBTC is created through a process involving merchants and custodians. BTC is sent to a custodian, who then mints an equivalent amount of WBTC on Ethereum. This process is also reversible, allowing WBTC holders to redeem their tokens for BTC. The value of WBTC is directly backed by BTC, with a 1:1 ratio. Each WBTC token represents one BTC, and the corresponding BTC is held by custodians off the Ethereum blockchain but is managed through on-chain contracts and mechanisms for minting and burning WBTC.

## Off-Chain Asset with Off-Chain Collateral and Direct/Indirect Backing

USDT and USDC fall into a unique category of RWAs, which are digital tokens representing fiat currencies like the US dollar on blockchain platforms. These RWAs are characterized by their off-chain assets (fiat currencies, gold, stock shares, real estate, etc) and off-chain collateral, with their value directly or indirectly backed by these reserves.

This process not only enhances liquidity and accessibility but also introduces new opportunities for investment and ownership.

-   Technical Framework for Tokenizing RWAs:

    -   Smart Contracts: The backbone of any tokenization platform is smart contracts, self-executing contracts with the terms of the agreement directly written into code. These contracts govern the creation, distribution, and management of tokens representing RWAs.

    -   Asset Custody and Verification: Essential to the process is ensuring that the real-world asset is securely held and verified. For instance, tokenizing gold would require a secure vault, and tokenizing real estate would need a reliable registry to confirm ownership and liens.

    -   Oracles for Real-World Data: Oracles are used to bring real-world information onto the blockchain securely. They can provide data on asset valuation, ownership changes, or even gold price fluctuations, which is crucial for maintaining the token's value and relevance.

    -   Regulatory Compliance and Legal Framework: Ensuring compliance with local and international regulations is critical. This might involve setting up legal structures that recognize token ownership as equivalent to owning a portion of the physical asset.

    -   Token Standards and Interoperability: Using established token standards like ERC-20 (for fungible tokens) or ERC-721 (for non-fungible tokens, useful in real estate to represent unique properties) ensures that the tokens can interact seamlessly with wallets, exchanges, and other smart contracts.

-   Examples:

    -   Gold: Tokenizing gold involves issuing digital tokens backed by physical gold stored in secure vaults. Each token represents a specific quantity of gold (e.g., 1 gram). The physical gold acts as collateral, and the token's value is directly tied to the gold price, offering investors exposure to gold without the need for physical possession. Example - Paxos Gold (PAXG) https://github.com/paxosglobal/paxos-gold-contract/tree/master/contracts

    -   Real Estate: Real estate tokenization breaks down property ownership into digital tokens, allowing for fractional ownership and investment. This could dramatically lower entry barriers to real estate investment and improve liquidity in the market. Each token might represent a share of ownership in a property, a right to rental income, or other property-related rights. Currently active Real Estate RWA projects - https://www.alchemy.com/best/real-estate-rwas

    -   Stock Market Shares: Tokenizing stock shares involves creating digital tokens that represent ownership of a company's stock. This can democratize access to equity markets, allowing for fractional ownership of stocks and potentially opening up global markets to a wider range of investors.

## Off-Chain Asset with On-Chain Collateral and Indirect Backing

The DAI stablecoin is a notable example of an off-chain asset with on-chain collateral and indirect backing, primarily because its value is pegged to the U.S. dollar (an off-chain asset), while its collateral consists of various cryptocurrencies stored on-chain within the MakerDAO system. This setup represents an indirect backing because the value of DAI is stabilized against the U.S. dollar through smart contracts and collateralized debt positions (CDPs), rather than a direct 1:1 reserve of dollars.

### Tokenising an Apple share

In this repository, we'll be diving deep into the technicalities of tokenisation of Real-World Assets by developing an Apple Coin (AAPL) ERC-20 token where the value of each AAPL token will be 1:1 pegged with the real time value of an Apple share in the US stocks market. The backing collateral will be wETH (on-chain collateral & indirectly backed).

![AAPL](./public/AAPL.png)

The project source code is pushed in the same repository for one's reference.

The AAPL smart contract is designed to tokenize Apple shares, allowing users to mint and redeem tokens that represent a share in Apple, using Ethereum (ETH) as collateral. This contract ensures that the system remains over-collateralized, maintaining algorithmic stability without governance or fees. Here's a detailed breakdown of the contract's components:

**Constructor**

![AAPL](./public/1.png)

-   The constructor sets up the contract by initializing it with the addresses of the Chainlink price feeds for Apple shares (AAPL) and ETH/USD. These feeds are essential for determining the value of the collateral and the AAPL tokens in USD.
-   Inherits from OpenZeppelin's ERC20 to provide standard token functionalities.

**External Functions**

1. `depositAndmint`:

![AAPL](./public/2.png)

-   Allows users to deposit ETH as collateral and mint AAPL tokens in the same transaction.
-   The amount of ETH sent with the transaction is added to the user's collateral balance.
-   The amountToMint of AAPL tokens is added to the user's minted balance.
-   Checks if the resulting health factor meets the minimum requirement, reverting the transaction if it doesn't, to ensure the system remains over-collateralized.
-   Mints the AAPL tokens to the user's account using the \_mint function from the ERC20 standard.

2. `redeemAndBurn`:

![AAPL](./public/3.png)

-   Users can redeem AAPL tokens and receive the equivalent value in ETH collateral.
-   The USD value of the AAPL tokens to redeem is calculated, and the equivalent amount of ETH is determined.
-   The AAPL tokens are subtracted from the user's minted balance, and the health factor is checked to ensure system stability.
-   The AAPL tokens are burned, and the equivalent ETH is sent back to the user.
-   Reverts if the ETH transfer fails, ensuring atomicity.

**Public/View Functions**

1. `getHealthFactor`

![AAPL](./public/4.png)

-   Computes and returns the health factor of a user's account, which indicates the level of over-collateralization.

2. `getUsdAmountFromaapl`

![AAPL](./public/5.png)

-   `amountaaplInWei`: The amount of AAPL tokens for which the USD value is being requested. It's denoted in Wei to maintain precision, considering that Ethereum and many tokens on the Ethereum blockchain, including ERC-20 tokens like AAPL, can have up to 18 decimal places.
-   The function returns the USD value of the specified amount of AAPL tokens as a uint256. This value is calculated based on the current price of an Apple share, as provided by an oracle.
-   The function first initializes a priceFeed object using the AggregatorV3Interface interface and the address of the AAPL price feed oracle (`i_aaplFeed`), which provides the current market price of an Apple share.
-   It then calls `staleCheckLatestRoundData()` on the priceFeed object, which is a method from the Chainlink Aggregator interface designed to fetch the latest reliable price data. The function returns multiple values, but only the price is used here, which represents the current price of an Apple share in USD.
-   The function calculates the USD value by multiplying the `amountaaplInWei` (the amount of AAPL tokens for which the value is being calculated) by the price of an Apple share in USD (uint256(price)).
-   To maintain precision, the price is first multiplied by `ADDITIONAL_FEED_PRECISION` (a constant that adjusts for the difference in decimal places between the token and the USD value as provided by the oracle).
-   The result is then divided by `PRECISION`, another constant used to adjust the final value back to a standard decimal format, ensuring the result is accurate and usable.

3. `getUsdAmountFromEth` & `getEthAmountFromUsd`

![AAPL](./public/6.png)

-   `getUsdAmountFromEth`: Returns the USD value of a given amount of ETH using the ETH/USD price feed.
-   `getEthAmountFromUsd`: Converts a USD amount to the equivalent ETH amount, facilitating the redemption process.
-   Both the functions are similar to `getUsdAmountFromaapl` and are executed in a similar way

4. `getAccountInformationValue`

![AAPL](./public/7.png)

-   Aggregates and returns the total USD values of AAPL minted and ETH collateral for a specific user, useful for understanding a user's position and the health factor calculation.

**Private/View Functions**

1. `_calculateHealthFactor`

![AAPL](./public/8.png)

-   `aaplMintedValueUsd`: The USD value of the AAPL tokens minted by the user.
-   `collateralValueUsd`: The USD value of the ETH collateral deposited by the user.
-   If the user has not minted any AAPL tokens (aaplMintedValueUsd == 0), the function returns the maximum possible uint256 value, indicating infinite health (no debt).
-   The function calculates the adjusted collateral value based on the LIQUIDATION_THRESHOLD, ensuring the user maintains a collateralization ratio above this threshold.
-   The health factor is computed as the ratio of the adjusted collateral value to the value of minted AAPL tokens, scaled by PRECISION to maintain decimal accuracy.

2. `_getAccountInformation`

![AAPL](./public/9.png)

-   `totalaaplMinted`: The total amount of AAPL tokens minted by the user.
-   `totalCollateralEth`: The total amount of ETH collateral deposited by the user.
-   The function accesses two mappings: s_aaplMintedPerUser and s_ethCollateralPerUser, using the user's address as the key.
-   It retrieves and returns the total amounts of AAPL tokens minted and ETH collateral deposited by the specified user.

## Auditing Process for Tokenization of Real-World Assets

Tokenizing real-world assets on the blockchain involves creating digital representations of physical or non-physical assets (such as stocks, bonds, commodities, or real estate) through tokens. This process requires rigorous security, legal compliance, and accurate representation of asset values through reliable data feeds. The use of oracles and off-chain data sources is central to ensuring that the token values reflect the real-world prices and attributes of the assets they represent.

1. Security Audit:

-   Code Review: Thorough examination of the smart contract code for security vulnerabilities such as reentrancy attacks, overflow/underflow errors, and improper access controls.
-   Architecture Review: Ensuring that the contract structure and data flows are secure against potential threats and that the system architecture supports robust handling of edge cases.

2. Oracle Reliability and Data Integrity:

-   Oracle Choice and Implementation: Evaluation of the oracles and data sources used for accuracy and resistance to manipulation.
-   Fallback Mechanisms: Assessment of mechanisms in place for handling oracle failures or discrepancies in data feeds.

3. Compliance and Legal Review:

-   Regulatory Compliance: Ensuring the tokenization process adheres to local and international regulations concerning asset tokenization and digital securities.
-   Tokenomics and Rights Attached: Verification that the tokens accurately represent the underlying assets in terms of ownership, dividends, voting rights, etc.

4. Functional Testing:

-   Unit Testing: Detailed tests for each function to ensure they perform as expected under various conditions.
-   Integration Testing: Testing the contract’s interactions with external contracts and services like oracles.
-   Scenario Testing: Simulating different operational scenarios to test how the contract behaves under unusual or extreme conditions.

5. Performance and Gas Efficiency:

-   Optimization Review: Ensuring that the contract operations are optimized for gas efficiency, which is crucial for scalability and user costs.
-   Load Testing: Assessing the contract’s performance under high transaction volumes.

6. User Role and Access Control:

-   Permissions and Roles: Ensuring that functions are accessible only to authorized users and that roles are clearly defined and enforced within the contract.

#### Specific Audit of the Provided Smart Contract

Now, let’s apply this auditing framework to the provided AAPL smart contract:

1. Security Audit

-   Reentrancy: The functions `depositAndmint` and `redeemAndBurn` are susceptible to reentrancy attacks, especially since they involve transferring ETH. This should be mitigated by using the checks-effects-interactions pattern.

2. Compliance and Legal Review

-   Token Representation: The contract mints tokens representing shares of Apple, which are securities. This requires compliance with securities regulations, including but not limited to the SEC in the U.S. or equivalent bodies elsewhere.
-   Rights and Obligations: There is no code managing dividends or other rights typically associated with stock ownership. This aspect might need to be integrated or clearly defined off-chain.

3. Functional Testing

-   Unit and Integration Testing: Ensure comprehensive coverage, including scenarios where the oracle feeds provide unexpected values.
-   Edge Case Handling: More tests are needed around the limits of minting and redemption, especially under fluctuating oracle values.

4. Performance and Gas Efficiency

-   Gas Cost Analysis: Functions like `depositAndmint` and `redeemAndBurn` involve multiple state changes and external calls, which can be gas-intensive. Optimization might be required.

5. User Role and Access Control

-   Access Controls: The contract currently does not implement any special access controls beyond the typical ownership patterns. Depending on the business model, you might need role-based access control mechanisms.

### Integration of Fuzz Testing in the Audit Process

Purpose: Fuzz testing is critical for identifying hidden issues that are not obvious during regular testing phases. It helps in detecting vulnerabilities like buffer overflows, crashes, memory leaks, and handling of unexpected or malicious inputs.

Process: Fuzz testing involves providing random data (inputs) to the smart contract functions to observe their behavior and track how well the contract handles edge or error cases.

Tools: In the Ethereum ecosystem, tools like Echidna and Foundry (with its forge fuzz command) are popular for conducting fuzz tests on smart contracts.

### Application to the AAPL Smart Contract

For the `AAPL` smart contract, incorporating fuzz testing would mean:

1. Target Functions: Functions like depositAndmint and redeemAndBurn, which are crucial and involve significant state changes and financial calculations, are ideal candidates for fuzz testing.
2. Scenario Creation: Generate inputs to cover a range of possible values for amounts to mint and redeem, ensuring the testing covers edge cases like zero inputs, extremely high values, and values that are borderline acceptable for minting and redemption based on the current oracle price feeds.
3. Oracle Mocking: To effectively fuzz test depositAndmint and redeemAndBurn, you would also need to simulate various responses from the oracle (e.g., high, low, rapidly changing, and static prices) to see how the contract handles these scenarios.

#### Why Include Fuzz Testing in the Audit

1. Coverage: Fuzz testing expands the test coverage by exploring paths that are not typically considered during standard testing, increasing the confidence in the contract’s reliability and security.

2. Automation: Fuzz tests can be automated and run continuously as regression tests, helping catch issues that might be introduced as the contract evolves.

3. Complexity Handling: Contracts interacting with external data sources like oracles can behave unpredictably. Fuzz testing helps ensure that the contract can handle such complexity and variability without failing.
