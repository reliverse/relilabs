# Reliverse's JS Alternative

> A modern, Rust-powered drop‑in replacement for JavaScript — reliable, deterministic, and fully compatible.

## ✨ Why ReliScript?

JavaScript powers the web, but decades of organic growth have left rough edges—runtime surprises, legacy syntax, and tooling quirks. **ReliScript (`.rse`)** brings Rust‑grade reliability and performance to everyday scripting while keeping **100% compatibility with existing modern JavaScript code**.

* **Rust core** – Memory‑safe, data‑race‑free compiler & toolchain.
* **Drop-in adoption** – Rename `.js` → `.rse`, run the build, ship.
* **Predictable runtime** – Deterministic semantics and explicit opt-ins for "unsafe" behaviour.
* **Progressive typing** – Opt-in static types (inspired by TypeScript) without losing JS dynamism.
* **Zero-cost interop** – Seamless mixing of `.js`, `.ts`, and `.rse` within one project.

## 🧭 Vision

* ReliScript is more than a language — it’s a movement toward rebuilding scripting from the ground up with correctness, composability, and care.  
* Inspired by Rust. Designed for the modern web. Built by developers who still believe JavaScript deserves better.

## 🚀 Quick Start

```bash
# 1 / Install the CLI (requires Rust toolchain ≥ 1.78)
cargo install reliscript-cli

# 2 / Transpile a single file to JavaScript
rse build src/app.rse --out dist/app.js

# 3 / Run your app as usual 🤘
node dist/app.js
```

> **Note** Until v0.2 the build output assumes ECMAScript 2022 targets.

## 📦 Installation Options

| Use‑case            | Command                                               |
|---------------------|-------------------------------------------------------|
| Global CLI          | `cargo install reliscript-cli`                        |
| Project local (npm) | `npm install --save-dev @reliverse/relisc`            |
| VS Code extension   | *Coming with M1 milestone*                            |

## 📝 Language Snapshot

```rse
// hello.rse
fn main() {
    let greeting: str = "Hello, Reli!";
    console.log(greeting);
}
```

Transpiles to:

```js
// hello.js (generated)
function main() {
    const greeting = "Hello, Reliverse!";
    console.log(greeting);
}
```

### Optional Typing

```rse
fn greet(name: str?) {
    console.log("Hi, " + (name ?? "friend") + "!");
}
```

## Planned Roadmap

| Milestone | Target 🎯 | Highlights |
|-----------|-----------|------------|
| **M0 – Bootstrap** | **Jun 2025** | Public repo launch, CI setup, minimal parser, `.rse` file recognition |
| **M1 – ES2022 Compatibility** | Dec 2025 | Complete modern JS grammar support, source maps, VS Code syntax highlighting |
| **M2 – Browser Integration (α)** | Jan 2026 | Reliverse Browser loads `.rse` natively, just like `.js` — no build step needed |
| **M3 – Reli Types (α)** | Jun 2026 | Optional static typing à la TypeScript, early type checker, editor support |
| **M4 – Borrowed Async** | Sep 2026 | Rust-style async model with green threads & compile-time race protection |
| **M5 – WebAssembly Backend** | Dec 2026 | Direct `.rse` to WASM compilation with auto-generated interop glue |
| **M6 – Standard Library v0.1** | Apr 2027 | Batteries included: ergonomic Web API wrappers, polyfill cleanup |
| **M7 – Self-Hosting Compiler** | Aug 2027 | ReliScript compiler rewritten in `.rse`, enters full dogfooding phase |
| **M8 – LTS 1.0** | Dec 2027 | Stability guarantees, plugin API, formal spec, long-term support |
| **M9 – Native Browser Adoption (β)** | Jan 2028 | Browser proposals, discussions with engines for `.rse` built-in support |

## Contributing

1. Fork & clone the repo
2. `cargo run --example playground` – hack the parser
3. Submit a PR following the Contributor Guide (soon)

## License

ReliScript is licensed under **MIT**.

> © 2025 Nazar Kornienko (blefnk), Reliverse
> Made with 🦀 & ☕️
