# XRP Ledger (XRPL) APIs.json Profile

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
