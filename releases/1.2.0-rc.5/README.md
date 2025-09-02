# Botanix v1.2.0-rc.5

**Release Channel:** `rc`
**Release Date:** 2025-09-02 16:49:24 UTC
**Git Tag:** `v1.2.0-rc.5`
**Git SHA:** `84e8b2aef60cd384b0380806daf86040d7e5472a`

## Release Notes


### Features

* **btc-server:** enfoce maximum tx weight limit during make_tx ([373cbcb](https://github.com/botanix-labs/Macbeth/commit/373cbcb2753d5a07caf98808fdcd13d1bd3ff790))
* **btc-server:** reduce pegout upper bound to more conservative value ([4300425](https://github.com/botanix-labs/Macbeth/commit/430042532d069ff967111c7f2ee505fdd667fe62))

### Bug Fixes

* **btc-server:** enforce max transaction weight limit on make_tx ([#943](https://github.com/botanix-labs/Macbeth/issues/943)) ([74b0e46](https://github.com/botanix-labs/Macbeth/commit/74b0e468a0e689d63926b705ff56148f031e6ad7))
* **btc-server:** fix logic for upper pegout bound ([16ddfcd](https://github.com/botanix-labs/Macbeth/commit/16ddfcdc1af207dd17420b7689b54112a725065e))
* **btc-server:** Removed metrics prefix ([#966](https://github.com/botanix-labs/Macbeth/issues/966)) ([72c381c](https://github.com/botanix-labs/Macbeth/commit/72c381cd84bc3182119af1545be30124adb5ba8e))
* **btc-server:** utxo recovery - script deserialization ([78a7ca8](https://github.com/botanix-labs/Macbeth/commit/78a7ca8396f221c2083289d1e201494e081e6913))
* **test:** fix script_hex in mockbitcoind ([4e0cc44](https://github.com/botanix-labs/Macbeth/commit/4e0cc441a623474873ead83851d4168f68241d15))
* **utxo-recovery:** resolve endian/type conversion issues ([#970](https://github.com/botanix-labs/Macbeth/issues/970)) ([bbf1b54](https://github.com/botanix-labs/Macbeth/commit/bbf1b5401d6c28bc70979d02d267fd3b5ea2e477))

### Code Refactoring

* **btc-server:** more logging around utxo recovery ([e1d6567](https://github.com/botanix-labs/Macbeth/commit/e1d65670d02fe1e7e3b57d6617322b1b49cf2af4))
* **btc-server:** use centralized OutPoint conversion in utxo recovery ([b3a8681](https://github.com/botanix-labs/Macbeth/commit/b3a8681cded505a854d56e799124259e2d6547e9))
* **btc-server:** utxo recovery log ([4dedd4f](https://github.com/botanix-labs/Macbeth/commit/4dedd4f9782d81fda74a2f08e9e6bc24b519da8c))
* **ntp:** remove ntp server logic ([#961](https://github.com/botanix-labs/Macbeth/issues/961)) ([4435919](https://github.com/botanix-labs/Macbeth/commit/4435919fd1c0835cbc8c3927620b5916fa5156cb))

### Documentation

* network deployment and release testing ([#752](https://github.com/botanix-labs/Macbeth/issues/752)) ([a5f8236](https://github.com/botanix-labs/Macbeth/commit/a5f82364661af7e2c9e56711c46e508b991d54a4))
* reth upgrade proposal ([#791](https://github.com/botanix-labs/Macbeth/issues/791)) ([500737c](https://github.com/botanix-labs/Macbeth/commit/500737cfe5e5d0cd2b85727939333e96f2d9260d))

### Tests

* **btc-server:** add integration test for utxo recovery ([09cb88e](https://github.com/botanix-labs/Macbeth/commit/09cb88ece15dab8c9a9c35c5c42e92397b041b6f))
* **btc-server:** extend unit test - test_utxo_recovery_data_conversion ([4c652a3](https://github.com/botanix-labs/Macbeth/commit/4c652a34a3e1b06ce4eb561c3d8aa9f6c47a7671))
* update conflict input test ([#958](https://github.com/botanix-labs/Macbeth/issues/958)) ([cba5b22](https://github.com/botanix-labs/Macbeth/commit/cba5b224bc8033461a6071abf9b854acbb899290))

### Miscellaneous

* **btc-server:** add pegout address to info log ([553cf9b](https://github.com/botanix-labs/Macbeth/commit/553cf9b254e2fb0e8155e44c0a46f0b011e9c0a8))
* **ci:** add tx_weight_limit test to ci ([7db26ab](https://github.com/botanix-labs/Macbeth/commit/7db26abe67fb75f4d67e238c9e1289b4b1cbf265))
* **test:** add utxo_recovery integration test ([7b3c9e5](https://github.com/botanix-labs/Macbeth/commit/7b3c9e52e0c7c69059dd95848e16e8c402bd91f3))
* update codeowners ([#971](https://github.com/botanix-labs/Macbeth/issues/971)) ([0c31906](https://github.com/botanix-labs/Macbeth/commit/0c31906905ed4c64d0e3a54c923435575e75c367))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.5/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.5/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.5/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.5/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.5
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.5
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.5 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.5

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.5
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.5/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
