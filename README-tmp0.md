# 🌌 **rse**: @reliverse/rse | (prev. reliverse cli: @reliverse/rse) | [reliverse.org](https://reliverse.org)

[💖 github sponsors](https://github.com/sponsors/blefnk) • [💬 discord](https://discord.gg/pb8ukbwpsj) • [✨ repo](https://github.com/reliverse/rse) • [📦 npm](https://npmjs.com/@reliverse/rse) • [📚 docs](https://blefnk.reliverse.org/blog/my-products/reliverse-cli)

## what is rse?

rse (**r**eliver**se**) is the all-in-one dev environment.

- **project creation & management**: spin up new projects in seconds.
- **ai-powered dev tools**: code gen, refactor, image gen, and more.
- **modern build system**: bundle, publish, and manage js/ts projects to npm.
- 🔜 **universal package registry**: public, private, whatever.
- 🔜 **alternative js ecosystem**: safer, saner, predictable. no more dependency hell.

start from scratch or supercharge what you've got. rse is bun on steroids, with a chainsaw.

## terminology

- `rse` → **reliverse standard environment**: the platform, the rules.
- `reli` → **reliverse**: the toolchain, the engine.
- `rse build` → the build/publish system (ex-relidler).  
  one command, all the power.

## core features

### project management

- 🚀 launch new projects or load templates instantly
- 🔧 refactor, inject libraries, and fix your codebase—safely, fast
- ⚙️ automate the boring (eslint, env, config, etc.)
- 🌐 push to github, deploy to vercel—one command, done
- 🏗️ next.js, anything else—rse doesn't care, it just works

### ai-powered development

- 🤖 chat with rse ai—get answers, code, whatever
- 🦾 generate/refactor code with ai, no hand-holding
- 🎨 create images from text, straight to your uploads
- 🧹 ai linting—find and fix issues before you even notice

### build system

- 📦 build/publish js/ts projects—no config hell
- 🦄 monorepo or standalone—doesn't matter
- 🔄 auto versioning, auto publishing, auto everything
- 🛠️ typescript path aliases? converted, handled, done
- 🔌 plugin system—extend, break, rebuild as you like

## getting started

**prereqs:** git, node.js, and a package manager (bun, pnpm, yarn, npm).  
if you don't have these, you're not ready.

### install

```sh
bun i -g @reliverse/rse
```

**update:**

```sh
rse update
```

### quick start

launch the wizard:

```sh
rse cli
```

first run spits out `.reliverse/reliverse.config.{ts,jsonc}`.  
tweak it, break it, make it yours.

## commands

### core

- `rse cli` — interactive wizard, project creation, upgrades, all in one
- `rse logout` — nuke your credentials
- `rse studio` — open the visual brain of rse
- `rse --help` — list every command, no excuses

### ai

- `rse ai <prompt>` — chat with rse ai, get instant answers
- `rse ai code <prompt> <paths>` — generate or refactor code, ai-style
- `rse ai gen <prompt>` — create images from text, zero effort
- `rse ai lint <prompt> <paths>` — linting and bug finder with ai

### project

- `rse init` — start a new rse project, minimal and clean
- `rse add` — drop in components, libs, or tools—no manual wiring
- `rse add -g <something>` — install global tools or desktop apps, system-wide
- `rse add rule <something>` — inject ai ide rules for any editor

### utility

- `rse clone` — clone github repos or convert webpages to llm-ready content
- `rse cmod` — apply codemods, refactor at scale
- `rse env` — generate .env files, skip the typos
- `rse multireli` — batch-generate configs for mass project creation
- `rse upload` — upload media to uploadthing, uploadcare, whatever

### build system

- `rse build cli` — build and publish, no drama
- `rse build tools --tool <tool>` — run standalone build tools:
  - `agger` — auto-export aggregator
  - `librer` — build/publish multiple libs from one repo
  - `merger` — merge files, fast
  - `splitter` — split files, cleaner
  - `adder` — add components/templates, instantly
  - `initter` — project init, automated
  - `certer` — manage certs, no sweat

## build system config

1. create config:

    ```sh
    rse build cli
    ```

2. update `.gitignore`:

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

4. `.config/rse.ts` is created on first run.  
   edit it, own it.

## api for developers

build plugins, extend rse, or hijack the sdk for your own tools:

```sh
bun add @reliverse/rse-sdk
```

## show some love 🫶

if rse saved you time or made you grin:

- [github sponsors](https://github.com/sponsors/blefnk)
- ⭐️ [github](https://github.com/reliverse/rse)

it matters. open source lives on this.

## contribute. please 😽

rse is built by [@blefnk nazar kornienko](https://github.com/blefnk)  
contributions? always welcome. bring your best.

**classic way:**

```bash
git clone https://github.com/reliverse/rse.git
cd cli
code .
```

**reliverse way:**

```bash
rse cli
> clone an existing repository
> developer related
> reliverse
> cli
> y/n # y opens your editor
```

install deps, make your changes, then:

```bash
git add .
git commit -m "your commit message"
git push
```

or the rse way:

```bash
rse cli
> commit
<your commit message>
<press enter to push>
```

open a pr: [github](https://github.com/reliverse/rse/pulls)

## license

💖 [mit](./license) © 2025 [blefnk (nazar kornienko)](https://github.com/blefnk)

## tl;dr

rse: the last dev tool you'll ever need.
