# FLASH

FLASH is a static analyzer for asynchronous liveness hazards such as deadlock
and starvation in real-world Rust. It extracts
asynchronous information from MIR, constructs field-sensitive lock identities,
and builds a wait-for graph that represents Rust's asynchronous semantics, on
which it performs liveness hazard detection. The implementation lives in
`rapx/src/analysis/future_lock`.

**Note**: The code is currently being prepared and will be uploaded prior to the start of the conference on May 17, 2027.

## Usage

```console
cargo rapx -A
```

## Acknowledgements

FLASH is built on [RAPx](https://github.com/Artisan-Lab/RAPx), the Rust Analysis
Platform with Extensions developed by Artisan-Lab at Fudan University. FLASH is
released under the same license as RAPx (MPL-2.0).
