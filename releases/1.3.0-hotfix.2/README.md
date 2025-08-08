# Botanix v1.3.0-hotfix.2

**Release Channel:** `hotfix`
**Release Date:** 2025-08-08 02:50:00 UTC
**Git Tag:** `v1.3.0-hotfix.2`
**Git SHA:** `2f9db4893b400abcf203373c97d04ccda3b326f6`

## Release Notes


### Bug Fixes

* **botanix-up:** pass is_rpc_node param ([1cb555a](https://github.com/botanix-labs/Macbeth/commit/1cb555a09e5c6d3d223b1a0fa3412c4ffd251d23))

### Tests

* **rpc_node:** port changes from closed pr 740 ([0dff40d](https://github.com/botanix-labs/Macbeth/commit/0dff40d726615eef24c0fa112b632e471e3fe952))
* **rpc_node:** refactor setup and test ([eef415a](https://github.com/botanix-labs/Macbeth/commit/eef415a58528bfc10835dde053b4e384d6e0d0c3))
* **rpc_node:** spawn cometbft node for each rpc node ([6acf5ac](https://github.com/botanix-labs/Macbeth/commit/6acf5ace0c4d797f7c60cc63b01efe113595f17e))
* **rpc:** and zmq address to bitcoind ([274477d](https://github.com/botanix-labs/Macbeth/commit/274477d28edd80f195f6bc3816bcd8996c86c25a))

### Build System

* **import:** add back missed import ([c5c23c8](https://github.com/botanix-labs/Macbeth/commit/c5c23c8eb5ab2865ed9a8bdc368a81d0e4cad553))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.0-hotfix.2/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.0-hotfix.2/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.0-hotfix.2/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.3.0-hotfix.2/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.3.0-hotfix.2
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.3.0-hotfix.2
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.3.0-hotfix.2 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.3.0-hotfix.2

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.3.0-hotfix.2
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.3.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
