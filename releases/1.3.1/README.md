# Botanix v1.3.1

**Release Channel:** `stable`
**Release Date:** 2025-08-21 15:04:34 UTC
**Git Tag:** `v1.3.1`
**Git SHA:** `41dd0fd56a7b7d36e5489e02ea64f89afd9725d2`

## Release Notes


### Bug Fixes

* **btc-server:** check is_coordinator before resetting pending pegouts ([#932](https://github.com/botanix-labs/Macbeth/issues/932)) ([6cacf76](https://github.com/botanix-labs/Macbeth/commit/6cacf7616408b8c93cbee423465b7bf92e8cef37))
* **btc-server:** pending pegout race condition ([#934](https://github.com/botanix-labs/Macbeth/issues/934)) ([34bb0a4](https://github.com/botanix-labs/Macbeth/commit/34bb0a4e41363905644edb40455795249b431206))
* pending pegouts race condition ([#938](https://github.com/botanix-labs/Macbeth/issues/938)) ([41dd0fd](https://github.com/botanix-labs/Macbeth/commit/41dd0fd56a7b7d36e5489e02ea64f89afd9725d2))

### Miscellaneous

* **release:** back-merge v1.3.0 from main to hotfix ([e874240](https://github.com/botanix-labs/Macbeth/commit/e874240667e96681f0c593b5a268e90c9faf1e7f))
* **release:** bump version to 1.3.1-hotfix.1 ([2689a0d](https://github.com/botanix-labs/Macbeth/commit/2689a0d0ed3b89703f18000352b60ccc6a2c95c1))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.1/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.1/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.1/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.1/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.3.1
docker pull ghcr.io/botanix-labs/botanix-btc-server:stable
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.3.1
docker pull ghcr.io/botanix-labs/botanix-reth-node:stable
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.3.1 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.3.1

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.3.1
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.1/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
