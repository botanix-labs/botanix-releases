# Botanix v1.1.14-hotfix.3

**Release Channel:** `hotfix`
**Release Date:** 2025-08-04 17:38:57 UTC
**Git Tag:** `v1.1.14-hotfix.3`
**Git SHA:** `b37b1d614272b8cf6fa7e94a6a8f3babcba6f74b`

## Release Notes


### Miscellaneous

* **docs:** remove network launch docs until upstream merge ([b37b1d6](https://github.com/botanix-labs/Macbeth/commit/b37b1d614272b8cf6fa7e94a6a8f3babcba6f74b))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.1.14-hotfix.3/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.1.14-hotfix.3/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.1.14-hotfix.3/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.1.14-hotfix.3/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.1.14-hotfix.3
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.1.14-hotfix.3
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.1.14-hotfix.3 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.1.14-hotfix.3

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.1.14-hotfix.3
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.1.14-hotfix.3/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
