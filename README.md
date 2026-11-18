Token metadata for Soda Labs wallets.

To the extent possible under law, Soda Bubble Labs LTD has waived all copyright
and related or neighboring rights to this token metadata. See LICENSE (CC0 1.0
Universal).

The data is published this way so wallets, explorers and aggregators can
redistribute it without attribution obligations. Token names, symbols and logos
referenced here may be trademarks of their respective owners; CC0 covers this
compilation, not those marks.

## Fields

Entries live under `tokenIcons.<chainId>.<token address>`:

- `iconUrl`: icon path or URL.
- `name`, `symbol`: display overrides; the on-chain values are used when absent.
- `coingeckoId`: CoinGecko coin id used for USD prices (e.g. `usd-coin`), on the underlying or the private entry.
  Without one, only USD stablecoins are valued (at $1).
- `default`: set `true` on a private (pERC20) token to show it on the wallet dashboard.
  Mainnet and testnet wallets read this same file, and each checks only its own chains:
  once any of its chains has a `default` token, that wallet shows only `default` tokens.
