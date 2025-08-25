# Botanix v1.3.2

**Release Channel:** `stable`
**Release Date:** 2025-08-25 23:46:05 UTC
**Git Tag:** `v1.3.2`
**Git SHA:** `ae90781ff7e9d89945006709ef7725efd6ab5f61`

## Release Notes


### Bug Fixes

* **config:** increase mainnet epoch length to 100 ([f173e7a](https://github.com/botanix-labs/Macbeth/commit/f173e7a430f8ee9a410bd1f59a77b2bafd93c551))
* **log:** set frost command log to debug ([d356455](https://github.com/botanix-labs/Macbeth/commit/d356455f81f2d5cbc190e04176ac245e18bf59c0))
* **log:** set frost command log to debug ([#954](https://github.com/botanix-labs/Macbeth/issues/954)) ([cc17edd](https://github.com/botanix-labs/Macbeth/commit/cc17edd5f888907013f665a2000efb9cdfce5097))
* **pegouts:** don't store pegout if in finalized pegouts list ([089c8fd](https://github.com/botanix-labs/Macbeth/commit/089c8fd4b10cb9c034e0e44b7336e24db28f4e6e))
* **pegouts:** don't store pegout if it has been broadcasted ([419c57a](https://github.com/botanix-labs/Macbeth/commit/419c57aa1bbcf12d4a4985d57b2dc417f92121e9))
* **pegouts:** remove finalized pegout from pending pegout list ([15c3cdf](https://github.com/botanix-labs/Macbeth/commit/15c3cdfb6e447c32a980b156263b22f37a9ed4de))
* remove finalized pegout from pending pegout list ([#944](https://github.com/botanix-labs/Macbeth/issues/944)) ([e55c0f6](https://github.com/botanix-labs/Macbeth/commit/e55c0f6e86e8bb1a9670f461c6662639a6ea5440))
* **wallet-sync:** change log levels ([33f6446](https://github.com/botanix-labs/Macbeth/commit/33f6446c009fdc28653281bc6d7a551a0f04f1c2))
* **wallet-sync:** increase epoch length ([#953](https://github.com/botanix-labs/Macbeth/issues/953)) ([99ae576](https://github.com/botanix-labs/Macbeth/commit/99ae5768edfc4cad6950cbf946bbbeb39b902937))

### Miscellaneous

* **logs:** set wallet state logs to trace for btc-server ([cd375e9](https://github.com/botanix-labs/Macbeth/commit/cd375e9be9433b2526fa5b06100e91c9bacd1d16))
* merge hotfix into main ([#945](https://github.com/botanix-labs/Macbeth/issues/945)) ([ae90781](https://github.com/botanix-labs/Macbeth/commit/ae90781ff7e9d89945006709ef7725efd6ab5f61))
* **release:** back-merge v1.3.1 from main to hotfix ([f2da833](https://github.com/botanix-labs/Macbeth/commit/f2da83302796c23d6a2da491c78b77d94eb3a679))
* **release:** bump version to 1.3.2-hotfix.1 ([7aa665d](https://github.com/botanix-labs/Macbeth/commit/7aa665d8a3639a18e61c6840fb508b4e7fd5d46f))
* **release:** bump version to 1.3.2-hotfix.2 ([4cc466f](https://github.com/botanix-labs/Macbeth/commit/4cc466fbf0b127d5a01fffbe01b7ecc74c1e8d8c))
* **release:** bump version to 1.3.2-hotfix.3 ([ec3d903](https://github.com/botanix-labs/Macbeth/commit/ec3d903d948ce83993d3e014a204cdd0f8689305))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.2/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.2/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.2/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.2/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.3.2
docker pull ghcr.io/botanix-labs/botanix-btc-server:stable
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.3.2
docker pull ghcr.io/botanix-labs/botanix-reth-node:stable
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.3.2 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.3.2

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.3.2
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.2/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
