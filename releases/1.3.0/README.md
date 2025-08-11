# Botanix v1.3.0

**Release Channel:** `stable`
**Release Date:** 2025-08-11 19:32:22 UTC
**Git Tag:** `v1.3.0`
**Git SHA:** `844163e84961a8e218dc334add0e6dd74f415475`

## Release Notes


### Features

*  command to rollback blocks ([#908](https://github.com/botanix-labs/Macbeth/issues/908)) ([ad84301](https://github.com/botanix-labs/Macbeth/commit/ad84301e6373e2048c1a97c0083b9c3cf7b4eb96))
*  command to rollback blocks ([#909](https://github.com/botanix-labs/Macbeth/issues/909)) ([45d3044](https://github.com/botanix-labs/Macbeth/commit/45d30446e77ce8e32d99ec6751c4d3ef88f12425))

### Bug Fixes

* **abci:** set version 0 to recover testnet ([#914](https://github.com/botanix-labs/Macbeth/issues/914)) ([1b9f87c](https://github.com/botanix-labs/Macbeth/commit/1b9f87c0f36c1848656236390523fed431271c61))
* **botanix-up:** pass is_rpc_node param ([1cb555a](https://github.com/botanix-labs/Macbeth/commit/1cb555a09e5c6d3d223b1a0fa3412c4ffd251d23))
* **import:** remove duplicate import ([b6621dc](https://github.com/botanix-labs/Macbeth/commit/b6621dcacbe689991704671393e32c8659b698c7))

### Code Refactoring

* **peers:** add upstream trusted peers logic ([ffd5d95](https://github.com/botanix-labs/Macbeth/commit/ffd5d95f56921ca5f290a0d566f813b8ee34714e))
* **peers:** add upstream trusted peers logic ([#913](https://github.com/botanix-labs/Macbeth/issues/913)) ([0bb1c0d](https://github.com/botanix-labs/Macbeth/commit/0bb1c0d91e59ae33c35883f2de460b01b1bac79b))

### Tests

* **rpc_node:** port changes from closed pr 740 ([0dff40d](https://github.com/botanix-labs/Macbeth/commit/0dff40d726615eef24c0fa112b632e471e3fe952))
* **rpc_node:** refactor setup and test ([eef415a](https://github.com/botanix-labs/Macbeth/commit/eef415a58528bfc10835dde053b4e384d6e0d0c3))
* **rpc_node:** spawn cometbft node for each rpc node ([6acf5ac](https://github.com/botanix-labs/Macbeth/commit/6acf5ace0c4d797f7c60cc63b01efe113595f17e))
* **rpc:** and zmq address to bitcoind ([274477d](https://github.com/botanix-labs/Macbeth/commit/274477d28edd80f195f6bc3816bcd8996c86c25a))

### Build System

* **import:** add back missed import ([c5c23c8](https://github.com/botanix-labs/Macbeth/commit/c5c23c8eb5ab2865ed9a8bdc368a81d0e4cad553))

### Miscellaneous

* **release:** back-merge v1.2.0 from main to hotfix ([e1cf64f](https://github.com/botanix-labs/Macbeth/commit/e1cf64f988188ed9e4fffa782569df4a74e189d4))
* **release:** bump version to 1.3.0-hotfix.1 ([4ac14db](https://github.com/botanix-labs/Macbeth/commit/4ac14db43faa1db42651124d3fc1691c6ffc1c00))
* **release:** bump version to 1.3.0-hotfix.2 ([8676d1c](https://github.com/botanix-labs/Macbeth/commit/8676d1c66e03ea9a022b3a72a2ff2966260f2c83))
* **release:** bump version to 1.3.0-hotfix.3 ([4c98011](https://github.com/botanix-labs/Macbeth/commit/4c98011fd3df42216137b32b1324366447903f49))
* **release:** bump version to 1.3.0-hotfix.4 ([89c4926](https://github.com/botanix-labs/Macbeth/commit/89c4926c7ab8c42ec7fa70b0c6f6ef56ee3f9e6d))
* **release:** bump version to 1.3.0-hotfix.5 ([72abd13](https://github.com/botanix-labs/Macbeth/commit/72abd138b3855669b29f6674a2cce485bf23a0c5))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.0/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.0/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.0/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.3.0/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.3.0
docker pull ghcr.io/botanix-labs/botanix-btc-server:stable
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.3.0
docker pull ghcr.io/botanix-labs/botanix-reth-node:stable
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.3.0 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.3.0

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.3.0
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.3.0/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
