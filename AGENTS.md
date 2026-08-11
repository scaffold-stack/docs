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
- **readability:** muted body text, dark headings, generous section spacing — one command block per step, not walls of code
- Prefer `<Steps>` + `<Step>` for sequential guides (quickstart, install flows); use `<Tip>` and `<Note>` for short asides instead of long paragraphs
- Drop redundant `## Contents` sections — the right sidebar TOC is enough
- Do not repeat the page title as an H1. Mintlify renders the frontmatter `title` as the page heading.
- Start each page with a short intro paragraph (1–2 sentences), then optional steps or sections
- Use requirement tables where tools or paths have version constraints
- Use `<Note>` and `<Warning>` callouts for important caveats
- Use Stacks brand orange (#FC6432) to match [docs.stacks.co](https://docs.stacks.co)
- Use Inter for headings and body (same as Stacks docs)
- Keep body text at ~14px with **1.75 line-height**; body color muted (`#52525b` light / `#a1a1aa` dark), headings darker
- Inline code: soft pills, **font-weight 400**, no heavy borders
- Fenced code blocks: inset panel (`#f6f6f7` light / `#111113` dark), one block per command step, generous padding
- Section spacing: ~2.75rem above `h2`, airy list items
- Model layout on Stacks docs: intro paragraph, optional card grid ("Looking for guides on..."), requirement tables
- Support link points to Telegram: https://telegram.me/+CBp6wSIiXNhmMjZk
- Do not use em dashes. Use periods, commas, colons, or separate sentences instead.
- Use sentence case for headings
- Bold for UI elements: Click **Connect Wallet**
- Code formatting for commands, file names, and code references
- Include practical code examples
- Focus on developer experience

## SEO

Every navigable page should help users find Scaffold Stacks via search (Google, Bing, AI indexes).

- **Site config:** `docs.json` sets global `description`, `seo.metatags`, `seo.organization`, and canonical base URL (`https://scaffoldstacks.mintlify.app`)
- **Page frontmatter:** always include `title`, `description` (120–160 chars, keyword-rich but natural), and `keywords` as a YAML array
- **Target terms:** Scaffold Stacks, stacksdapp, stacksdapp CLI, Stacks dApp, Clarity, Clarinet, Bitcoin L2, SIP-010, SIP-009, testnet, mainnet
- **Titles:** use searchable phrases where it fits (e.g. "stacksdapp CLI reference", not just "CLI commands")
- **Intro paragraphs:** mention stacksdapp and Stacks naturally in the first 1–2 sentences — crawlers weight early content
- **Headings:** use terms people search for (`Deploy to Stacks testnet`, `Clarity smart contracts`) without keyword stuffing
- **Links:** use descriptive anchor text ("stacksdapp CLI reference" not "click here")
- **Do not** add `noindex` to production guides; boilerplate pages outside `docs.json` navigation are not indexed by default

## Content boundaries

- Put walkthroughs, layout examples, and tutorials in **Guides** (sidebar groups)
- Keep **CLI reference** (`cli/commands`) to syntax, flags, and short links into Guides
- Document Clarinet **3.23+**, Clarity 6 default, `doctor --strict`, git hooks, agent skill, `dev --auto-deploy`, ABI cache, `generate --watch`, `--clarity-version`, `--yes` deploy
- Include guides: quickstart, workflows, adopt-existing, upgrade, project-layout, frontend, sip-standards, clarity-language, troubleshooting
- Include sample contracts and testing patterns
- Cover deployment workflows (testnet / mainnet / local-devnet)
- Don't document internal crate implementation details
- Don't include marketing copy (keep technical focus)
- Prefer documenting features shipped through the latest scaffold; call out Clarity 6, epoch 4.0, and bundled agent skill in guide copy
