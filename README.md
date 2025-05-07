# Awesome Aztec

A curated list of resources for learning and programming in Noir.

[![Awesome](https://github.com/sindresorhus/awesome#readme/badge-flat.svg)](https://github.com/sindresorhus/awesome#readme)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/aztecnetwork.svg?style=social&label=Follow%20%40aztecnetwork)](https://twitter.com/aztecnetwork)
[![Discord](https://img.shields.io/badge/discord-join%20chat-blue.svg)](https://discord.com/invite/aztec)
[![Telegram](https://img.shields.io/endpoint?color=neon&logo=telegram&label=chat&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2FAztecProtocol)](https://t.me/AztecAnnouncements_Official)

## Official Resources

- [Website](https://aztec.network/)
- [Docs](https://docs.aztec.network/)
- [Forum](https://discourse.aztec.network/)
- [Github](https://github.com/AztecProtocol)
- [Awesome Noir](https://github.com/noir-lang/awesome-noir/tree/main#benchmarks)

## Learning

### Talks and workshops

- [Inside Aztec Labs Youtube playlist](https://www.youtube.com/playlist?list=PLabpoAlaCBY2-sW1C8UDo16SRaMNFrnt1) - Includes videos reviewing Private Transactions, the kernel circuit, Noir Contract Syntax, Cross chain communication and tree data structures.
- [Intro to Aztec.nr](https://www.youtube.com/watch?v=58YWjQe6Cqs&list=PLabpoAlaCBY0XuHR5q3jKqKGYWbP4fDeU) - An introductory workshop for Aztec.nr, the smart contract framework for Noir contracts written on Aztec.
- [Privacy Preserving Smart Contract Architectures](https://www.youtube.com/watch?v=09nDPDN1ORA) - Zac Williamson, the co-founder and CEO of Aztec Labs, explores how to enable encrypted programmable blockchain networks with strong privacy guarantees. 
- [Private-Public Composability](https://www.youtube.com/watch?v=7Oc0tjdbi70&t=17723s)
- [How to build a SNARK](https://www.youtube.com/watch?v=j6wlamEPKlE) - Zac Williamson

### Blog Posts and Articles

- [Aztec Sandbox: The Endgame for Smart Contract Privacy](https://aztec.network/blog/announcing-aztec-sandbox-the-endgame-for-smart-contract-privacy/)
- [Aztec’s Transaction Anatomy](https://aztec.network/blog/aztecs-transaction-anatomy/)
- [Privacy Abstraction with Aztec](https://aztec.network/blog/privacy-abstraction-with-aztec/)
- [Announcing Fernet: Aztec’s Decentralized Sequencer Selection Protocol](https://medium.com/aztec-protocol/announcing-fernet-aztecs-decentralized-sequencer-selection-protocol-dd06194d572f)

### Tutorials

- [Sandbox quickstart](https://docs.aztec.network/getting_started)
- [Writing a NFT Contract](https://docs.aztec.network/developers/tutorials/codealong/contract_tutorials/nft_contract)
- [Writing a Token Bridge](https://docs.aztec.network/developers/tutorials/codealong/contract_tutorials/token_bridge)
- [Aztec Contracts 0–100](https://medium.com/@niallinio/aztec-contracts-0-100-905fe41bf998)
- [Learn Aztec](https://github.com/taurushq-io/private-CMTAT-aztec/blob/master/LEARN-AZTEC.md) by Taurus
- [How to use Aztec Packages and Aztec Docs](https://gist.github.com/rajeshb62/60a7018d97124b5644d84c4f3ea5cc18)
- [Play the Glass Bridge Game (ZK Tutorial)](https://zkdev.net/docs/tutorial/glass-bridge)

## Coding

### Dev Tools

- [Aztec version of the Noir programming language](https://docs.aztec.network/guides/smart_contracts/writing_contracts/initializers) - for writing smart contracts on Aztec
- [Noir VS Code extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.vscode-noir) - Syntax highlighting, snippets and more for Noir.
- [aztec.tools](https://aztec.tools) - collection of handy tools for Aztec development in the browser.
- [Aztec Test Runner](https://github.com/marketplace/actions/aztec-test-runner) - a Github Action for running TXE tests in your CI
- [Remix IDE Plugin for Aztec](https://github.com/hsy822/aztec-remix-plugin) - a plugin for Remix IDE to compile, deploy, and interact with Aztec smart contracts.

### Boilerplates

- [Aztec Starter](https://github.com/AztecProtocol/aztec-starter) - A starting point for writing Aztec contracts and tests (and learning!)
- [Aztec Boxes](https://github.com/AztecProtocol/aztec-packages/tree/master/boxes) - A collection of boilerplates for building with Aztec
  - [Install the sandbox](https://docs.aztec.network/reference/sandbox_reference/sandbox-reference)
  - run `aztec-cli unbox [box_name] [new_project_name]`
- [Vite Starter](https://github.com/puzzlehq/aztec-sandbox-vite-starter)

### Libraries

- [Aztec.nr docs](https://docs.aztec.network/guides/smart_contracts/writing_contracts/initializers) and [source code](https://github.com/AztecProtocol/aztec-packages/tree/master/noir-projects/aztec-nr)
  - Includes:
    - `aztec` (core) - the core of the framework
    - `easy-private-state` - for easily creating private state
    - `safe-math` - for safe arithmetic
    - `value-note` - for storing arbitrary values
- [Noir libraries](https://github.com/noir-lang/awesome-noir/blob/main/README.md#libraries) - can be used in Aztec contracts

### Contract development

- [Contract state](https://docs.aztec.network/developers/reference/smart_contract_reference/storage/private_state)
- [Functions](https://docs.aztec.network/aztec/smart_contracts/functions)
- [Compiling contracts](https://docs.aztec.network/developers/guides/smart_contracts/how_to_compile_contract)
- [Deploying contracts](https://docs.aztec.network/developers/guides/smart_contracts/how_to_deploy_contract)
- [Portal contracts](https://docs.aztec.network/aztec/concepts/communication/portals) - portal contracts enable L1<>L2 communication

### Common Patterns

- [Authentication Witness](https://docs.aztec.network/guides/developer_guides/smart_contracts/writing_contracts/authwit) - authentication witnesses are like token approvals on Ethereum, but are much more flexible and powerful.
- [Calling public function from private functions](https://docs.aztec.network/developers/guides/smart_contracts/writing_contracts/common_patterns#writing-public-storage-from-private) - private functions cannot directly manipulate public state, they can by staging a call to a public function that updates public state.
  - You can also use this pattern to "pass" public inputs into private state by passing the input as an argument to a private function, staging a public function call that validates the input against the current public state.
- The list is growing quickly, see [this page of the docs](https://docs.aztec.network/guides/developer_guides/smart_contracts/writing_contracts/common_patterns) for the latest, most complete list.
- [Defi Wonderland's Aztec Patterns](https://github.com/defi-wonderland/aztec-patterns/tree/dev). Includes patterns for:
  - Shared Nullifier Key
  - Note Sharing
  - Contracts as Note Owners
  - Immediate Note Nullification
  - Callback
  - Multiparty Note-Sharing

### Projects

- [Shieldswap](https://app.shieldswap.org/) - swap tokens with privacy
- [Interface to the example token contract](https://github.com/defi-wonderland/aztec-token)
- [(Experimental) NFT Standards](https://github.com/resurgencelabs/nft_standards)
- [Private subscription service](https://github.com/resurgencelabs/ikigai_backend)
- [Tezac](https://github.com/0xandee/tezac/) - Privacy-preserving NFT marketplace

## Reference

- [Private Execution Environment (PXE) API Reference](https://docs.aztec.network/developers/reference/aztecjs/pxe/interfaces/pxe)
- [Current Limitations](https://docs.aztec.network/developers/reference/considerations/limitations)
