# Botanix v1.2.0-hotfix.3

**Release Channel:** `hotfix`
**Release Date:** 2025-08-05 18:40:03 UTC
**Git Tag:** `v1.2.0-hotfix.3`
**Git SHA:** `2ad22b078fe98427b9ead87b57b683b27ae872ce`

## Release Notes


### Features

* runtime version 3 adjust floor base fee! ([#901](https://github.com/botanix-labs/Macbeth/issues/901)) ([2ad22b0](https://github.com/botanix-labs/Macbeth/commit/2ad22b078fe98427b9ead87b57b683b27ae872ce))

### Code Refactoring

* set floor base fee to 0.0005 GWEI ([fb62d01](https://github.com/botanix-labs/Macbeth/commit/fb62d010b396712e5b816565d488092fb9085efa))

### Continuous Integration

* allow for stable release to persist ([b0cb977](https://github.com/botanix-labs/Macbeth/commit/b0cb977544dbc0f825f579f17499ff1975b2bc4e))
* allow for stable release to persist ([#898](https://github.com/botanix-labs/Macbeth/issues/898)) ([9785f86](https://github.com/botanix-labs/Macbeth/commit/9785f86cc0b99e6a1812aa2df3fb00f3a6e4ca11))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.3/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.3/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.3/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.3/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.3
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-hotfix.3
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.3 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.3

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-hotfix.3
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
