# tokenomics for farmers of grid 1.0

Farmers on grid 1.0 had slightly different farming rules compared to v2.0.

In v2.0 we made following changes to improve the tokenomics (economics of the token)
The basic idea is to lower the max amount of TFT which will result in more long term stability and growth potential for the token.

- difficulty level not determined by guardians (people chosen by community) but now build into the farming code
    - in 2.0 difficulty level goes up in relation to nr of TFT
- introduction of burning of TFT
    - to limit the amount of TFT, we introduce burning of TFT
    - in v2.x farmers get 50% of the TFT used to buy capacity in the TF Grid (40-45% burned, 10-5% to foundation)
- foundation gets less tokens: 
    - after 2 years goes to only 5%, was 10% to promote the grid and keep development going
- maximum amount of TFT is now 2 Billion 
    - was 100 Billion before
    - nr of tokens limited thanks to the difficulty level going up and burning of tokens
- the difficulty level and price of TFT was set at connection time, this is now calculated every farming month

## what about TFT already made on 1.0 grid

- In grid 2.0 we use the Stellar blockchain to track our tokens in stead of our own now legacy blockchain called TFChain (based on our tech Rivine)
- April 30 the TFT will launch on Stellar blockchain and some new public exchanges.
- 1.0 Grid token holders will be able to convert from TFChain to Stellar starting April 30 2020
- the 1.0 Grid tokens will be called TFTA on Stellar.
- the 2.0 Grid tokens are called TFT.
- starting July 1, TFTA can be sold as TFT on Stellar using a digitized market maker.

## digitized market maker

- Untill end 2020, TFTA can only be sold if price is higher than the min TFT price compared to USD.
- min TFT price by the market maker is USD 0.15 starting April 30, going up 4% per month in relation to the gold price.
- End 2020, all TFTA get converted to TFT at same conditions as on TFTA chain (same lockup periods), which means TFTA stops to exist.
- Every TFTA holder can place sell orders on the digitized market maker bot, only 1 can be open at the same time.
- The digitized market maker bot will sell per USD 20k into the market and sales done get's distributed evenly over the sell orders in the order book.
- As long as price is higher than the minimum price the digitized market maker bot will keep on selling if orderbook is not empty.
- TFTA holders can set the sales price (min sales price) or they can sell at market.
- The sales orders are always done versus XLM which is the native Stellar currency which will also till 6 levels deep sell to other currencies like BTC, ETH, ...
    - this means if someone wants to buy TFT for BTC, it will still work, Stellar paymnet network will convert to XLM then to TFT
    
