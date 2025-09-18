# Botanix v1.2.0-rc.6

**Release Channel:** `rc`
**Release Date:** 2025-09-18 09:47:21 UTC
**Git Tag:** `v1.2.0-rc.6`
**Git SHA:** `46c377b79695c1415fb4cac14121fa18e5541a9f`

## Release Notes


### Features

* Added get validator signatures cli command ([e537bd2](https://github.com/botanix-labs/Macbeth/commit/e537bd29da13d092362f88f44a2d37a1934ee387))
* Added get validator signatures cli command ([#980](https://github.com/botanix-labs/Macbeth/issues/980)) ([3049958](https://github.com/botanix-labs/Macbeth/commit/304995869dc0f1ca02620145dd4ed25aba487e4d))

### Bug Fixes

* **btc-server:** add backwards compatibility for RpcUtxo script format change ([049e925](https://github.com/botanix-labs/Macbeth/commit/049e925e65a9eef86d6531a6076aa1c8951c3722))
* fixed metrics prefix using a global registry one ([bade8dd](https://github.com/botanix-labs/Macbeth/commit/bade8dd1bf8f43fce6aeb2ae5d6dbd65c304d9f6))
* fixed metrics prefix using a global registry one ([#979](https://github.com/botanix-labs/Macbeth/issues/979)) ([32c8169](https://github.com/botanix-labs/Macbeth/commit/32c8169efce781e769fcb90f8b96949696e5d42d))
* **rpc:** Remove additional encoding for rpc utxo scripts ([8949bcb](https://github.com/botanix-labs/Macbeth/commit/8949bcb6d107b793960d4b0c2617e92a7369c3f1))
* **rpc:** Remove additional encoding for rpc utxo scripts ([#949](https://github.com/botanix-labs/Macbeth/issues/949)) ([ddeb402](https://github.com/botanix-labs/Macbeth/commit/ddeb40200079ffe718e6f51391f41448daa945af))

### Code Refactoring

* cargo fmt ([b0e374b](https://github.com/botanix-labs/Macbeth/commit/b0e374b4181083555c18deba26a26086416b160c))

### Tests

* **btc-server:** add unit test for db rpc utxo conversion ([09f57f6](https://github.com/botanix-labs/Macbeth/commit/09f57f6b5799da6526c5b0624f1a1d3be0c19e61))
* **btc-server:** remove exact fee amount from psbt validation unit test ([229b43b](https://github.com/botanix-labs/Macbeth/commit/229b43bc37d32a198bb14fa49e742ec40910f821))

### Miscellaneous

* rc for testing util & metrics features ([#982](https://github.com/botanix-labs/Macbeth/issues/982)) ([46c377b](https://github.com/botanix-labs/Macbeth/commit/46c377b79695c1415fb4cac14121fa18e5541a9f))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.6/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.6/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.6/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.6/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.6
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.6
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.6 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.6

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.6
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.6/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
