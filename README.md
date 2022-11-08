# cargo-leptos

Build tool for [Leptos](https://crates.io/crates/leptos)

# Installation

You need the following command line tools installed:

- [sass](https://sass-lang.com/dart-sass)
- [web-pack](https://rustwasm.github.io/wasm-pack/)

Install with: `cargo install --path .`

# Use

Help: `cargo leptos --help`

Cargo leptos assumes that you have three cargo projects:

- _app_: the app logic (feature: **csr**, target: **wasm** or **current**).
- _client_: the client packaging of _app_ (feature: **hydrate**, target: **wasm**)
- _server_: the server packaging of _app_ (feature: **ssr**, target: **current**)

You should not use a cargo workspace.

The configuration is done in a `leptos.toml` file in the root of the project. A default one can be generated by running: `cargo leptos init`. All options are documented there.
