# Botanix v1.3.2-hotfix.1

**Release Channel:** `hotfix`
**Release Date:** 2025-08-22 17:11:09 UTC
**Git Tag:** `v1.3.2-hotfix.1`
**Git SHA:** `e55c0f6e86e8bb1a9670f461c6662639a6ea5440`

## Release Notes


### Bug Fixes

* **pegouts:** don't store pegout if in finalized pegouts list ([089c8fd](https://github.com/botanix-labs/Macbeth/commit/089c8fd4b10cb9c034e0e44b7336e24db28f4e6e))
* **pegouts:** don't store pegout if it has been broadcasted ([419c57a](https://github.com/botanix-labs/Macbeth/commit/419c57aa1bbcf12d4a4985d57b2dc417f92121e9))
* **pegouts:** remove finalized pegout from pending pegout list ([15c3cdf](https://github.com/botanix-labs/Macbeth/commit/15c3cdfb6e447c32a980b156263b22f37a9ed4de))
* remove finalized pegout from pending pegout list ([#944](https://github.com/botanix-labs/Macbeth/issues/944)) ([e55c0f6](https://github.com/botanix-labs/Macbeth/commit/e55c0f6e86e8bb1a9670f461c6662639a6ea5440))

### Miscellaneous

* **logs:** set wallet state logs to trace for btc-server ([cd375e9](https://github.com/botanix-labs/Macbeth/commit/cd375e9be9433b2526fa5b06100e91c9bacd1d16))
* **release:** back-merge v1.3.1 from main to hotfix ([f2da833](https://github.com/botanix-labs/Macbeth/commit/f2da83302796c23d6a2da491c78b77d94eb3a679))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.2-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.2-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.2-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.2-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.3.2-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.3.2-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.3.2-hotfix.1 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.3.2-hotfix.1

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.3.2-hotfix.1
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
