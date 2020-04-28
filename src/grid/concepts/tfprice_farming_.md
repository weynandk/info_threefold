## TFT Price for Start of TF Farming

The TFT Price at the start of farming defines the total (possible) amount of TFT’s minted by the farmer equipment for the 60 month period. Historically the TFT pricing has been:
*   TFT price from 1st of April 2018 until the 31st of December 2018:		USD 0.10
*   TFT price from 1st of January 2019 until the 31st of January 2020:	USD 0.12
*   TFT price from 1st of February 2020:					USD 0.15

After the Token Listing Event (which is approximately end of March 2020) the TFT price for the start of farming will be calculated as the weighted average of the last 3 months periods of TFT traded on public exchanges. The 10% highest and 10% lowest weighted token trades will not be used for calculating the TFT price for start of farming. This should eliminate the extremities in trading patterns. The TFT Price for the start of farming will be rounded to the 4th digit after the comma. This TFT price will be calculated after the end of the first 3 periods of 2020 and is valid for the following 3 periods. The first TFT price for farming will be calculated on March 31st 2020.

### Simple trading period example to explain the concept

Consider the following trades for an example period of three month:.

| Trade | Token Volume | Token Price [USD] |
| ---- | ---- | ---- |
| 1	| 10,000 | 0.25 |
| 2 |	1,000 | 0.12 |
| 3 |	500 | 0.15 |
| 4 |	2,000 | 0.16 |
| 5 |	300 |	0.15 |
| 6 |	3,000 |  0.17 |
| 7 |	9,000 |	 0.20 |
| 8 |	1,000 | 0.15 |
| 9 |	500 | 0.16 |
| 10 | 1,000 | 0.18 |

This would read as follows in a graph showing the token pricing vs. the trade volume.

![](./img/trade_graph.png)

In this period a total of 28,300 tokens were traded. Trade 1 traded at the highest price (0.25 USD) and trade 2 (0.12 USD) at the lowest price. In order to cut 10% of the tokens traded at the highest price and 10% of the lowest price we have to organise all tokens traded in a sequence from high to low.

Once we have organised all single tokens trades in a sequence we can quite easily cut 10% of highest traded token and lowest traded tokens.  See the red markers in the graph.  Please note that in this example the 10% of highest price traded tokens fits into a single trade while the 10% of lowest price traded tokens spans 5 trades.  Remember that these are just example trades, it might be the reverse in real life where high price trades represent lower volumes and low price trades higher volumes, but the principles stay the same.

![](./img/tokens_traded_organised.png)

See table below where the token trades have been ordered from the highest price to the lowest and where we take out both 10 percentiles:

![](sorted_trade_examples.png)

So for the coming 3 months period the token price for new farming equipment will be set at the weighted average token price of 0.2066 USD.

