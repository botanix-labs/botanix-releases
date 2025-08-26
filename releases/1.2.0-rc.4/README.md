# Botanix v1.2.0-rc.4

**Release Channel:** `rc`
**Release Date:** 2025-08-26 01:02:48 UTC
**Git Tag:** `v1.2.0-rc.4`
**Git SHA:** `2f30163fb45901f9703c97f3897b8955822fb876`

## Release Notes


### Features

* **btc-server:** Added many new metrics, cleanup, versioning ([#933](https://github.com/botanix-labs/Macbeth/issues/933)) ([fd9bbee](https://github.com/botanix-labs/Macbeth/commit/fd9bbeebceb9486ea2fd87f1a362d25588a86a95))
* **reth:** Created new crates botanix-chainspec and botanix-hardforks ([#847](https://github.com/botanix-labs/Macbeth/issues/847)) ([4473aa7](https://github.com/botanix-labs/Macbeth/commit/4473aa7851511ff4782b465ac462585151bfd9da))

### Bug Fixes

* **btc-server:** check is_coordinator before resetting pending pegouts ([#932](https://github.com/botanix-labs/Macbeth/issues/932)) ([c388961](https://github.com/botanix-labs/Macbeth/commit/c38896185e1c8b3cbcd944772f9c215db3a6e25c))

### Code Refactoring

* **btc-server:** helper method to calculate max inputs for psbt ([#942](https://github.com/botanix-labs/Macbeth/issues/942)) ([a49662a](https://github.com/botanix-labs/Macbeth/commit/a49662a66a427d38046c218a6356834eed66e65e))
* **btc-server:** helper method to calculate maximum number of psbt inputs ([6edab39](https://github.com/botanix-labs/Macbeth/commit/6edab3956ec70b956966a32b77c43cd149663f2b))
* **btc-server:** readability improvement for calculate max input ([2766e60](https://github.com/botanix-labs/Macbeth/commit/2766e605b833a7a63d473f1d6e6fb0b4a60650c3))
* **btc-server:** readability improvement for calculate max input ([#952](https://github.com/botanix-labs/Macbeth/issues/952)) ([18aec30](https://github.com/botanix-labs/Macbeth/commit/18aec3006e53e73c82f250994f6771adf73a8299))

### Miscellaneous

* cherry pick hotfix into develop ([#955](https://github.com/botanix-labs/Macbeth/issues/955)) ([83569e3](https://github.com/botanix-labs/Macbeth/commit/83569e3eb1f1aa068b80b94b54c3a41dcf41bb72))
* **deps:** bump actions/checkout from 4 to 5 ([#930](https://github.com/botanix-labs/Macbeth/issues/930)) ([af0c9e6](https://github.com/botanix-labs/Macbeth/commit/af0c9e6d0537ec85427e76f8a56efb4295cccb35))
* **deps:** bump amannn/action-semantic-pull-request from 5 to 6 ([#931](https://github.com/botanix-labs/Macbeth/issues/931)) ([642d58b](https://github.com/botanix-labs/Macbeth/commit/642d58b92bb0441b83ab651179b56e5ae575de3b))
* merge develop into rc ([#937](https://github.com/botanix-labs/Macbeth/issues/937)) ([2f30163](https://github.com/botanix-labs/Macbeth/commit/2f30163fb45901f9703c97f3897b8955822fb876))
* update cargo.lock ([d567307](https://github.com/botanix-labs/Macbeth/commit/d56730788f299ad02ba4a9a92cf8d57ab44b0147))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.4/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.4/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.4/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.4/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.4
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.4
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.4 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.4

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.4
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.4/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
