# Patch

> **_NOTE:_**  This patch adds atomic-cas polyfill to bytes for targets like thumbv6m-none-eabi until the following PR/issue is resolved:
>
> * https://github.com/tokio-rs/bytes/pull/467
> * https://github.com/tokio-rs/bytes/issues/461

The patch can be applied by adding the following segment to root Cargo.toml:

````TOML
[patch.crates-io]
bytes = { git = "ssh://git@github.com/pegasus-aero/rt-bytes.git", branch = "cfg_target_has_atomic" }
````
