# Amazon Ion Schema Rust
[![License](https://img.shields.io/hexpm/l/plug.svg)](https://github.com/amzn/ion-schema-rust/blob/main/LICENSE)
[![Rust](https://github.com/amzn/ion-schema-rust/workflows/Rust/badge.svg)](https://github.com/amzn/ion-schema-rust/actions?query=workflow%3A%22Rust%22)

An implementation of [Amazon Ion Schema](http://amzn.github.io/ion-schema) in Rust.

**This package is considered experimental, under active/early development, and the API is subject to change.**

## Development

This repository contains [git submodules](https://git-scm.com/docs/git-submodule)
called `ion-schema-schemas` and `ion-schema-tests`, which holds test data used by
this library's unit tests.

The easiest way to clone the `ion-schema-rust` repository and initialize its submodules
is to run the following command:

```bash
$ git clone --recursive https://github.com/amzn/ion-schema-rust.git ion-schema-rust
```

Alternatively, the submodule may be initialized independently from the clone
by running the following commands:

```bash
$ git submodule init
$ git submodule update
```

Building the project,
```bash
$ cargo build --workspace --all-targets
```

Running all tests for `ion-schema-rust`,
```bash
$ cargo test --workspace
```

## License

This library is licensed under the Apache-2.0 License.
