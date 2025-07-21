# Botanix v1.1.12

**Release Channel:** `stable`
**Release Date:** 2025-07-21 20:38:59 UTC
**Git Tag:** `v1.1.12`
**Git SHA:** `2e730b166a2d18bcf8b9441f7a4d1dbb03656709`

## Release Notes


### Continuous Integration

* semantic release flow ([#749](https://github.com/botanix-labs/Macbeth/issues/749)) ([316400d](https://github.com/botanix-labs/Macbeth/commit/316400d2b8375234c598788f05b96ac620b8c135))

### Miscellaneous

* bump to v1.1.12 ([ddb0e92](https://github.com/botanix-labs/Macbeth/commit/ddb0e9228326d9d0e8842a5ed6ab5d6719bc3fba))
* merge hotfix into main ([#862](https://github.com/botanix-labs/Macbeth/issues/862)) ([2e730b1](https://github.com/botanix-labs/Macbeth/commit/2e730b166a2d18bcf8b9441f7a4d1dbb03656709))
* **release:** bump version to 1.1.11-hotfix.1 ([997becb](https://github.com/botanix-labs/Macbeth/commit/997becb3dc820d01d435ece4a426de15023af8b5))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.1.12/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.1.12/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.1.12/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.1.12/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.1.12
docker pull ghcr.io/botanix-labs/botanix-btc-server:stable
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.1.12
docker pull ghcr.io/botanix-labs/botanix-reth-node:stable
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.1.12 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.1.12

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.1.12
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.1.12/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
