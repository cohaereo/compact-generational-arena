# `compact-generational-arena`
Extracted from [rapier](https://github.com/dimforge/rapier/blob/master/src/data/arena.rs) as a standalone crate

The implementation in rapier is based off [`generational-arena`](https://github.com/fitzgen/generational-arena)

Rapier changed the index key size from 64+64 (=128) bits to 32+32 (=64) bits, and made the index key `#[repr(C)]` as to make it FFI compatible
