# threefold marketmaker bot

While potentially the name is misleading, because this bot does not have funding to keep a market stable, 
this bot has as goal to allow any TFTA token holder to sell tokens to the Stellar network in way that price stability gets maintained.

Technical detail: the original Rivine TFT’s are going under name TFTA on the Stellar blockchain until the end of 2020. Starting 2021 this name difference will go away, do note that a TFTA or TFT is the same. Jan 2021, all TFTA get converted into TFT at same conditions on TFTA chain (same lockup periods), which means TFTA stops to exist, users will have to ask this conversion on TF Wallet.

The TFT bot market maker is a digitized bot. We choose to do this through our own digitized bot because a 3rd party bot service costs 20k USD per month.

All TFTA holders can sell as much as they want starting June 1, 2020 through the TFT market maker bot as long as the price of the TFT is high enough & there is liquidity on the market.

The rules the bot maintains are as follows:

- Until the end of 2020 TFTA can only be sold if the sell price is higher than the min TFT price.
- Min TFT price by market maker is USD 0.15 starting april 29, going up 2% per month compared to the USD, in the unexpected event that the USD would become unstable then the gold price will be used.
- Every TFTA holder can place sell orders on the digitized market maker bot, only 1 order can be open at the same time per TFTA holder. There is no limit to the size of the order.
- The digitized market maker bot will sell per USD 20k onto the market and sales done gets distributed evenly over the sell orders in the order book. 
- As long as the price is higher than the minimum price the digitized market maker bot will keep on selling until the order book is empty.
- TFTA holders can set the sales price (min sales price) or they can sell at market. 

### remarks

- The sales orders are always done versus XLM which is the native Stellar currency
- It's very easy for everyone in the world to buy XLM and as such buy TFT.
- The Stellar network allows you to sell to other currencies like BTC, ETH, ... up to 6 levels deep. 
- This means if someone wants to buy TFT for BTC, it will still work, Stellar payments network will convert to XLM and then to TFT. 



