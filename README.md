# range-proof-benches

Various range proof implementations for 64 and 32 bit ranges and their benchmarks in Rust.
At the moment the following protocols are covered:
- D Boneh, B Fisch, A Gabizon, and Z Williamson. A simple range proof from polynomial commitments, 2020 [BFGW + KZG](https://hackmd.io/@dabo/B1U4kx8XI)
- Groth16 w/ Poseidon hash function
- Groth16 w/ Pedersen hash function
- Bulletproofs
- HashWires

```
# implementation attributes to https://github.com/roynalnaruto/range_proof with minor updates to dependencies.

cd BFDW/
cargo bench

# implementation attributes to https://github.com/MystenLabs/fastcrypto/blob/02d3d4fb096a5575fde71bbd6e0d337245ac1f53/fastcrypto/src/bulletproofs.rs without modification.

cd bulletproofs/
cargo bench

# implementation h/o to https://github.com/novifinancial/hashwires without modification.

cd hashwire/
cargo bench
```
