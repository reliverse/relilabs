# 🌌 RSE: The Reliverse Standard Environment

[💖 GitHub Sponsors](https://github.com/sponsors/blefnk) • [💬 Discord](https://discord.gg/Pb8uKbwpsJ) • [✨ Repo](https://github.com/reliverse/rse) • [📦 NPM](https://npmjs.com/@reliverse/rse) • [📚 Docs](https://blefnk.reliverse.org/blog/my-products/reliverse-cli)

---

## What is RSE?

**RSE** (`@reliverse/rse`) is your all-in-one, AI-powered companion for building, improving, and managing web projects. Whether you're starting from scratch or upgrading an existing app, RSE brings together project bootstrapping, refactoring, automation, bundling, and more—right in your terminal.

- **Unified CLI**: One tool for project creation, refactoring, deployment, and AI-powered enhancements.
- **Modern Bundler**: Includes Relidler, a fast, Rust-powered alternative to the JS ecosystem (npm, bun, yarn, etc.).
- **AI Superpowers**: Chat, refactor, lint, and generate images/code with built-in AI tools.

---

## Quick Links

- [GitHub Sponsors](https://github.com/sponsors/blefnk)
- [Discord](https://discord.gg/Pb8uKbwpsJ)
- [NPM: @reliverse/rse](https://npmjs.com/@reliverse/rse)
- [Docs](https://blefnk.reliverse.org/blog/my-products/reliverse-cli)
- [Reliverse Registry](https://rse.reliverse.org)

---

## Key Features

- 🦾 **Superapp for Devs**: One CLI, tons of features—spin up, refactor, deploy, and automate.
- 🚀 **Fast Project Bootstrapping**: Start fresh or use templates in seconds.
- 🔧 **Safe Refactoring**: Drop in popular libs, automate setup, and keep your codebase happy.
- ⚙️ **Automation**: ESLint, env files, and more—let RSE handle the boring stuff.
- 🏗️ **Framework Friendly**: Works great with Next.js and other frameworks.
- 🌐 **Integrated Deployment**: Push to GitHub, deploy to Vercel, all in one go.
- 🤖 **AI Tools**: Chat, refactor, lint, and generate images/code with Reliverse AI.
- 🏯 **Monorepo & Bundler**: Relidler for monorepos, standalone repos, and modern JS/TS bundling.
- 🔌 **Plugin System**: Extend RSE with custom plugins and tools.

---

## Getting Started

### Prerequisites

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/)
- One of: [bun](https://bun.sh), [pnpm](https://pnpm.io), [yarn](https://yarnpkg.com), or [npm](https://npmjs.com)

### Installation

**Install globally:**

```sh
bun i -g @reliverse/rse
```

**Or update:**

```sh
rse update
```

### First Run

```sh
rse cli
```

- On first run, `.reliverse/reliverse.config.{ts,jsonc}` is generated.
- Customize this config to fit your project. Changes apply on next launch (hot-reload coming soon).

---

## Core Usage

### Main Commands

- `rse cli` — Launches the interactive wizard for project creation or enhancement.
- `rse logout` — Logs you out and clears credentials.
- `rse studio` — Opens the Reliverse Studio (visual brain center).
- `rse --help` — Shows all available commands and usage tips.

**Tip:** All commands and flags are optional. RSE guides you even if you skip arguments.

### Direct Commands

- Prefer quick access or CI/CD? Use specific commands directly.
- Run `rse <command> --help` for options and flags.

---

## AI & Automation

- `rse ai <prompt>` — Chat with Reliverse AI for help, code, or questions.
- `rse ai code <prompt> <paths>` — AI-powered code generation or refactoring.
- `rse ai gen <prompt>` — Generate images from descriptions, saved to your upload provider.
- `rse ai lint <prompt> <paths>` — Smart AI linting, issue detection, and fixes.

[See AI docs](./src/cli/docs/docs-ai.md)

---

## Project Bootstrapping & Add-ons

- `rse init` — Start a new minimal Reliverse project (library or app).
- `rse add` — Same as `rse init` (interactive wizard, context-aware).
- `rse add <something>` — Instantly add APIs, auth, DB, payments, i18n, AI tools, file uploaders, forms, and more.
- `rse add -g <something>` — Install global CLIs, essential tools, or desktop apps from your terminal.
- `rse add rule <something>` — Browse and install AI IDE rules for RSE, Cursor, Windsurf, Copilot, and more.

[See Add docs](./src/cli/docs/docs-add.md)

---

## Advanced: Bundler & Workspace System

### Relidler: The All-in-One Bundler

**@reliverse/relidler** is a flexible, unified, and fully automated bundler for TypeScript and JavaScript projects, as well as an NPM and JSR publishing tool.

- 🦄 Monorepo and standalone repo support
- 🥇 Single or per-package `package.json`
- 🗑️ Cleans unused files
- ⚡ Fast, Rust-powered, drop-in replacement for `unbuild`
- 📦 Automated NPM/JSR publishing
- 🔄 Automatic version bumps
- 🔧 TypeScript alias conversion
- 🔌 Plugin system (7+ built-in plugins)

### Setup

**Install:**

```sh
bun add -D @reliverse/relidler
# OR globally:
# bun i -g @reliverse/relidler
```

**Update:**

```sh
bun update --latest
# OR globally:
# bun update -g --latest
```

**Configure:**

```sh
echo "*.log" >> .gitignore
echo "dist-npm" >> .gitignore
echo "dist-jsr" >> .gitignore
echo "dist-libs" >> .gitignore

bun add -D @reliverse/relidler-cfg
relidler cli
```

- `.config/rse.ts` is created on first run. [Example config](https://github.com/reliverse/relidler-js-bundler/blob/main/.config/rse.ts)

**Run:**

```sh
relidler cli
```

**Add to package.json:**

```json
"scripts": {
  "pub": "relidler cli"
}
```

### Plugins & Tools

- `relidler tools --tool <tool> --input <dir> --out <file> [options]`
- Tools: agger, librer, merger, splitter, adder, initter, certer

[See plugin docs](src/cli/args/tools/README.md)

---

## API & SDK

- Build custom RSE/Reliverse CLI plugins or extend your own tools.
- Interact with [reliverse.org](https://reliverse.org) or power up your own CLIs.

```sh
bun add @reliverse/rse-sdk
# For Relidler SDK:
bun add @reliverse/relidler-sdk
```

---

## Contributing

**Classic way:**

```sh
git clone https://github.com/reliverse/rse.git
cd cli
code .
```

**RSE way:**

```sh
rse cli
> Clone an existing repository
> Developer related
> reliverse
> cli
> Y/n # opens default editor
```

**Development:**

```sh
bun install
bun dev
# bun dev:command = rse <command> --dev
bun check
```

**Committing:**

```sh
git add .
git commit -m "your commit message"
git push
# OR via RSE:
rse cli
> Commit
<your commit message>
<press enter to push>
```

**Open a PR:** [GitHub Pull Requests](https://github.com/reliverse/rse/pulls)

---

## Support

- [GitHub Sponsors](https://github.com/sponsors/blefnk)
- Star [the repo](https://github.com/reliverse/rse) to show your love!

---

## License

[MIT](./LICENSE) © 2025 [blefnk (Nazar Kornienko)](https://github.com/blefnk)

---

## Shoutouts

- Inspired by [t3-oss/create-t3-app](https://github.com/t3-oss/create-t3-app#readme)
- Special thanks to [unjs/unbuild](https://github.com/unjs/unbuild#readme)

---

> Everything you see in Reliverse so far is **built by one person** ([@blefnk Nazar Kornienko](https://github.com/blefnk)) — with love, caffeine, and way too many terminal tabs.  
> Got feedback, ideas, or just want to hang out? [Join the Discord](https://discord.gg/Pb8uKbwpsJ) — everyone's welcome!

---

**You're amazing. Thanks for being part of this!**
