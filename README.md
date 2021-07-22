This repository currently only fuzz the indexation.
You can add valid datasets in `/in`, it needs to be in csv currently.

# Setup
You need to install `cargo-afl`:
```bash
cargo install afl
```

# Compile
```bash
cargo afl build --release
```

# Run
```bash
cargo afl fuzz -i in -o out target/release/milli_index
```
