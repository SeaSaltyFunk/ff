---
description: Tokenomics of $KP3R explained
---

# $KP3R Tokenomics

## Monetary Policy

$KP3R has an inflationary supply, creating new token emissions through isolated liquidity mints. These are distributed in the following ways;

1. The creation of new $KP3R distributed as Options Liquidity Mining Rewards for incentivizing liquidity of Fixed Forex Assets
2. The creation of new $KP3R distributed to vested token holders as Options Liquidity Mining Rewards
3. The creation of new $KP3R via the Keep3r Network credit minting process

Each isolated liquidity mint has a weekly cap target, which is controlled & reviewed through governance power by a Multisig. Currently, these are;

* Keep3r Jobs - limit of up to 1k $KP3R per week
* Fixed Forex Asset liquidity incentives - ~~limit of up to 1k $KP3R per week~~ (_Currently on hold due to_ [_discovery of vulnerability in GaugeProxyV2 Contract_](https://twitter.com/thekeep3r/status/1575459785214169088?s=20\&t=bcNOc5SYI5wD0rKQ-usuYQ))
* Vested Token Holders - ~~limit of up to 1k $KP3R per week~~ (_see above_)

_Note; actual new mint & emissions may vary & skew lower or higher each week._

Governance of new liquidity mints is controlled by the Multisig. For more detail on Multisig responsibilities please check the [Governance Section](broken-reference)

Additionally, the Multisig may optionally mint new $KP3R for utilizing treasury funds to sustain growth of the protocol

## Token Supply

### Circulating Supply

Circulating supply can be derived by determining the total amount of $KP3R either;

* Bonded by Keep3rs within the Keep3r Network (Total Bond amount can be viewed [here](https://keep3r.network/stats))
* Vested by $KP3R holders within Fixed Forex (Total Vested amount can be viewed [here](https://dune.com/ChainsightAnalytics/Fixed-Forex))

Sum of total $KP3R locked in both mechanisms should then be deducted from the Total Supply to arrive at Circulating Supply

$$
Circulating Supply = Total Supply - (BondedKP3R +VestedKP3R)
$$

### Max Supply

$KP3R has no hard cap on maximum supply, similar to Ethereum. Total token supply will increase as a product of time. Vested token holders are compensated for dilution through the distribution of fees from OLM revenues & through the issue of $rKP3R rewards

### Total Supply

Total supply can be tracked within the [$KP3R token smart contract](https://etherscan.io/token/0x1ceb5cb57c4d4e2b2433641b95dd330a33185a44) or [visualized via this Dune Analytics query](https://dune.com/embeds/1265393/2168062/2b0801ff-d0c8-447d-bcc5-c941b43f9e91)

Total supply is expected to grow over time due to Monetary Policy of the protocol & no cap on maximum supply

## Distribution at Launch

$KP3R was distributed at launch as a "fair launch" meaning all participants had the same ruleset with no allocations to team, influencers, or seed rounds, etc. Tokens were distributed to participants based on use of the Keep3r and Fixed Forex protocols

## Value Capture

Fixed Forex generates ongoing revenues, a share of which is converted to $ibEUR and distributed to $vKP3R holders. For more details on how what & how fees are distributed please see the [Benefits of Vesting Section](../vesting/benefits-of-vesting.md)

Value is captured from the following ongoing revenue-generating activities;

* Fixed Forex Minting & Reserve Fees
* Options Liquidity Mining Redemptions
* Protocol Owned or Managed Liquidity
* Swap Fees from exchanges between Fixed Forex Assets
