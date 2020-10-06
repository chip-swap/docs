# Chipswap Documentation

As a venue for pooled, automated liquidity provision on Binance Smart Chain, the Chipswap protocol (Chipswap) functions without upkeep, providing an unstoppable platform for BEP20 token conversion. 

Chipswap is a Uniswap-based DEX that is designed to accelerate the influencer economy.

![About](assets/about.png)

## How it works

Chipswap is an automated liquidity protocol powered by a constant product formula and implemented in a system of non-upgradeable smart contracts on the Binance Smart Chain. It obviates the need for trusted intermediaries, prioritizing decentralization, censorship resistance, and security.

Each Chipswap smart contract, or pair, manages a liquidity pool made up of reserves of two BEP20 tokens.

Anyone can become a liquidity provider for a pool by depositing an equivalent value of each underlying token in return for pool tokens. These tokens track pro-rata LP shares of the total reserves, and can be redeemed for the underlying assets at any time.

## Pricing

Pairs act as automated market makers, standing ready to accept one token for the other as long as the “constant product” formula is preserved. This formula, most simply expressed as x * y = k, states that trades must not change the product (k) of a pair’s reserve balances (x and y). Because k remains unchanged from the reference frame of a trade, it is often referred to as the invariant. This formula has the desirable property that larger trades (relative to reserves) execute at exponentially worse rates than smaller ones.

Because the relative price of the two pair assets can only be changed through trading, divergences between the Chipswap price and external prices create arbitrage opportunities. This mechanism ensures that Chipswap prices always trend toward the market-clearing price.

## Fee

In practice, Chipswap applies a 0.30% fee to trades, which is added to reserves. As a result, each trade actually increases k. This functions as a payout to LPs, which is realized when they burn their pool tokens to withdraw their portion of total reserves.

## Ecosystem

The Chipswap ecosystem is primarily comprised of three types of users: liquidity providers, traders, and developers. Liquidity providers are incentivized to contribute BEP20 tokens to common liquidity pools. Traders can swap these tokens for one another for a fixed 0.30% fee (which goes to liquidity providers). Developers can integrate directly with Chipswap smart contracts to power new and exciting interactions with tokens, trading interfaces, retail experiences, and more.

In total, interactions between these classes create a positive feedback loop, fueling digital economies by defining a common language through which tokens can be pooled, traded and used.


## Reference

