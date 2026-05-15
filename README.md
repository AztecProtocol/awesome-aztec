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
- [aztec-packages](https://github.com/AztecProtocol/aztec-packages) - The Aztec monorepo containing the protocol implementation, Aztec.nr framework, and reference contracts
- [AZIPs / Governance](https://github.com/AztecProtocol/governance) - Aztec Improvement Proposals and governance discussions
- [Awesome Noir](https://github.com/noir-lang/awesome-noir/tree/main#benchmarks)
- [Blog](https://aztec.network/blog)

## Learning

### Talks and workshops

- [Aztec Smart Contract Development Course](https://www.youtube.com/watch?v=cQIPG_J1W9g) - Official 5-hour course on building smart contracts with Aztec
- [Inside Aztec Labs Youtube playlist](https://www.youtube.com/playlist?list=PLabpoAlaCBY2-sW1C8UDo16SRaMNFrnt1) - Includes videos reviewing Private Transactions, the kernel circuit, Noir Contract Syntax, Cross chain communication and tree data structures.
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
- [Aztec Lint](https://github.com/NethermindEth/aztec-lint/blob/main/docs/lints-reference.md) - Nethermind's linter for Aztec contracts
- [Lampe](https://github.com/reilabs/lampe/tree/main) - Lean-based formal verification framework for Noir programs

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
- [Immutables via salt](https://aztecprotocol.slack.com/archives/C0AFUDH357F/p1772548531737649) - Wonderland's pattern for emulating immutable values using the contract salt
- [Private state & key management](https://gist.github.com/porco-rosso-j/d4ca9f3331206b5ca3b92aa79bc256bc) - Porco (Obsidion) write-up on private state variables and key management

### FPC

- [Cold start FPC design](https://gist.github.com/wei3erHase/6890bf7480f70daf5a1c4899a1d44c28) - weißer's design for cold-start Fee-Paying Contracts

### Projects

- [Obsidion](https://obsidion.xyz/) - Mobile wallet
- [Azguard](https://azguardwallet.io/) - Browser wallet
- [Nemi](https://nemi.fi) - AMM: swap tokens with privacy
- [RavenHouse](https://www.ravenhouse.xyz/) - NFT Marketplace and NFt private ownership verification.
- [(Experimental) NFT Standards](https://github.com/resurgencelabs/nft_standards)
- [Private subscription service](https://github.com/resurgencelabs/ikigai_backend)
- [Tezac](https://github.com/0xandee/tezac/) - Privacy-preserving NFT marketplace
- [Dark Forest (Aztec port)](https://github.com/dfarchon/dfpunk-aztec/tree/cherry/temp) - Aztec port of the Dark Forest game
- [Galactica zkKYC](https://github.com/Galactica-corp/aztec-zkkyc) - zkKYC implementation on Aztec
- [Galactica threshold decryption](https://github.com/Galactica-corp/aztec-v4-issue-sample) - Threshold decryption sample in Noir and TypeScript ([demo recording](https://drive.google.com/file/d/1NxH8hjfRrqeUsI-o7mUti-HidyF_kGSV/view))
- [Play](https://play.aztec-labs.com/) - Aztec Labs playground
- [Aztec Swap](https://swap.aztec-kit.anothercoffeefor.me/) - Swap UI
- [Aztec Bridge](https://bridge.aztec-kit.anothercoffeefor.me/) - Bridge UI
- [Aztec FPC](https://fpc.aztec-kit.anothercoffeefor.me/) - Fee-Paying Contract demo
- [Olla Finance Demo](https://demo.olla.finance/) - Privacy-focused DeFi demo

### Design Docs & Specs

- [BlackJack Spec](https://daffy-newsboy-a51.notion.site/BlackJack-Spec-14e2d36e9dba8018bd59e030178474cd)
- [Obsidion Portal Design Doc](https://www.notion.so/aztecnetwork/Obsidion-Portal-Design-Doc-313a1f6b0e35807f974cfaf25a8877d3)
- Wonderland Escrows — [Design](https://www.notion.so/defi-wonderland/Escrows-18c9a4c092c780c8a2c5d6a2ad6040a4) and [Background Research](https://www.notion.so/defi-wonderland/Background-Research-Escrow-2479a4c092c7805dba8fc7180352be34)
- [Selective Disclosure PoC](https://github.com/aztec-pioneers/aztec-atvs-proof) by Jack — plus an [exploratory write-up](https://hackmd.io/bVRw0Rc4TNOFy2Kfcppe3A#Diagrammed-Volume-Proof)
- [Private Stablecoin working doc](https://docs.google.com/document/d/1DNUlXpITGxV2KZQ6oaQC7AKjc5S_-AAuvpExT43vzgc/edit?tab=t.0#heading=h.4coko9c40tac)

### Explorers - Node focussed

- [Aztec Staking Dashboard](https://stake.aztec.network/) - Official Staking Dashboard by Aztec Labs
- [Validator Info](https://validatorinfo.com/networks/aztec/overview) - Blockchain Explorer and Dashboard for Aztec
- [Dashtec](https://dashtec.xyz/) - Aztec Sequencer Dashboard
- [Aztec Vision](https://aztec.vision/) - Aztec Sequencer Explorer
- [Aztec Nodes](https://aztecnodes.xyz/) - Aztec Node Map, showing geographical node distribution

### Explorers - Block focussed

- [Aztec Scan](https://aztecscan.xyz/) - Aztec Block Explorer
- [Clustec](https://clustec.xyz/) - Aztec Block & Network Health explorer
- [Aztec Explorer](https://aztecexplorer.xyz/) - Aztec Block Explroer

### Dashboards

- [Latency Explorer](https://aztecprotocol.github.io/benchmark-page-data/misc/tx-latency-explorer/) - Transaction latency benchmarks
- [Aztec Governance Dashboard](https://aztecgov.nethermind.io/) - Nethermind's governance dashboard
- [Dashtec Governance](https://dashtec.xyz/governance) - Governance view on Dashtec

### Faucet

- [Aztec Faucet](https://aztec-faucet.nethermind.io/) - Testnet faucet by Nethermind

### RPC - Mainnet

- [drpc](https://drpc.org/chainlist/aztec-mainnet-rpc) - Aztec mainnet RPC

### RPC - Testnet

- [drpc](https://drpc.org/chainlist/aztec-testnet-rpc) - Aztec testnet RPC

## Reference

- [Private Execution Environment (PXE) API Reference](https://docs.aztec.network/developers/reference/aztecjs/pxe/interfaces/pxe)
- [Current Limitations](https://docs.aztec.network/developers/reference/considerations/limitations)
