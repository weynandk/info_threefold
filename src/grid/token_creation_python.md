
```python

class TokenCreator:


    def tft_farm(self, month, nodes_batch):
        """
        calculate the farming of tft's
        """
        return self.farming_logic.tft_farm(month)

    def tft_cultivate(self, month, nodes_batch):
        """
        calculate the nr of TFT cultivated for the full batch
        cultivation means selling of capacity which results in TFT income for farmer
        """
        tftprice_now = self.simulation.tft_price_get(month)
        revenue_usd = nodes_batch.revenue_get(month)
        return revenue_usd / tftprice_now * 0.9

    def tft_burn(self, month, nodes_batch):
        """
        burning is no part of the chosen tokenomics model
        """
        return 0

```
