# 🌌 **rse**: @reliverse/rse | (prev. reliverse cli: @reliverse/rse) | [reliverse.org](https://reliverse.org)

[💖 GitHub Sponsors](https://github.com/sponsors/blefnk) • [💬 Discord](https://discord.gg/Pb8uKbwpsJ) • [✨ Repo](https://github.com/reliverse/rse) • [📦 NPM](https://npmjs.com/@reliverse/rse) • [📚 Docs](https://blefnk.reliverse.org/blog/my-products/reliverse-cli)

**@reliverse/rse** is your all-in-one companion for building and improving web projects — whether you're kicking off something new or upgrading an existing app. It's like having a little AI-powered toolbox in your terminal, ready to help with coding, refactoring, image gen, and more.

## What it can do

- 🦾 It's a superapp for devs. One CLI. Tons of stuff. Spin up, refactor, deploy, AI — it's all in there.
- 🚀 Start fresh or load up an existing template in seconds.
- 🔧 Refactor safely, drop in popular libs, and keep your codebase happy.
- ⚙️ Automate boring setup stuff like ESLint, env files, etc — let the CLI handle it.
- 🏗️ Works great with Next.js and plays nice with other frameworks too.
- 🌐 Push to GitHub, deploy to Vercel — all in one go.
- ⏬ Reliverse auto-clones repos/templates and configures them smartly.
- 🔌 Use the `🔬 Create/edit project manually` (or `reliverse init`) to integrate things into your codebase.
- 🤖 Chat with Reliverse AI or let agentic tools like Relinter suggest improvements to your code.

## Getting Started

Ensure Git, Node.js, and bun•pnpm•yarn•npm are installed. Then:

### Installation

1. **Install globally**:

   ```sh
   bun i -g @reliverse/rse
   ```

   **Or update as needed**:

   ```sh
   rse update
   ```

2. **Run and enjoy**:

   ```sh
   rse cli
   ```

  `.reliverse/reliverse.config.{ts,jsonc}` is generated on first run.
  Customize it to fit your project and tweak CLI behavior.
  Changes apply next launch (hot-reload coming soon).

## Show some love 🫶

If `@reliverse/rse` saved you time or made you smile:

- Support on [GitHub Sponsors](https://github.com/sponsors/blefnk)
- Or just drop a ⭐️ on [GitHub](https://github.com/reliverse/rse)

It helps more than you think! Thanks for being here!

## Commands

From bootstrapping projects to unleashing AI superpowers. Below is a quick overview of what the Reliverse CLI can do.

### Notes

- All commands and flags are optional. Reliverse tries its best to guide you, even if you skip arguments.
- `rse cli` is your all-in-one entry point — it includes everything available in the individual commands.
- Prefer quick access or running in non-interactive environments like CI/CD? Use the specific commands directly.  
- Run `reliverse <command> --help` to explore available options and flags.

### Core Commands

- `rse cli` — Here you can launch an interactive wizard to create or boost your project.
- `rse logout` — Logs you out and clears credentials. For when it's time to start fresh.
- `rse studio` — Opens the Reliverse Studio — the visual brain center of your local Reliverse memory.
- `rse --help` — Shows all available commands and handy usage tips. Because we all forget sometimes.

### AI Commands ([docs](./src/cli/docs/docs-ai.md))

- `rse ai <prompt>` — Your terminal-sidekick. Ask questions, get help, or just have a quick chat with Reliverse AI.  
- `rse ai code <prompt> <paths>` — Need a refactor or something new? Let AI generate or improve code across the given paths.  
- `rse ai gen <prompt>` — Describe an image and the AI will create it for you, saving it directly to your selected upload provider.  
- `rse ai lint <prompt> <paths>` — Run smart linting on your code using AI. It catches issues, suggests fixes, and helps clean things up fast.

### Init/Add Commands ([docs](./src/cli/docs/docs-add.md))

- `rse init` — Kickstart a new minimal Reliverse project. Building a library or an app? Just pick your direction and you're good to go — clean start, full power.
- `rse add` _(without args)_ — Same as `reliverse init`. Both open an interactive wizard — with different prompts depending on whether the folder is empty or not.
- `rse add <something>` — Drop in the essentials or the extras — from API, auth, DB, payments, and i18n — to AI tools, file uploaders, and form libraries — all integrated into your codebase in seconds. Feels like magic. Actually is.
- `rse add -g <something>` — Use `-g` to install global CLIs (e.g. `eslint`, `@reliverse/relidler`), essential tools (e.g. `bun`, `stripe`), or even desktop apps (e.g. `code`, `obsidian`) — all from your terminal.
- `rse add rule <something>` — Browse and install AI IDE rules for Reliverse, Cursor, Windsurf, Copilot, and more — from both official and community sources. Powered by smart caching and auto-conversion to `.mdc` when needed.

### Additional

- `rse clone` ([docs](./src/cli/docs/docs-clone.md)) — Clone a GitHub repo (just paste the link), or convert a webpage into LLM-ready content if you pass a non-GitHub URL.
- `rse cmod` ([docs](./src/cli/docs/docs-cmod.md)) — Applies codemods to your project — for quick, safe refactoring powered by AI or presets.
- `rse env` ([docs](./src/cli/docs/docs-env.md)) — Instantly generates a .env file based on your .env.example with an interactive wizard. Saves time, avoids typos.
- `rse multireli` ([docs](./src/cli/docs/docs-multireli.md)) — Generates multiple reliverse config files so you can batch-generate multiple projects with reliverse cli.
- `rse upload` ([docs](./src/cli/docs/docs-upload.md)) — Uploads a media files like images to your selected provider like UploadThing and Uploadcare.
- `rse sync` _(coming soon)_ — Syncs your local @reliverse/rse memory with your own Reliverse AI which lies on [reliverse.org](https://reliverse.org).

## API (for advanced users)

- The SDK lets you build custom Reliverse CLI plugins, interact with [reliverse.org](https://reliverse.org), or even power up your own CLIs.
- No need to reinvent the wheel — [@blefnk](https://github.com/blefnk) already took care of the hard parts, so you can use it however you like.
- If it saves you time, please [consider making a small donation](https://github.com/sponsors/blefnk) 🩷 to support ongoing development.

```sh
bun add @reliverse/rse-sdk
```

## But... rse is also a

# @reliverse/relidler | Relidler | Reliverse Bundler

[💖 GitHub Sponsors](https://github.com/sponsors/blefnk) • [💬 Discord](https://discord.gg/Pb8uKbwpsJ) • [✨ Repo](https://github.com/reliverse/relidler-js-bundler) • [📦 NPM](https://npmjs.com/@reliverse/relidler)

🌠 @reliverse/rse is all-in-one alternative to a whole JS ecosystem. It's workspace system for both monorepos and standalone repos. It's also a new programming language and modern alternative to npmjs, JS package managers (npm, bun, deno, yarn, pnpm), and build system. Fast, secure, and all-in-one — from private registries with granular tokens to bundling, testing, hot reload, and Node/Bun-compatible runtime. WIP.

🏯 Reliverse is a website builder inside your terminal. You can start from scratch or use a template. You can set everything up automatically or configure everything exactly the way you like. You can have it all, with all the tools already prepared for you.

**@reliverse/relidler** is a flexible, unified, and fully automated bundler for TypeScript and JavaScript projects, as well as an NPM and JSR publishing tool.

🌠 `@reliverse/rse` is a radical rethinking of the modern JavaScript ecosystem. Drop-in JS replacement. Public and private registries. Universal package manager. All built on Rust. All-in-one.

🌌 rse is a flexible, unified, and fully automated bundler for typescript & javascript projects, as well as an npm & jsr publishing tool

## Features

- 🦄 Both monorepo and standalone repo support
- 🥇 Single `package.json` for all packages
- 🧬 Per-package `package.json` also supported
- 🗑️ Builder cleans different unused stuff
- 😘 Drop-in replacement for `unbuild`
- ⚡ `relidler` works via CLI and SDK
- 📦 Automated NPM/JSR publishing
- ✅ Ensures reliable JS/TS builds
- 🔄 Handles automatic version bumps
- 🔧 Eliminates `package.json` headaches
- 🎯 Optimized for speed and modern workflows
- 🛠️ Converts TypeScript aliases to relative paths
- ✨ Packed with powerful features under the hood
- 📝 Highly configurable flow via a configuration file
- 🔌 Plugin system with two built-in plugins included

## Resources

- [reliverse.org](https://rse.reliverse.org) — rse's registry

> **🌠 `@reliverse/rse` is a radical rethinking of the modern JavaScript ecosystem.**  
> Drop-in JS replacement. Public and private registries. Universal package manager. All built on Rust. All-in-one.

RSE isn't just a tool — it's the **Reliverse Standard Environment**.

It aims to unify everything you rely on:  

- A **typed, safe, predictable JavaScript alternative**  
- A **secure registry ecosystem** (public & private, with token scopes)  
- A **modern package manager** that replaces `npm`, `yarn`, `pnpm`, `bun`, `deno`  
- A **build/test/run/dev toolchain** with bundling, HMR, and Bun/Node compatibility  

- Built in Rust for **speed, safety, and confidence**.  
- Still a WIP — but we're building something that will outlive the chaos.

## Terminology

- `rse` → **ReliverSE**, the unified standard
- `reli` → **RELIverse**, the toolchain powering it

## Navigation

Each part of the system has its own README:

- [`Reliverse's JS Alternative`](README-js-alt.md) — a drop-in `.js` replacement with Rust-like stability
- [`Reliverse's NPM Alternative`](README-npm-alt.md) — modern package registry and publishing flow
- [`Reliverse's GIT Alternative`](README-git-alt.md) — a decentralized, developer-first approach to versioning

## Getting Started

- Make sure you have Git, Node.js, and a package manager (bun, pnpm, yarn, or npm) installed.
- It's also a good idea to make sure you're using the latest npm version: `npm i -g npm@latest`.

### 1: **Installation**

```bash
bun add -D @reliverse/relidler

# OR: install globally
# bun i -g @reliverse/relidler
```

Or update as needed:

```bash
bun update --latest

# OR: if you installed globally
# bun update -g --latest
```

### 2: **Prepare your project**

a. **Configure `.gitignore`**:

```sh
echo "*.log" >> .gitignore
echo "dist-npm" >> .gitignore
echo "dist-jsr" >> .gitignore
echo "dist-libs" >> .gitignore
```

b. **Install config intellisense**:

```sh
bun add -D @reliverse/relidler-cfg
```

c. **Initialize config**:

```sh
relidler cli
```

- The `.config/rse.ts` file is automatically created on first run.
- **It's recommended to customize this file according to your needs.**
- You can check an example config here: [.config/rse.ts](https://github.com/reliverse/relidler-js-bundler/blob/main/.config/rse.ts)

#### 3: **Run and enjoy**

```bash
relidler cli
```

Optionally you can add this to your package.json scripts: `"pub": "relidler cli"`

### Playground

> **💡 Tip**:
> Want to test Relidler before integrating it into your project?
> Clone the repo and build it using Relidler itself!

```sh
git clone https://github.com/reliverse/relidler.git
cd relidler
bun i
bun dev # bun src/main.ts --dev
```

## Cleaner

For example:

```json
"main": "apps/web/index.tsx",
"module": "apps/web/index.tsx",
```

Will not be added to the final bundle when bundling libraries.

## 🔌 Plugins (aka Tools)

**Relidler** ships with a powerful plugin system — offering flexible utilities for various use cases. It already comes with **7 plugins** out of the box.

Lets you run standalone Relidler features directly from the CLI:

```bash
relidler tools --tool <tool> --input <dir> --out <file> [options]
```

**Note for contributors**: All plugins (tools) are defined in the `src/cli/args/tools` directory.

**Available tools**:

- `agger`: Generates aggregator file with content like `export { getSomething } from "./utils.js"`. **Note**: Currently it replaces the file content, not appends.

### 1. `relidler-tool-librer`

> Build and publish multiple libraries from a single repo — without losing your mind.

- 📦 Turns specific subdirectories in your project into **independent, publishable packages**.
- 🧠 No workspace madness. You only need **one `package.json`** — but can manage multiple libraries.
- 🔗 Handles **dependency wiring**, **cross-library references**, **type resolution**, and more — automatically.
- 🛠 Perfect for monorepos, CLI toolchains, component libraries, or SDKs — where each subpackage is part of a bigger whole.

> It's like workspaces, but chill.

**Setup**:

1. Create `libs` directory in the root or in the `src` directory of your project.
2. Create a `package.json` with at least: name, version, author; everything else is optional and autogenerated.
3. Open `.config/rse.ts`, switch `libsActMode` to `main-and-libs` or `libs-only` (default is `main-only`).
4. Define `libsList` in the config `.config/rse.ts`.
5. Create correspoing folders in the `libs` directory.
6. Optionally you can also use `relidler tools --tool agger` to generate an aggregator file for your libraries.
7. Run `relidler cli` to build and publish your libraries.

**Usage example**:  
Using `@reliverse/relidler-cfg` to package [src/libs/cfg](https://github.com/reliverse/relidler-js-bundler/tree/main/src/libs/cfg):

```ts
// .config/rse.ts
libsActMode: "main-and-libs",
libsDirDist: "dist-libs",
libsDirSrc: "src/libs",
libsList: {
  "@reliverse/relidler-cfg": {
    libDeclarations: true,
    libDescription: "@reliverse/relidler defineConfig",
    libDirName: "cfg",
    libMainFile: "cfg/cfg-main.ts",
    libPkgKeepDeps: false,
    libTranspileMinify: true,
  },
},
```

**Relidler Task Commands**:

- `// relidler-replace-me` tells Relidler to grab the contents of `../../types.ts` and inject them directly in place of your command definition.

  ```ts
  export * from "../../types.js"; // relidler-replace-me
  // OR:
  export type { SpecificTypeName1, SpecificTypeName2 } from "../../types.js"; // relidler-replace-me
  ```

- More magic commands coming soon...

### 2. `relidler-tool-agger`

**Usage example**: If you're exploring the example [Playground](#playground), you can try the following:

1. Open [src/libs/sdk/sdk-main.ts](https://github.com/reliverse/relidler-js-bundler/blob/main/src/libs/sdk/sdk-main.ts) in your IDE.
2. Press `Ctrl+A`, then `Backspace`. Run the command below and watch the magic happen:

```bash
bun tools:agger # Shortcut for:
bun src/main.ts tools --dev --tool agger --input src/libs/sdk/sdk-impl --out src/libs/sdk/sdk-main.ts --recursive --named --strip src/libs/sdk
```

### 3. `relidler-tool-merger`

See [src/cli/args/tools/merger/README.md](src/cli/args/tools/merger/README.md) for details.

### 4. `relidler-tool-splitter`

See [src/cli/args/tools/splitter/README.md](src/cli/args/tools/splitter/README.md) for details.

### 5. `relidler-tool-adder`

See [src/cli/args/tools/adder/README.md](src/cli/args/tools/adder/README.md) for details.

### 6. `relidler-tool-initter`

See [src/cli/args/tools/initter/README.md](src/cli/args/tools/initter/README.md) for details.

### 7. `relidler-tool-certer`

See [src/cli/args/tools/certer/README.md](src/cli/args/tools/certer/README.md) for details.

## API (for advanced users)

The SDK lets you build custom Relidler CLI plugins or even extend your own CLI tools.

```sh
bun add @reliverse/relidler-sdk
```

**Usage example**: [@reliverse/rse](https://github.com/reliverse/rse-website-builder) leverages this SDK to extend its functionality.

## TODO

- [x] ~~Implement stable `regular` build and publish~~
- [ ] Implement stable `library` build and publish
- [ ] Achieve full drop-in replacement for `unbuild`
- [ ] Support auto migration from `build.config.ts`
- [ ] Allow plugins to extend Relidler's `defineConfig`
- [ ] Support configuration via `reliverse.{ts,jsonc}`
- [ ] Make config file optional with sensible defaults

## Related

Special thanks to the project that inspired `@reliverse/relidler`:

- [unjs/unbuild](https://github.com/unjs/unbuild#readme)

## Support

- If Relidler saves you time and effort, please consider supporting its development: [GitHub Sponsors](https://github.com/sponsors/blefnk);
- Even a simple star on [GitHub](https://github.com/reliverse/relidler) shows your love. Thank you!

## License

🩷 [MIT](./LICENSE) © 2025 [blefnk Nazar Kornienko](https://github.com/blefnk)

## Marketing Website

> Coming soon — with docs, demos, and design systems.

### Contributing

**Install dependencies:**

```bash
bun install
```

**Start the dev server:**

```bash
bun dev
```

> Built using [Bun](https://bun.sh), [Reliverse CLI](https://github.com/reliverse/rse), and raw determination.

## License

[MIT](LICENSE) © 2025 [@blefnk Nazar Kornienko](https://github.com/blefnk)

## Contribute, please 😽

- Everything you see in Reliverse so far is **built by one person** ([@blefnk Nazar Kornienko](https://github.com/blefnk)) — with love, caffeine, and way too many terminal tabs.
- Got feedback, ideas, bugs to squash, or just wanna vibe with the project? [Hop into my Discord](https://discord.gg/Pb8uKbwpsJ) — I'd love to chat.
- Whether you want to code, brainstorm, fix typos, or just hang out — you're always welcome here.  
  No pressure, no gatekeeping — just good energy and open-source fun.

### <🏗️1> Come together, right now

Two ways to clone this repo and contribute:

**Classic way**:

```bash
git clone https://github.com/reliverse/rse.git
cd cli
code . # opens vscode editor
```

**Reliverse way**:

```bash
reliverse cli
> Clone an existing repository
> Developer related  
> reliverse  
> cli
> Y/n # opens default editor
```

Boom. You're in.

### <🏗️2> You're a magician, do magic

1. Run `bun latest` to install dependencies and keep things fresh.
2. Use AI (Reliverse, Cursor, whatever floats your dev boat) or write code manually.
3. Note that `bun dev:command` works just like running `reliverse <command> --dev`.
4. It's a good idea to run `bun check` to make sure everything's clean and happy.
5. All done? Awesome! Now commit and push your changes by following your way:

**Classic way**:

```bash
git add .
git commit -m "your commit message"
git push
```

**Reliverse way**:

```bash
reliverse cli
> Commit
<your commit message>
<press enter to push>
```

### <🏗️3> What a great time to live

- All done? High five! 🖐️
- Head to [repo](https://github.com/reliverse/rse/pulls) & open a PR.
- That's it. You're amazing.

Thanks for being part of this!

## Shoutout

Reliverse CLI was inspired by this gem:

- [t3-oss/create-t3-app](https://github.com/t3-oss/create-t3-app#readme)

## License

💖 [MIT](./LICENSE) © 2025 [blefnk (Nazar Kornienko)](https://github.com/blefnk)
