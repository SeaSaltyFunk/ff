---
description: Fixed Forex Assets Overview
---

# ibXXX Assets Explained

## Utility of ibXXX Assets

ibXXX Assets can be utilized as explained in the [Fixed Forex Use Case Section](../getting-started/fixed-forex-use-cases.md). Further appeals of ibXXX are;

* To hold assets that are not exposed to the same variability in value as other (volatile) assets, for example; $wBTC, $ETH, $KP3R etc.
* To gain exposure to stable assets that aren’t based on a peg with USD (for example, to invest in on-chain opportunities without having to have exposure to USD currency fluctuations vs users fiat currency)
* To seek yield opportunities that may exceed those available to users through off-chain fiat use [Minting & Issuance Security Section](../appendix/minting-and-issuance-security.md)

## Fixed Forex & Iron Bank Responsibilities

Full details of the split in responsibilities between Fixed Forex & Iron Bank can be found in the [Minting & Issuance Security Section](https://app.gitbook.com/o/gYdgh8RgGKXRgpdzZ92w/s/dcazEWFTJX0SB3s4mSJg/\~/changes/hOewjqgeoSgzykeFBkOt/security-and-risk-appendix/minting-and-issuance-security). In simple terms the responsibilities can be described as;

* Fixed Forex;
  * Creates & owns level of supply of ibXXX Assets deposited into Iron Bank Ethereum supply markets via the [ib Controller Contract](../developers/contract-addresses.md#system-contracts) which is owned by the [Multisig](../governance/multisig.md). The level of supply directly impacts rate of interest applied to supply or borrow markets
* Iron Bank;
  * Creates & owns the supply & borrow markets (i.e. what assets are available for lending). A full list of assets available as collateral can be found [here](https://docs.ib.xyz/lending-market/collateral-factor)
  * Maintains Price Oracles, as per [Iron Bank documentation](https://docs.ib.xyz/v/ethereum/lending-market/price-oracle)
  * Controls the [interest rate model mechanisms](https://docs.ib.xyz/lending-market/interest-rate-model) applied to supply & borrow markets

## How ibXXX Assets are issued to users

ibXXX Assets borrowing is restricted to the following conditions;

* ibXXX Assets can **ONLY** be borrowed from Iron Bank
* ibXXX Assets can **ONLY** be borrowed where borrower has provided an accepted form of collateral

ibXXX Assets **CANNOT** be used as collateral to borrow any other assets within Iron Bank markets

## ibXXX Asset Value

ibXXX Asset valuation within Iron Bank markets is based on fiat price Oracle Feeds.

This means that Iron Bank always values each borrow as equal to the fiat price feed. For example, 100 $ibEUR borrowed will be valued using a EUR/USD Price Oracle

Since each ibXXX Asset borrowed is backed by collateral, and overcollateralization is a requirement of borrowing, then each ibXXX Asset is backed by a collateral of a higher value than the outstanding borrowed amounts. Where variable valuation of collateral is a factor, suppliers of collateral are at risk of liquidation

### Reserve Mechanisms

Iron Bank maintains a Reserve Ration of 10% on all borrows of ibXXX Assets, which is funded by a portion of interest paid by the borrower&#x20;

Reserve Factor information is available within the Iron Bank documentation. Actual reserve live data can be viewed at each Iron Bank ibXXX Asset information page listed under the "Reserve" section here;

* [$ibEUR](https://app.ib.xyz/markets/Ethereum/0x00e5c0774A5F065c285068170b20393925C84BF3)
* [$ibCHF](https://app.ib.xyz/markets/Ethereum/0x1b3E95E8ECF7A7caB6c4De1b344F94865aBD12d5)
* [$ibGBP](https://app.ib.xyz/markets/Ethereum/0xecaB2C76f1A8359A06fAB5fA0CEea51280A97eCF)
* [$ibAUD](https://app.ib.xyz/markets/Ethereum/0x86BBD9ac8B9B44C95FFc6BAAe58E25033B7548AA)
* [$ibJPY](https://app.ib.xyz/markets/Ethereum/0x215F34af6557A6598DbdA9aa11cc556F5AE264B1)
* [$ibKRW](https://app.ib.xyz/markets/Ethereum/0x3c9f5385c288cE438Ed55620938A4B967c080101)

### Impact for users acquiring ibXXX assets to repay outstanding borrows

This means that where borrowers are able to acquire ibXXX assets via a DEX then the following scenarios apply;

* ibXXX acquired at _**less than**_ the value of the fiat - then the borrower will be able to pay back their outstanding borrow at a discount
* ibXXX acquired at _**more than**_ the value of fiat - then the borrower will pay back their outstanding borrow at a premium

