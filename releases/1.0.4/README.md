# Botanix v1.0.4

**Release Channel:** `stable`
**Release Date:** 2025-08-05 13:48:02 UTC
**Git Tag:** `v1.0.4`
**Git SHA:** `15f3d294c54516c1cdca0447fef3fc822f186f55`

## Release Notes


### Continuous Integration

* test fix for public repo ([be79803](https://github.com/botanix-labs/macbeth-release/commit/be79803c748874dc26739e82e3b85126e25ac055))

### Miscellaneous

* **release:** back-merge v1.0.3 from main to hotfix ([2adbcb8](https://github.com/botanix-labs/macbeth-release/commit/2adbcb834a03513f02c210aca9ad3c4242e732c1))
* **release:** bump version to 1.0.4-hotfix.1 ([54dc98d](https://github.com/botanix-labs/macbeth-release/commit/54dc98d2406c630042beaa16bc0759e8113c6d99))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.0.4/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.0.4/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.0.4/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.0.4/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.0.4
docker pull ghcr.io/botanix-labs/botanix-btc-server:stable
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.0.4
docker pull ghcr.io/botanix-labs/botanix-reth-node:stable
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.0.4 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.0.4

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.0.4
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.0.4/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
