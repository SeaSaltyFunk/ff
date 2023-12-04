---
description: Access ibXXX Assets through swapping on fixedforex.fi/swap
---

# Fixed Forex's AMM

## Acquiring ibXXX without Borrowing

It is possible for users to acquire ibXXX without borrowing, this is possible by Fixed Forex hosting a limited AMM that allows swaps from a shortlist of approved Assets to ibXXX

### Approved Assets

Users can swap to any of the ibXXX asset types by providing any of the following approved Assets at [fixedforex.fi/swap](https://fixedforex.fi/swap);

* $DAI

This swap functionality is available for operation at all times

## Swapping out of ibXXX Assets

It is possible for users to swap from ibXXX back to a limited set of non-Fixed Forex Assets via the AMM. Swaps to the following Assets are possible;

* $sAUD
* $sCHF
* $sEUR
* $sGBP
* $sJPY
* $sKRW
* $sUSD

This swap functionality is **ONLY** available during limited hours of operation. This is due to utilization of Atomic Exchange features of Synthetix Forex Assets & a dependency on the Oracles used within this process.&#x20;

Users can check status of markets on [Synthetix site ](https://synthetix.io/synths)(indicated with either "Live" or "Paused" status) - check L1 Synths, Forex.

## Swapping between ibXXX Assets

This functionality is not currently available

## How to use Fixed Forex's AMM

Users wishing to swap Assets must visit the [Fixed Forex site Swap page](https://fixedforex.fi/swap), ensuring that wallet is connected and the Ethereum network is selected, then complete steps below;

* Select appropriate From & To Assets from the options available
* Approve Assets & confirm transaction in connected wallet
* Swap Assets & confirm transaction in connected wallet

Successful completion of steps will result in desired Asset being provided to users

## Fees & Slippage

Fixed Forex's AMM aims to provide low slippage between Asset swaps with low transaction fees. Details of slippage, dependencies & fees is included in the table below;

| Swaps between Assets | Slippage & Dependancies              | Fees                                                           |
| -------------------- | ------------------------------------ | -------------------------------------------------------------- |
| $DAI to $ibXXX       | No Slippage                          | 0.30%                                                          |
| $sXXX to $sXXX       | No Slippage                          | 0.05% - 0.10%                                                  |
| $ibXXX to $sXXX      | Yes, dependant on Curve pool balance | As per Curve and/or Synthetix fees (dependant on swap routing) |
| $sXXX to $ibXXX      | Yes, dependant on Curve pool balance | As per Curve and/or Synthetix fees (dependant on swap routing) |
