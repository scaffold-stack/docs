# Scaffold Stacks Documentation

Documentation for Scaffold Stacks, a Rust-powered CLI and Next.js template for building full-stack Stacks (Bitcoin L2) dApps.

## About Scaffold Stacks

Scaffold Stacks provides everything you need to build decentralized applications on the Stacks blockchain. It combines a powerful CLI tool with a modern Next.js frontend template, making it easy to create, test, and deploy smart contracts.

### Key Features

- **Auto-generated TypeScript bindings**: Automatically generate type-safe TypeScript code from your Clarity contracts
- **Live debug UI**: Interactive interface to test contract functions during development
- **One-command deployment**: Deploy to testnet or mainnet with a single command
- **Local development**: Run a full Stacks devnet locally with Docker
- **Contract templates**: Start with pre-built SIP-010 tokens or SIP-009 NFTs

## Quick Start

Get started in 5 steps:

1. Install the CLI: `cargo install stacksdapp`
2. Scaffold a new project: `stacksdapp new my-app`
3. Deploy to testnet: `stacksdapp deploy --network testnet`
4. Start the frontend: `stacksdapp dev --network testnet`
5. Connect your wallet and interact with contracts

## License

This documentation is part of the Scaffold Stacks project.
