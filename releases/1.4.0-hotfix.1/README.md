# Botanix v1.4.0-hotfix.1

**Release Channel:** `hotfix`
**Release Date:** 2025-09-29 22:28:32 UTC
**Git Tag:** `v1.4.0-hotfix.1`
**Git SHA:** `fef3c7a349decda993ea72c6b6e5f8a07c8efa77`

## Release Notes


### Features

* **btc-server:** add flag excluded_eth_addresses for coin selection ([7631ed9](https://github.com/botanix-labs/Macbeth/commit/7631ed98b3cddd45dc40b7f9799c3edf921e4859))

### Code Refactoring

* **btc-server:** remove unused error type ([8598590](https://github.com/botanix-labs/Macbeth/commit/8598590ee0ef8e4dcf00c1f845a81d5630e3af92))

### Miscellaneous

* **ci:** bump rust version on clippy checks ([3193291](https://github.com/botanix-labs/Macbeth/commit/3193291717f1e58f9532d46fc14fb0eb8e1605b8))
* **ci:** fix clippy cmdline ([5bdc045](https://github.com/botanix-labs/Macbeth/commit/5bdc04518473e52e7248c67fcc53ec21e0337fa2))
* **ci:** relax result-large-err clippy warning ([3a641ae](https://github.com/botanix-labs/Macbeth/commit/3a641aed5bdd4a6e51c67f4895a4d0c3c9127b46))
* **ci:** use clippy action ([993dfaa](https://github.com/botanix-labs/Macbeth/commit/993dfaabd9593173e1d61ce6514d4aae8dbbc38f))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.4.0-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.4.0-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.4.0-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.4.0-hotfix.1 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.4.0-hotfix.1

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.4.0-hotfix.1
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.4.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
