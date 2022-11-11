---
title: Running Tests Conditionally in Rust
date: "2022-11-11"
description: "Running Tests Conditionally in Rust"
---

In Rust it is possible to run tests conditionally.

Feature-gated test:
```
#[test]
#[cfg(feature = "add-a-variant")]
fn add_a_variant() {...}
```

It will run only if the following parameters are used:
```
cargo test --features add-a-variant
```

This is useful when doing TDD and if the code which will pass the test is not ready yet. We can mark the test as pending until the feature is ready.