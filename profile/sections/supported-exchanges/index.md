[< Back](../../README.md#sections)

# Supported exchanges

| Exchange (ID)                                        | Window  | Liquidity | Coins   | Trading |
| ---------------------------------------------------- | ------- | --------- | ------- | ------- |
| [**Binance (binance)**](https://www.binance.com/)    | &check; | &check;   | &check; | &check; |
| [**Bitfinex (bitfinex)**](https://www.bitfinex.com/) | &check; | &check;   | &check; | &cross; |
| [**Coinbase (coinbase)**](https://www.coinbase.com/) | &cross; | &cross;   | &cross; | &cross; |
| [**Kraken (kraken)**](https://www.kraken.com/)       | &check; | &check;   | &check; | &cross; |
| [**OKX (okx)**](https://www.okx.com/)                | &cross; | &cross;   | &cross; | &cross; |

### Binance Users

- ...

### Bitfinex Users

- ...

### Kraken Users

- Unlike other exchanges, the rate limits on Kraken are very strict. Therefore, when setting the `Re-fetch frequency (seconds)` field in the Window Configuration ensure to set a value larger than 10 seconds to avoid hitting rate limits.

- When the Kraken implementation was being developed, the trading pairs making use of **USDT** had very low volume compared to pairs making use of **USD**. If you wish to use of **USD** make sure to set it in the `EXCHANGE_CONFIGURATION.quoteAsset` environment variable.
