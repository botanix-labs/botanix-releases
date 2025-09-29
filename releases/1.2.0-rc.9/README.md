# Botanix v1.2.0-rc.9

**Release Channel:** `rc`
**Release Date:** 2025-09-29 19:12:48 UTC
**Git Tag:** `v1.2.0-rc.9`
**Git SHA:** `e1e7b3f867b74710481ed66ec622bd6b13153efc`

## Release Notes


### Features

* **btc-server:** add error log if invalid address passed into excluded_eth_addresses ([2067edc](https://github.com/botanix-labs/Macbeth/commit/2067edc4bed40179498dd2afeeab73e6cdb34f91))
* **btc-server:** add flag excluded_eth_addresses for coin selection ([49e0aad](https://github.com/botanix-labs/Macbeth/commit/49e0aad4f8520594939b5dab3a42f3740f13b8ea))
* **btc-server:** add flag excluded_eth_addresses for coin selection ([#990](https://github.com/botanix-labs/Macbeth/issues/990)) ([50da2e9](https://github.com/botanix-labs/Macbeth/commit/50da2e9cdafd73d4b595372cb8b7bbbffaae0112))
* **btc-server:** additional pegin pegout and signing metrics ([#988](https://github.com/botanix-labs/Macbeth/issues/988)) ([fd484fe](https://github.com/botanix-labs/Macbeth/commit/fd484feeed12f0064376608d94c2f98afa346301))

### Code Refactoring

* **btc-server:** refactor filter_excluded_utxos to remove unecessary cloning ([d85f659](https://github.com/botanix-labs/Macbeth/commit/d85f6593b8028ed76473660e3e843b39fd7bb514))
* **btc-server:** remove unused error type ([83c696b](https://github.com/botanix-labs/Macbeth/commit/83c696ba3ecc5adffe1ae1bc3a3c60b065a419d1))
* **btc-server:** use clap for parsing excluded_eth_addresses ([66deb32](https://github.com/botanix-labs/Macbeth/commit/66deb3207518deda665358679c6fe955c55d081b))
* **btc-server:** use hashmap.retain for eth address filtering ([4625e6a](https://github.com/botanix-labs/Macbeth/commit/4625e6a7c38049fb6bd64a42c218a26d13fa155c))
* **btc-sweep:** use all utxo for conflicting input selection ([02e9e7b](https://github.com/botanix-labs/Macbeth/commit/02e9e7be9af45dc59ce07f382fa60bd0233dca38))

### Miscellaneous

* **crates:** remove auto_doc_cfg ([7a51042](https://github.com/botanix-labs/Macbeth/commit/7a510424758882fd1bf32538ed953d7fe9e7c7cc))
* **crates:** remove auto_doc_cfg ([#994](https://github.com/botanix-labs/Macbeth/issues/994)) ([27f5f01](https://github.com/botanix-labs/Macbeth/commit/27f5f015fd6b8a9e877c5ae025adb28f04d420af))
* **crates:** remove doc_auto_cfg attribute ([7cd3315](https://github.com/botanix-labs/Macbeth/commit/7cd33155e55adcec978555d8b47affad6357db6d))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.9/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.9/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.9/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.9/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.9
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.9
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.9 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.9

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.9
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.9/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
