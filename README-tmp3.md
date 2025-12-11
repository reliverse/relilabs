# 🌌 **rse**: @reliverse/rse | (prev. reliverse cli: @reliverse/rse) | [reliverse.org](https://reliverse.org)

[💖 github sponsors](https://github.com/sponsors/blefnk) • [💬 discord](https://discord.gg/pb8ukbwpsj) • [✨ repo](https://github.com/reliverse/rse) • [📦 npm](https://npmjs.com/@reliverse/rse) • [📚 docs](https://blefnk.reliverse.org/blog/my-products/reliverse-cli)

## what is rse?

rse (**r**eliver**se** — reliverse standard environment) is an all-in-one development ecosystem that unifies the entire javascript development workflow:

- **project creation & management**: start new projects or enhance existing ones
- **ai-powered development tools**: code generation, refactoring, image creation, and more
- **modern build system**: bundle, publish, and manage javascript/typescript projects
- **universal package registry**: a complete replacement for npm, with public and private options
- **alternative js ecosystem**: a safer, more predictable programming environment

whether you're starting a new project or improving an existing one, rse provides the tools you need in a unified experience.

rse is something like bun but on steroids.

## terminology

- `rse` → **reliverse standard environment**, the unified platform
- `reli` → **reliverse**, the toolchain powering it
- `rse build` → the build and publishing system (previously known as relidler)

## core features

### project management

- 🚀 start fresh projects or load existing templates in seconds
- 🔧 safely refactor, integrate libraries, and improve your codebase
- ⚙️ automate setup tasks (eslint, env files, etc.)
- 🌐 push to github and deploy to vercel with a single command
- 🏗️ works with next.js and other popular frameworks

### ai-powered development

- 🤖 chat with rse ai for coding assistance
- 🦾 generate and refactor code with ai
- 🎨 create images from text descriptions
- 🧹 smart linting with ai-powered suggestions

### build system

- 📦 build and publish typescript/javascript projects
- 🦄 support for both monorepos and standalone projects
- 🔄 automated versioning and publishing to npm/jsr
- 🛠️ typescript path alias conversion
- 🔌 powerful plugin system for extending functionality

## getting started

ensure git, node.js, and a package manager (bun, pnpm, yarn, npm) are installed, then:

### installation

```sh
bun i -g @reliverse/rse
```

or update to the latest version:

```sh
rse update
```

### quick start

launch the interactive wizard:

```sh
rse cli
```

a config file (`.reliverse/reliverse.config.{ts,jsonc}`) is generated on first run. customize it to fit your project and tweak cli behavior.

## commands

### core commands

- `rse cli` — interactive wizard to create or boost your project
- `rse logout` — clear credentials
- `rse studio` — open the visual brain center of your local rse memory
- `rse --help` — show all available commands

### ai commands

- `rse ai <prompt>` — chat with rse ai from your terminal
- `rse ai code <prompt> <paths>` — generate or improve code
- `rse ai gen <prompt>` — create images from text descriptions
- `rse ai lint <prompt> <paths>` — smart linting with ai

### project commands

- `rse init` — start a new minimal rse project
- `rse add` — add components, libraries or tooling to your project
- `rse add -g <something>` — install global tools or desktop apps
- `rse add rule <something>` — add ai ide rules for various editors

### utility commands

- `rse clone` — clone a github repo or convert webpages to llm-ready content
- `rse cmod` — apply codemods for quick, safe refactoring
- `rse env` — generate .env files based on your .env.example
- `rse multireli` — generate multiple config files for batch project creation
- `rse upload` — upload media files to services like uploadthing and uploadcare

### build system commands

- `rse build cli` — build and publish packages
- `rse build tools --tool <tool>` — run standalone build tools:
  - `agger` — generate aggregator files for exports
  - `librer` — build and publish multiple libraries from a single repo
  - `merger` — merge files
  - `splitter` — split files
  - `adder` — add components/templates
  - `initter` — initialize projects
  - `certer` — certificate management

## build system configuration

for build system functionality:

1. create a config file:

```sh
rse build cli
```

2. configure `.gitignore`:

```sh
echo "*.log" >> .gitignore
echo "dist-npm" >> .gitignore
echo "dist-jsr" >> .gitignore
echo "dist-libs" >> .gitignore
```

3. install config intellisense:

```sh
bun add -d @reliverse/relidler-cfg
```

4. the `.config/rse.ts` file will be created on first run. customize it to your needs.

## api for developers

use the sdk to build custom plugins or integrate rse capabilities into your own tools:

```sh
bun add @reliverse/rse-sdk
```

## show some love 🫶

if rse saved you time or made you smile:

- support on [github sponsors](https://github.com/sponsors/blefnk)
- drop a ⭐️ on [github](https://github.com/reliverse/rse)

it helps more than you think!

## contributing

everything in rse is built by [@blefnk nazar kornienko](https://github.com/blefnk) with love and caffeine. contributions are always welcome!

two ways to get started:

**classic way**:

```bash
git clone https://github.com/reliverse/rse.git
cd cli
code . # opens vscode editor
```

**rse way**:

```bash
rse cli
> clone an existing repository
> developer related  
> reliverse  
> cli
> y/n # y opens default editor
```

run `bun latest` to install dependencies, make your changes, and then:

```bash
git add .
git commit -m "your commit message"
git push
```

or use the rse way:

```bash
rse cli
> commit
<your commit message>
<press enter to push>
```

then head to [github](https://github.com/reliverse/rse/pulls) to open a pr.

## license

💖 [mit](./license) © 2025 [blefnk (nazar kornienko)](https://github.com/blefnk)
