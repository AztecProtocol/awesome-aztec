# Awesome Aztec

A curated list of resources for learning and programming the Aztec blockchain.

⚠️ This repository or the contained links are not endorsed as safe and secure by Aztec Labs or the Noir team. Users are advised to exercise caution before utilizing any content or code provided herein.

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/aztecnetwork.svg?style=social&label=Follow%20%40aztecnetwork)](https://twitter.com/aztecnetwork)
[![Discord](https://img.shields.io/badge/discord-join%20chat-blue.svg)](https://discord.com/invite/aztec)
[![Telegram](https://img.shields.io/endpoint?color=neon&logo=telegram&label=chat&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2FAztecAnnouncements_Official)](https://t.me/AztecAnnouncements_Official)

## Official Resources

- [Website](https://aztec.network/)
- [Docs](https://docs.aztec.network/)
- [Aztec Starter](https://github.com/AztecProtocol/aztec-starter/tree/next/)
- [Forum](https://discourse.aztec.network/)
- [Github](https://github.com/AztecProtocol)
- [Awesome Noir](https://github.com/noir-lang/awesome-noir/tree/main#benchmarks)
- [Blog](https://aztec.network/blog)

## Learning

### Talks and workshops

- [Inside Aztec Labs Youtube playlist](https://www.youtube.com/playlist?list=PLabpoAlaCBY2-sW1C8UDo16SRaMNFrnt1) - Includes videos reviewing Private Transactions, the kernel circuit, Noir Contract Syntax, Cross-chain communication and tree data structures.
- [Intro to Aztec.nr](https://www.youtube.com/watch?v=58YWjQe6Cqs&list=PLabpoAlaCBY0XuHR5q3jKqKGYWbP4fDeU) - An introductory workshop for Aztec.nr, the smart contract framework for Noir contracts written on Aztec.
- [Privacy Preserving Smart Contract Architectures](https://www.youtube.com/watch?v=09nDPDN1ORA) - Zac Williamson, the co-founder and CEO of Aztec Labs, explores how to enable encrypted programmable blockchain networks with strong privacy guarantees. 
- [Private-Public Composability](https://www.youtube.com/watch?v=7Oc0tjdbi70&t=17723s)
- [How to build a SNARK](https://www.youtube.com/watch?v=j6wlamEPKlE) - Zac Williamson
- [An Intro to Aztec Smart Contract Development](https://youtu.be/93pfZMjKMmQ) - Ciara Nightingale

### Blog Posts and Articles

- [WTF is Aztec?](https://aztec.network/blog/wtf-is-aztec)
- [Aztec’s Transaction Anatomy](https://aztec.network/blog/aztecs-transaction-anatomy/)
- [Privacy Abstraction with Aztec](https://aztec.network/blog/privacy-abstraction-with-aztec/)

### Tutorials

- [Local network quickstart](https://docs.aztec.network/getting_started)
- [Write a counter contract](https://docs.aztec.network/developers/docs/tutorials/contract_tutorials/counter_contract)
- [Write a token contract](https://docs.aztec.network/developers/docs/tutorials/contract_tutorials/token_contract)
- [Bridging to Aztec](https://docs.aztec.network/developers/docs/tutorials/js_tutorials/token_bridge)
- [Aztec Contracts 0–100](https://medium.com/@niallinio/aztec-contracts-0-100-905fe41bf998)
- [Learn Aztec](https://github.com/taurushq-io/private-CMTAT-aztec/blob/master/LEARN-AZTEC.md) by Taurus
- [How to use Aztec Packages and Aztec Docs](https://gist.github.com/rajeshb62/60a7018d97124b5644d84c4f3ea5cc18)
- [Play the Glass Bridge Game (ZK Tutorial)](https://zkdev.net/docs/tutorial/glass-bridge)
- [Aztec Personal AI Tutor](https://github.com/Atunde-SS/Aztec-AI.git)

## Coding

### Examples

- [Aztec Examples Repo](https://github.com/AztecProtocol/aztec-examples/tree/main)
  - Built and maintained by the Aztec devnrel team
- [Smart Contract Examples](https://github.com/AztecProtocol/aztec-packages/tree/next/noir-projects/noir-contracts)
  - Built and maintained by the Aztec engineering team
  - This is the best place to find smart contracts that are up-to-date with the latest changes
- [Aztec Standards](https://github.com/defi-wonderland/aztec-standards)
  - Smart contracts, built and maintained by the Wonderland team, with both e2e tests in JavaScript and unit tests written in Aztec.nr
- [Private OTC Desk](https://github.com/aztec-pioneers/aztec-otc-desk/tree/main)
  - Great example of a more complex app with Aztec smart contracts including multiple wallets (PXEs), tests, Aztec.nr, Aztec.js as more 
- [GregoSwap demo app](https://gregoswap.anothercoffeefor.me/)
  - Wallet SDK demo app, [code here](https://github.com/AztecProtocol/gregoswap)
- [Helpful scripts](https://github.com/AztecProtocol/aztec-starter/tree/next/scripts)
  - How to do common actions like deploying & interacting with contracts

### Dev Tools

- [Aztec version of the Noir programming language](https://docs.aztec.network/guides/smart_contracts/writing_contracts/initializers) - for writing smart contracts on Aztec
- [Noir VS Code extension](https://marketplace.visualstudio.com/items?itemName=noir-lang.vscode-noir) - Syntax highlighting, snippets and more for Noir.
- [aztec.tools](https://aztec.tools) - collection of handy tools for Aztec development in the browser.
- [Aztec Test Runner](https://github.com/marketplace/actions/aztec-test-runner) - a Github Action for running TXE tests in your CI
- [Remix IDE Plugin for Aztec](https://github.com/hsy822/aztec-remix-plugin) - a plugin for Remix IDE to compile, deploy, and interact with Aztec smart contracts.
- [Demo wallet](https://github.com/AztecProtocol/demo-wallet) -  An Aztec wallet application (designed for devs) that allows dApps to interact with user accounts through a secure interface
- [Aztec MCP Server](https://github.com/critesjosh/aztec-mcp-server) - An MCP (Model Context Protocol) server that provides local access to Aztec documentation, examples, and source code through cloned repositories.
- [Aztec Claude Code Plugin](https://github.com/critesjosh/aztec-claude-plugin) - A Claude Code plugin for Aztec smart contract and application development. 

### Boilerplates

- [Aztec Starter](https://github.com/AztecProtocol/aztec-starter) - A starting point for writing Aztec contracts and tests (and learning!)
- [Aztec web starter](https://github.com/AztecProtocol/aztec-web-starter) - an example web app that demonstrates how to interact with an Aztec contract using the Aztec JS SDK
- [Next.js Starter](https://github.com/raven-house/aztec-nextjs-starter) - Next.js starter template with Aztec Network integration
- [Defi Wonderland's Aztec Boilerplate](https://github.com/defi-wonderland/aztec-boilerplate) - similar to Aztec starter, but includes benchmarking on PRs
- [Aztec Boxes](https://github.com/AztecProtocol/aztec-packages/tree/master/boxes) - A collection of boilerplates for building with Aztec
  - [Install local network](https://docs.aztec.network/developers/getting_started_on_local_network)
  - run `aztec-cli unbox [box_name] [new_project_name]`

### Libraries

- [Aztec.nr docs](https://docs.aztec.network/guides/smart_contracts/writing_contracts/initializers) and [source code](https://github.com/AztecProtocol/aztec-packages/tree/master/noir-projects/aztec-nr)
  - Includes:
    - [`aztec`](https://github.com/AztecProtocol/aztec-packages/tree/master/noir-projects/aztec-nr/aztec) (core) - the core of the framework
    - [`easy-private-state`](https://github.com/AztecProtocol/aztec-packages/tree/master/noir-projects/aztec-nr/easy-private-state) - for easily creating private state
    - [`value-note`](https://github.com/AztecProtocol/aztec-packages/tree/master/noir-projects/aztec-nr/value-note) - for storing arbitrary values
- [Noir libraries](https://github.com/noir-lang/awesome-noir/blob/main/README.md#libraries) - can be used in Aztec contracts
- [Aztec Storage proofs](https://github.com/nemi-fi/aztec_storage_proofs) - Prove Aztec note inclusion in plain Noir. Generate verifiable proofs for verification in JS or Solidity.

### Contract development

- [Contract state](https://docs.aztec.network/developers/reference/smart_contract_reference/storage/private_state)
- [Functions](https://docs.aztec.network/developers/docs/aztec-nr/framework-description/functions)
- [Compiling contracts](https://docs.aztec.network/developers/docs/aztec-nr/how_to_compile_contract)
- [Deploying contracts](https://docs.aztec.network/developers/docs/aztec-js/how_to_deploy_contract)
- [Portal contracts](https://docs.aztec.network/developers/docs/aztec-nr/framework-description/ethereum-aztec-messaging) - portal contracts enable L1<>L2 communication

### Common Patterns

- [Defi Wonderland Aztec standards](https://github.com/defi-wonderland/aztec-standards) - Aztec Standards is a compilation of reusable, standardized contracts for the Aztec Network.
  - [Token standard](https://github.com/defi-wonderland/aztec-standards?tab=readme-ov-file#token-contract) - The Token contract implements an ERC-20-like token with Aztec-specific privacy extensions.
- [Calling public function from private functions](https://docs.aztec.network/developers/docs/aztec-nr/framework-description/how_to_call_contracts#private-to-public-calls) - private functions cannot directly manipulate public state, they can by staging a call to a public function that updates public state.
  - You can also use this pattern to "pass" public inputs into private state by passing the input as an argument to a private function, staging a public function call that validates the input against the current public state.

### Projects

- [Obsidion](https://obsidion.xyz/) - Mobile wallet
- [Azguard](https://azguardwallet.io/) - Browser wallet
- [Nemi](https://nemi.fi) - AMM: swap tokens with privacy
- [RavenHouse](https://www.ravenhouse.xyz/) - NFT Marketplace and NFt private ownership verification.
- [(Experimental) NFT Standards](https://github.com/resurgencelabs/nft_standards)
- [Private subscription service](https://github.com/resurgencelabs/ikigai_backend)
- [Tezac](https://github.com/0xandee/tezac/) - Privacy-preserving NFT marketplace

## Reference

- [Private Execution Environment (PXE) API Reference](https://docs.aztec.network/developers/reference/aztecjs/pxe/interfaces/pxe)
- [Current Limitations](https://docs.aztec.network/developers/reference/considerations/limitations)
