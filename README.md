# OMG IDL v4 grammar for pest

[![Docs](https://docs.rs/pest_idl_v4_grammar/badge.svg)](https://docs.rs/pest_idl_v4_grammar)
[![Crates.io](https://img.shields.io/crates/d/pest_idl_v4_grammar.svg)](https://crates.io/crates/pest_idl_v4_grammar)
[![Crates.io](https://img.shields.io/crates/v/pest_idl_v4_grammar.svg)](https://crates.io/crates/pest_idl_v4_grammar)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Object Management Group [Interface Definition Language v4.1](http://www.omg.org/spec/IDL/4.1/) grammar for [pest](https://github.com/pest-parser/pest)


## Status

This grammar was manually converted from the EBNF Consolidated IDL Grammar Annex of the specification.  As such, it has not been fully tested.  In many cases pest's eager matching causes an unexpected rule to match when the rules are ordered as in the reference EBNF grammar.  As there is not a comprehensive test suite / example IDL file for this project, it is likely there are other undiscovered errors of this type.  Problem reports are appreciated.  Bonus points if an example triggering the error is included.


## Usage

pest_idl_v4_grammar requires [Cargo and Rust](https://www.rust-lang.org/en-US/downloads.html).

Add the following to `Cargo.toml`:

```toml
pest_idl_v4_grammar = "*"
```

and in your Rust `lib.rs` or `main.rs`:

```rust
extern crate pest;
use pest::Parser;
extern crate pest_idl_v4_grammar;
use pest_idl_v4_grammar::{Rule,IdlParser};


```

## License

Licensed under either of

 * Apache License, Version 2.0
   ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license
   ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

## Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.

