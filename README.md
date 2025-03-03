# Building your first hook

A really simple onchain "points program"

Assume we launch some memecoin - TOKEN

we set up a pool for ETH/TOKEN

We're gonna issue points for every time somebody buys TOKEN with ETH
We're gonna issue points everytime somebody adds liquidity to the pool

## How many points to give out?

For every swap, we will give out (20% of the value in ETH) as points
e.g. if somebody sells 1 ETH to buy "TOKEN", they will get 0.2 POINTS

For add liquidity, we'll keep it 1:1 for ETH added

## How are these points represented?

Separate ERC-20 token, call it POINTS, minting POINTS to people who do those above things

(1) - issue points everytime somebody swaps to buy TOKEN for ETH

we will issue points proportional to amount of ETH being spent in the swap

HOW Much ETH is being spent in the swap => we only know this for sure AFTER the swap has happened

afterSwap
(2) - issue points everytime somebody adds liquidity

afterAddLiquidity
