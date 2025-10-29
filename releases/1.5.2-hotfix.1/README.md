# Botanix v1.5.2-hotfix.1

**Release Channel:** `hotfix`
**Release Date:** 2025-10-29 16:48:06 UTC
**Git Tag:** `v1.5.2-hotfix.1`
**Git SHA:** `53394e93ae6dc3e9f8ba376f473d483b5fb9c7ca`

## Release Notes


### Bug Fixes

* **pegouts:** remove all finalized pegouts from pending pegouts list ([0d8e12d](https://github.com/botanix-labs/Macbeth/commit/0d8e12dbc2fc75839bf6489f79f80ad6c3a203ab))
* **pegouts:** remove all finalized pegouts from pending pegouts list ([#1019](https://github.com/botanix-labs/Macbeth/issues/1019)) ([53394e9](https://github.com/botanix-labs/Macbeth/commit/53394e93ae6dc3e9f8ba376f473d483b5fb9c7ca))

### Tests

* **outputs:** add test to validate finalized pegouts are removed from pending pegouts ([70bec97](https://github.com/botanix-labs/Macbeth/commit/70bec97a7fae2676bddac9476d43c13bc3794346))

### Miscellaneous

* **release:** back-merge v1.5.1 from main to hotfix ([bb55593](https://github.com/botanix-labs/Macbeth/commit/bb555939c84538c688eba862002f258ebbaa06da))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.5.2-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.5.2-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.5.2-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.5.2-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.5.2-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.5.2-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.5.2-hotfix.1 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.5.2-hotfix.1

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.5.2-hotfix.1
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.5.2-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
