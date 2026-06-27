---
title: "Introducing XRP Ledger version 3.2.0"
url: "https://xrpl.org/blog/2026/xrpld-3.2.0"
date: "2026-06-15"
feed_url: "https://xrpl.org/blog/"
---
Version 3.2.0 is a maintenance release that renames the reference server from rippled to xrpld (affecting config files and database paths), retires 30+ amendments active for over two years, and bundles bug fixes for Single Asset Vaults, the Lending Protocol, permissioned DEX, Multi-Purpose Tokens, and permissioned domains via the fixCleanup3_2_0 amendment. New capabilities include configurable NuDB block sizes (4K-32K), optional TLS/mTLS support for gRPC servers, and a server_definitions endpoint exposing transaction and ledger entry formats, flags, and account settings. The C++ codebase was modernized by renaming the ripple namespace to xrpl, adopting Conan for dependencies, and integrating clang-tidy.
