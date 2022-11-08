---
title: Formatting Rust Code
date: "2022-11-08"
description: "How to format Rust code"
---

To install:
```
    rustup component add rustfmt
```

To run on a cargo project in the current working directory:
```
    cargo fmt
``` 

To format individual files
```
    rustfmt lib/lib.rs src/main.rs
```

[Official Documentation](https://github.com/rust-lang/rustfmt)