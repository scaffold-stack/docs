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
- Keep sentences concise. One idea per sentence.
- Do not repeat the page title as an H1. Mintlify renders the frontmatter `title` as the page heading.
- Start each page with a short intro paragraph, then optional `## Contents` on longer pages (see [Starknet Foundry docs](https://foundry-rs.github.io/starknet-foundry/getting-started/installation.html))
- Use requirement tables where tools or paths have version constraints
- Use `<Note>` and `<Warning>` callouts for important caveats
- Use Stacks brand orange (#FC6432) to match [docs.stacks.co](https://docs.stacks.co)
- Use Inter for headings and body (same as Stacks docs)
- Keep body text at ~16px with 1.625 line-height; avoid oversized marketing headings
- Inline code and fenced blocks: 15px (`0.9375rem`) minimum, never smaller than body text
- Model layout on Stacks docs: intro paragraph, optional card grid ("Looking for guides on..."), requirement tables
- Support link points to Telegram: https://telegram.me/+CBp6wSIiXNhmMjZk
- Do not use em dashes. Use periods, commas, colons, or separate sentences instead.
- Use sentence case for headings
- Bold for UI elements: Click **Connect Wallet**
- Code formatting for commands, file names, and code references
- Include practical code examples
- Focus on developer experience

## Content boundaries

- Put walkthroughs, layout examples, and tutorials in **Guides** (sidebar groups)
- Keep **CLI reference** (`cli/commands`) to syntax, flags, and short links into Guides
- Document Clarinet **3.21+**, `doctor`, `dev --auto-deploy`, ABI cache, `generate --watch`
- Include sample contracts and testing patterns
- Cover deployment workflows (testnet / mainnet / local-devnet)
- Don't document internal crate implementation details
- Don't include marketing copy (keep technical focus)
- Prefer documenting features shipped through **v0.1.9** in guide copy; call out newer CLI behavior only when the installed version docs intentionally cover it
