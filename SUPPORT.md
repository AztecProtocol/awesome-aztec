# Supporting Guide to Aztec Protocol GitHub Organization

Welcome to this supporting guide for the [AztecProtocol GitHub organization](https://github.com/orgs/AztecProtocol/repositories?type=all). Aztec Protocol is a privacy-centric Layer 2 scaling solution for Ethereum, leveraging zero-knowledge proofs (zk-SNARKs) and the domain-specific language Noir to enable confidential smart contracts and transactions. This allows developers to build private DeFi, payments, and apps without revealing sensitive data on-chain.

This guide provides a progressive, educational sequence—from zk privacy basics to deploying private contracts—accessible for non-technical users (focus on concepts like "shielded transactions") and developers (dive into Noir code and TS integrations).

This guide sequences content for knowledge assimilation: start with "why Aztec," move to "core tools," then "building apps," and end with "community engagement." Each section includes:

- **Overview**: What it covers and its importance.
- **Key Repos/Files**: Clickable GitHub links to repos, MD files, or code.
- **Learning Path**: Step-by-step order with cognitive tips (e.g., link concepts via examples).
- **Transitions**: How it leads to the next section.

By the end, you'll understand Aztec's zk-rollup architecture, engage with Noir for zk-circuits, and build/deploy confidential contracts. For updates, check repo commits or [docs.aztec.network](https://docs.aztec.network/).

## 1. High-Level Overview (zk Privacy Fundamentals and Aztec Ecosystem)
Build intuition for Aztec's hybrid zk-rollup: Public execution for scalability, private proofs for confidentiality. Ideal for beginners/non-devs; devs, note how it integrates with Ethereum L1.

### Key Concepts Covered
- zk-SNARKs for private txs: Prove computations without revealing inputs.
- Noir: DSL for zk-programs, compiling to ACIR circuits.
- Use cases: Private voting, shielded DeFi (e.g., confidential transfers).

### Key Repos/Files
- [`awesome-aztec/README.md`](https://github.com/AztecProtocol/awesome-aztec/blob/main/README.md): Curated hub with patterns (e.g., public-private state bridging).
- [`protocol-specs-pdf/README.md`](https://github.com/AztecProtocol/protocol-specs-pdf/blob/main/README.md): Links to PDF specs (e.g., protocol overview).
- [`aztec-packages/README.md`](https://github.com/AztecProtocol/aztec-packages): Monorepo intro to zk/FHE stack.

### Learning Path
1. Scan [`awesome-aztec/README.md`](https://github.com/AztecProtocol/awesome-aztec/blob/main/README.md) for patterns like token standards—non-devs focus on "ERC-20 with privacy."
2. Read [`aztec-packages/README.md`](https://github.com/AztecProtocol/aztec-packages) for ecosystem map (e.g., Barretenberg for proving).
3. View external: [Aztec Litepaper](https://docs.aztec.network/protocol/overview) (linked from repos) for diagrams.

**Tips**: Visualize zk as "math magic" hiding data. Connect to Ethereum: How does it fix public tx leaks? Use for motivation.

**Transition**: With basics, dive into core libraries for the "zk engine."

## 2. Core Libraries (zk Prover and Language Tools)
Foundational repos for zk-proofs and circuit writing. Devs start here for compilation; non-devs skim READMEs for "prover speed."

### 2.1 Barretenberg (zk Prover Backend)
Overview: Optimized PLONK SNARK prover for bn128 curve—powers Aztec's succinct proofs (UltraHonk for Noir, MegaHonk for apps).

#### Key Files
- [`barretenberg/README.md`](https://github.com/AztecProtocol/barretenberg/blob/main/README.md): Setup, benchmarks (e.g., sha256 proof in 388ms on 64 threads).
- [`barretenberg/cpp/src/barretenberg/bb/main.cpp`](https://github.com/AztecProtocol/barretenberg/blob/main/cpp/src/barretenberg/bb/main.cpp): BB commands for prove/verify.
- Mirro Active dev in [`aztec-packages/barretenberg`](https://github.com/AztecProtocol/aztec-packages/barretenberg).

#### Learning Path
1. Read README for install (`./cpp/bootstrap.sh` on Ubuntu/Mac).
2. Run benchmarks: `cmake --build --preset default --target ecc_bench`.
3. Test proving: `bb prove` on sample circuit—devs note OpenMP for multithreading.
4. Link to packages: Follow mirror for integration.

**Tips**: Non-devs: Prover = "zk calculator." Devs: Experiment with Keccak vs. Poseidon hashes.

### 2.2 Aztec-nr (Noir Framework for Contracts)
Overview: Extends Noir DSL for Aztec—write zk-provable contracts with private state (notes) and public views.

#### Key Files
- [`aztec-nr/README.md`](https://github.com/AztecProtocol/aztec-nr): Framework guide, state management (e.g., `@private` annotations).
- Mirror: [`aztec-packages/noir-projects/aztec-nr`](https://github.com/AztecProtocol/aztec-packages/noir-projects/aztec-nr)—stdlib like `uint-note.nr`.
- [`aztec-nr/src/main.nr`](https://github.com/AztecProtocol/aztec-nr/src/main.nr): Basic contract template.

#### Learning Path
1. Overview in README: Compare to vanilla Noir (ACIR for private funcs).
2. Setup: `aztec-nargo compile` (from docs link).
3. Write: Add `@compute` for zk-circuits—test with `first.nr`.
4. Stdlib: Explore notes (e.g., `value-note` for private balances).

**Tips**: Think Noir as "zk Rust." Devs: Compile to AVM bytecode for public funcs.

**Transition**: Tools ready? Use starters to build your first private app.

## 3. Applications (Building and Testing zk Contracts)
Apply libs to contracts and tests. Sequence: Starters first (simple), then examples (advanced).

### 3.1 Aztec Starter (Hello World Contract)
Overview: Minimal template for Noir contract + TS tests—ideal for onboarding.

#### Key Files
- [`aztec-starter/README.md`](https://github.com/AztecProtocol/aztec-starter): Getting started (Node 22+, `aztec start --sandbox`).
- [`aztec-starter/src/main.nr`](https://github.com/AztecProtocol/aztec-starter/src/main.nr): Easy Private Voting contract.
- [`aztec-starter/src/test/e2e/index.test.ts`](https://github.com/AztecProtocol/aztec-starter/blob/main/src/test/e2e/index.test.ts): Integration tests (spawn sandbox).
- [`aztec-starter/src/test/first.nr`](https://github.com/AztecProtocol/aztec-starter/blob/main/src/test/first.nr): TXE tests.
- Scripts: [`aztec-starter/scripts/deploy_contract.ts`](https://github.com/AztecProtocol/aztec-starter/blob/main/scripts/deploy_contract.ts) for deployment.

#### Learning Path
1. Install: `bash -i <(curl -s https://install.aztec.network)` then `yarn install`.
2. Compile: `yarn compile` → `yarn codegen` for artifacts.
3. Test: Run TS tests (`yarn test:e2e`)—deletes `./store` for clean PXE.
4. Deploy: `./scripts/deploy_contract.ts` on local net.
5. Branch: Switch to `testnet` for public testing.

**Tips**: Non-devs: Follow commands visually. Devs: Note PXE for private env—practice voting example.

### 3.2 Noir Starter and Examples
Overview: Templates and projects for zk apps (e.g., private DeFi).

#### Key Files
- [`noir-starter/README.md`](https://github.com/AztecProtocol/noir-starter/blob/main/README.md): Public template for Noir projects.
- [`aztec-examples/README.md`](https://github.com/AztecProtocol/aztec-examples): Sample Aztec projects (Noir contracts).
- From awesome: [`defi-wonderland/aztec-standards`](https://github.com/defi-wonderland/aztec-standards) (external, but linked)—token standard.

#### Learning Path
1. Clone noir-starter: Build basic circuit.
2. Explore examples: Run voting or token in sandbox.
3. Patterns: From awesome, stage public calls from private (e.g., update state via auth).

**Tips**: Incremental: Add privacy to ERC-20. Devs: Use TXE for Noir tests.

**Transition**: Apps built? Engage community for real-world projects.

## 4. Community and Advanced Resources (Engagement & Specs)
Deepen with workshops, audits, and designs.

### Key Repos/Files
- [`dev-rel/README.md`](https://github.com/AztecProtocol/dev-rel/blob/main/README.md): Workshops/tutorials (e.g., private voting codealong).
- [`audit-reports/README.md`](https://github.com/AztecProtocol/audit-reports/blob/main/README.md): Security audits.
- [`engineering-designs/README.md`](https://github.com/AztecProtocol/engineering-designs/blob/main/README.md): Internal designs (Jupyter for zk math).
- From awesome: [Common Patterns](https://docs.aztec.network/developers/guides/smart_contracts/writing_contracts/common_patterns)—public storage from private.

### Learning Path
1. Tutorials in dev-rel: Follow [private voting](https://docs.aztec.network/developers/tutorials/codealong/contract_tutorials/private_voting_contract).
2. Specs: Read AZIPs for upgrades.
3. Community: Join [Discord](https://discord.gg/aztec) for support.

**Tips**: Non-devs: Watch talks. Devs: Contribute audits or designs.

## Additional Repo Navigation Tips
- **Root Across Repos**: Check `README.md` for quickstarts; search org for "Noir" to find buried .nr files.
- **Building Locally**: Use `aztec-up` from starters; monorepo bootstrap in aztec-packages.
- **Search Tip**: GitHub org search for "tutorial" across files (e.g., in dev-rel).
- **External Complements**: Repos link to [docs.aztec.network](https://docs.aztec.network/) for built guides (e.g., Noir stdlib).

This guide sequences progressively: concepts → tools → apps → community. Revisit for a private dApp. For updates, check [roadmap](https://aztec.network/roadmap). Happy zk-building!
