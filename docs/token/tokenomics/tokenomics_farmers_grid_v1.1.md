# tokenomics for farmers of grid 1.0

Farmers on grid 1.0 had slightly different farming rules compared to v2.0.

In v2.0 we made following changes to improve the tokenomics (economics of the token)
The basic idea is to lower the max amount of TFT which will result in more long term stability and growth potential for the token.

- difficulty level not determined by guardians (people chosen by community) but now build into the farming code
    - in 2.0 difficulty level goes up in relation to nr of TFT in circulation
- introduction of burning of TFT
    - To ensure there is always enough TFT left to be created through farming, we introduce the burning of TFT on a certain type of transaction
    - in v2.x farmers receive only 50% of TFT from transactions paying for capacity in the TF Grid. 40-45% of those transactions is     burned, 10-5% goes to the TF Foundation)
- the TF Foundation now gets less tokens: 
    - after 2 years goes to only 5%, was 10% to promote the grid and keep development going
- maximum amount of TFT is now 2 Billion (2,000,000,000)
    - was 100 Billion before
    - The number of tokens in circulation is now limited through the difficulty level increasing exponentially 
    - The burning mechanism ensures that TFT are taken out of the circulation and can be farmed again. This incentivizes constant growth of the network.
- the difficulty level and price of TFT was set at connection time, this is now calculated every farming month.

## what about TFT already made on 1.0 grid

- In grid 2.0 we use the Stellar blockchain to track our tokens in stead of our own now legacy blockchain called TFChain (based on our tech Rivine)
- April 30 the TFT will launch on Stellar blockchain and some new public exchanges.
- 1.0 Grid token holders will be able to convert from TFChain to Stellar starting April 30 2020
- the 1.0 Grid tokens will be called TFTA on Stellar.
- the 2.0 Grid tokens are called TFT.
- starting July 1, TFTA can be sold as TFT on Stellar using a digitized market maker.

## digitized market maker

- Until end 2020, TFTA can only be sold if price is higher than the min TFT price compared to USD.
- min TFT price by the market maker is USD 0.15 starting April 30.
- End 2020, all TFTA get converted to TFT at same conditions as on TFTA chain (same lockup periods), which means TFTA stops to exist.
- Every TFTA holder can place sell orders on the digitized market maker bot, only one such order can be open per TFTA holder at the same time. Those orders comprise the TFTA internal order book.
- TFTA holders can set the sales price (min sales price) or they can sell at market.
- TFTA sold by the market maker will be traded internally against all orders in the TFTA interal order book according to their volume as long as the price realized on the public exchange matches at least the minimum price specified by the token holder.
- The digitized market maker bot will match 60-90% of all buying orders on public exchanges with selling orders.
- The sales orders are always done versus XLM which is the native Stellar currency which will also till 6 levels deep sell to other currencies like BTC, ETH, ...
    - this means if someone wants to buy TFT for BTC, it will still work, Stellar payment network will convert to XLM then to TFT
    
