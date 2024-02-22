# Scroll Monorepo 
*The zkEVM zkRollup L2 for Ethereum scalability*

[![rollup](https://github.com/scroll-tech/scroll/actions/workflows/rollup.yml/badge.svg)](https://github.com/scroll-tech/scroll/actions/workflows/rollup.yml)
[![contracts](https://github.com/scroll-tech/scroll/actions/workflows/contracts.yml/badge.svg)](https://github.com/scroll-tech/scroll/actions/workflows/contracts.yml)
[![bridge-history](https://github.com/scroll-tech/scroll/actions/workflows/bridge_history_api.yml/badge.svg)](https://github.com/scroll-tech/scroll/actions/workflows/bridge_history_api.yml)
[![coordinator](https://github.com/scroll-tech/scroll/actions/workflows/coordinator.yml/badge.svg)](https://github.com/scroll-tech/scroll/actions/workflows/coordinator.yml)
[![prover](https://github.com/scroll-tech/scroll/actions/workflows/prover.yml/badge.svg)](https://github.com/scroll-tech/scroll/actions/workflows/prover.yml)
[![integration](https://github.com/scroll-tech/scroll/actions/workflows/integration.yml/badge.svg)](https://github.com/scroll-tech/scroll/actions/workflows/integration.yml)
[![codecov](https://codecov.io/gh/scroll-tech/scroll/branch/develop/graph/badge.svg?token=VJVHNQWGGW)](https://codecov.io/gh/scroll-tech/scroll)

<a href="https://scroll.io">Scroll</a> is a zkRollup Layer 2 scaling solution for Ethereum, offering significant performance and cost improvements while maintaining full compatibility with existing Ethereum developer tools.  Scroll is ideal for developers building decentralized applications that need high throughput, low fees, and seamless Ethereum compatibility.

**For developers building on Scroll.**

## Prerequisites
* Go 1.20 
* Rust (for version, see [rust-toolchain](./common/libzkp/impl/rust-toolchain))
* Hardhat / Foundry
* Docker

## Installation & Getting Started
1. `git clone https://github.com/scroll-tech/scroll`
2. `cd scroll && make install_dependencies` 
3. `make start_local_testnet`

## Directory Structure
* **bridge-history-api:** Collects deposit/withdraw events, generates withdrawal proofs
* **common:** Shared libraries and types
* **coordinator:** Dispatches proving tasks
* **database:** Database client and schema
* **l2geth:**  Scroll execution node
* **prover:**  Runs proof generation
* **rollup:** Rollup-related services
* **rpc-gateway:** RPC gateway (external repo)
* **tests:** Integration tests

## Technologies
* Rust
* Solidity
* Hardhat / Foundry

## Contributing
Please see the [Code of Conduct](CODE_OF_CONDUCT.md) and [Contribution Guideline](CONTRIBUTING.md) before submitting issues or PRs.

## License
Scroll Monorepo is licensed under the [MIT](./LICENSE) license.
