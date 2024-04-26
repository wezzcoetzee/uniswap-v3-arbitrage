# Introduction

Beacuse of how decentralized finance works, there are arbitrage oppotunities that we can take advantage of. What is arbitrage? It's finding price discrepancies on different platforms for the same asset, and buying that asset at a lower price on one and selling it at a high price on another.

## Strategy

Pools are DAI / WETH

Pool A - 0.5% fee with 2000 DAI / WETH
Pool B - 0.1% fee with 2100 DAI / WETH

In this scenario, if you bought 1 WETH from Pool A and sold to Pool B you would make 100 DAI (roughly).

To do this we need to do the following:

1 - Flash swap on Pool A (receive WETH)
2 - Swap on Pool B (WETH -> DAI)
3 - Send DAI to Pool A
4 - Profit is the DAI from Pool B subtract the DAI repaid to Pool A
