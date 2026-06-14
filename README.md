# XRP Ledger (XRPL) APIs.json Profile

APIs.json 0.19 provider profile for the XRP Ledger blockchain public APIs.

## Overview

The XRP Ledger is a decentralized public blockchain with fast settlement (3-5 seconds) and low transaction fees. It provides JSON-RPC and WebSocket APIs for querying accounts, transactions, ledgers, order books, AMM pools, NFTs, payment channels, and network statistics.

Public community-operated nodes are freely available for mainnet, testnet, and devnet with no API key required.

## APIs Cataloged

| API | Protocol | Network | Base URL |
|-----|----------|---------|----------|
| XRPL JSON-RPC API | HTTP/JSON-RPC | Mainnet | https://xrplcluster.com/ |
| XRPL WebSocket API | WebSocket | Mainnet | wss://xrplcluster.com/ |
| XRPL JSON-RPC API | HTTP/JSON-RPC | Testnet | https://s.altnet.rippletest.net:51234/ |
| XRPL WebSocket API | WebSocket | Testnet | wss://s.altnet.rippletest.net:51233/ |

## Method Categories

- **Account Methods** - account_info, account_channels, account_currencies, account_lines, account_nfts, account_objects, account_offers, account_tx, gateway_balances, noripple_check
- **Ledger Methods** - ledger, ledger_closed, ledger_current, ledger_data, ledger_entry
- **Transaction Methods** - submit, submit_multisigned, transaction_entry, tx
- **Path & Order Book Methods** - amm_info, book_offers, deposit_authorized, nft_buy_offers, nft_sell_offers, path_find, ripple_path_find
- **Payment Channel Methods** - channel_verify, channel_authorize
- **Subscription Methods** (WebSocket only) - subscribe, unsubscribe
- **Server Info Methods** - fee, feature, server_info, server_state, server_definitions, manifest
- **Utility Methods** - ping, random, vault_info

## Files

- `apis.yml` - APIs.json 0.19 provider profile
- `plans/plans.yml` - API access plans (free public tier, self-hosted)
- `rate-limits/rate-limits.yml` - Rate limiting details
- `finops/finops.yml` - Cost model (API access free; on-chain fees in XRP)

## Resources

- Documentation: https://xrpl.org/docs/
- Public Servers: https://xrpl.org/docs/tutorials/public-servers
- GitHub: https://github.com/XRPLF/rippled
- Explorer: https://livenet.xrpl.org/
- Testnet Faucet: https://faucet.altnet.rippletest.net/accounts
