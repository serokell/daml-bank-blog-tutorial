<!--
   - SPDX-FileCopyrightText: 2026 Serokell <https://serokell.io>
   -
   - SPDX-License-Identifier: MPL-2.0
   -->

# daml-bank-blog-tutorial

[![License: MPL 2.0](https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg)](https://opensource.org/license/MPL-2.0)

A minimal bank ledger written in [Daml](https://docs.canton.network), companion code for the [Serokell blog post on Daml smart contracts](https://serokell.io/blog).

The example models accounts, peer-to-peer transfers with an accept/reject workflow, and bank-driven settlement, all expressed as Daml templates and choices.

## Install

You need the [Daml SDK](https://docs.daml.com/getting-started/installation.html) version 3.5.1 or later.

```bash
dpm build --package-root main
```

## Usage

Run the Daml Script tests to see the workflows in action:

```bash
dpm test --package-root test
```

The `testTransfer` script walks through Alice transferring 10 to Bob, Bob accepting, and the bank settling the transaction.

## Contributing

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more information.

## License

[MPL-2.0](LICENSE) © [Serokell](https://serokell.io)

## About Serokell

daml-bank-blog-tutorial is maintained and funded with ❤️ by [Serokell](https://serokell.io/).
The names and logo for Serokell are trademark of Serokell OÜ.

We love open source software! See [our other projects](https://serokell.io/projects?utm_source=github) or [hire us](https://serokell.io/contacts?utm_source=github) to design, develop and grow your idea!
