# Botanix v1.4.0-hotfix.2

**Release Channel:** `hotfix`
**Release Date:** 2025-10-01 15:34:14 UTC
**Git Tag:** `v1.4.0-hotfix.2`
**Git SHA:** `b410e1771c8bdb01577fba11c85cd1404c48f567`

## Release Notes


### Features

* **btc-server:** add jwt validation to recover_missing_utxos ([2745e60](https://github.com/botanix-labs/Macbeth/commit/2745e607788ce37067c989c8d2bd1dd98ddc31d9))
* **btc-server:** add recover_missing_utxos method to BtcServerExtendedApi ([4364675](https://github.com/botanix-labs/Macbeth/commit/43646754e45263613a80952e36a641e29a94e201))
* **btc-server:** recover_missing_utxo grpc endpoint ([a479c28](https://github.com/botanix-labs/Macbeth/commit/a479c28494fa08cffaff3b878343845e0bc35e22))
* **btc-server:** update merkle root and flush when recovering missing utxos ([2881f67](https://github.com/botanix-labs/Macbeth/commit/2881f672b81234d0b156320cd5b7e1253d39b1a9))
* **reth:** add missing utxos on reth startup ([a5f0040](https://github.com/botanix-labs/Macbeth/commit/a5f004056f8a6cda5df9dd79037baf54ac2aaecb))
* **reth:** add optional argument for utxo recovery file ([cf62419](https://github.com/botanix-labs/Macbeth/commit/cf6241984c2d3e9a71535f648a20e9de52e6766e))

### Bug Fixes

* **btc-server:** utxo recovery - script deserialization ([bde5277](https://github.com/botanix-labs/Macbeth/commit/bde5277a3789edc97a388d5e1f93ab0b20444cf8))
* **test:** fix script_hex in mockbitcoind ([8a837b3](https://github.com/botanix-labs/Macbeth/commit/8a837b3695e3a4011062bbf926f0d67795aac232))

### Code Refactoring

* ** btc-server:** handle error properly instead of unwrap ([8128764](https://github.com/botanix-labs/Macbeth/commit/8128764d324ebe606f0b67f464374f81cae273ee))
* **authority:** utxo recovery file json to use camelCase ([1f221f1](https://github.com/botanix-labs/Macbeth/commit/1f221f1092151a811ee961fc88953de73e5a80b5))
* **btc-server:** code readability ([6a534db](https://github.com/botanix-labs/Macbeth/commit/6a534db66423fe7a48e568443176e959d7cf4905))
* **btc-server:** more logging around utxo recovery ([ed4e3a6](https://github.com/botanix-labs/Macbeth/commit/ed4e3a6a09348df492f7206cc2d998c3b82771c2))
* **btc-server:** move utxo recovery file reading logic to btc-server ([ee6a0b6](https://github.com/botanix-labs/Macbeth/commit/ee6a0b6e06363a5a0e51077631f7cce59b7e8109))
* **btc-server:** use centralized OutPoint conversion in utxo recovery ([9e72e2a](https://github.com/botanix-labs/Macbeth/commit/9e72e2aa8ede19183161a2d250f4f03b4e2bd6ba))
* **btc-server:** use TryFrom for reading utxo recovery file ([8e5059f](https://github.com/botanix-labs/Macbeth/commit/8e5059f50e898b9e3a09e3c650b0eba07ff893b0))
* **btc-server:** utxo recovery log ([b4af328](https://github.com/botanix-labs/Macbeth/commit/b4af3282ec26db554b4c747a4c5fd54e85af25cd))
* fixing merge conflicts when moving to hotfix branch ([f9860ab](https://github.com/botanix-labs/Macbeth/commit/f9860abb71921161388ac84029116b33f26a3daa))

### Tests

* **authority:** add unit tests for adding utxos on startup ([db773e4](https://github.com/botanix-labs/Macbeth/commit/db773e4f0ee715778fa9e3053db3a82c6461b405))
* **authority:** update utxo recovery unit test with real examples ([41b24a8](https://github.com/botanix-labs/Macbeth/commit/41b24a89f8995b08000b0bc6e287296711b89d41))
* **btc-server:** add integration test for utxo recovery ([1fe5855](https://github.com/botanix-labs/Macbeth/commit/1fe5855765156dc40bf8339d1526ff00443d15d7))
* **btc-server:** extend unit test - test_utxo_recovery_data_conversion ([74c4b83](https://github.com/botanix-labs/Macbeth/commit/74c4b838c1213e8a0ecd13de336b20215712a617))

### Miscellaneous

* **ci:** robust prepare binary for upload ([ab1cc6b](https://github.com/botanix-labs/Macbeth/commit/ab1cc6b8b494dd0297ce02406c95d72436722d2a))
* **ci:** switch build binaries to k8 runners ([8ca0ba2](https://github.com/botanix-labs/Macbeth/commit/8ca0ba2de95c2042fa57ecb812dfde193124484b))
* **test:** add utxo_recovery integration test ([48ceb48](https://github.com/botanix-labs/Macbeth/commit/48ceb4846bc1d33f00d5fb87dcd76e89affbaa9a))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.2/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.2/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.2/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.2/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.4.0-hotfix.2
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.4.0-hotfix.2
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.4.0-hotfix.2 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.4.0-hotfix.2

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.4.0-hotfix.2
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
