# Reth Snapshots
Sync your Reth archive nodes in hours, instead of weeks, with our snapshots.

## BSC

**Size**: 4.36TB  
**Extracted Size**: 6.41TB  
**Latest Block**: 40817260  
**Path**: https://snapshots.fuzz.land/bsc.tar.gz

**Instructions**

Run Reth BSC node
```
# setup rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
# build reth
git clone https://github.com/bnb-chain/reth.git && cd reth
make build-bsc
./target/release/bsc-reth node --datadir=./db
```

Get snapshot
```
aria2c -s14 -x14 -k100M https://snapshots.fuzz.land/bsc.tar.gz
tar -xzvf bsc.tar.gz
```

Then, kill the node and cover `./db` with the extracted files

## ETH
todo

## Op
todo

## Base
todo

## Arbitrum
todo
