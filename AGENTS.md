> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Scaffold Stacks Documentation

## About this project

- Documentation for Scaffold Stacks, a Rust-powered CLI and Next.js template for building full-stack Stacks (Bitcoin L2) dApps
- Built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Terminology

- Use "dApp" not "app" or "application"
- Use "contract" for Clarity smart contracts
- Use "Stacks" for the blockchain platform
- Use "sBTC" for Stacks' Bitcoin-backed token
- Use "testnet" for Stacks test network
- Use "mainnet" for Stacks production network
- Use "devnet" for local development network

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Connect Wallet**
- Code formatting for commands, file names, and code references
- Use orange accent color (#FF6B35) in examples
- Include practical code examples
- Focus on developer experience

## Content boundaries

- Document CLI commands and their usage
- Include sample contracts and explanations
- Cover deployment workflows
- Explain auto-code generation
- Include testing best practices
- Don't document internal implementation details
- Don't include marketing copy (keep technical focus)
