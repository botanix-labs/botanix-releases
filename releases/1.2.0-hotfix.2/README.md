# Botanix v1.2.0-hotfix.2

**Release Channel:** `hotfix`
**Release Date:** 2025-08-05 15:28:34 UTC
**Git Tag:** `v1.2.0-hotfix.2`
**Git SHA:** `5e17625e72a61663516803fcfa23546ed3ba016a`

## Release Notes


### Continuous Integration

* allow last stable release to persist on public release pags ([cef35fd](https://github.com/botanix-labs/Macbeth/commit/cef35fdff3eca0d1b91f13562abc9914e05e5897))
* explicit tags on readme ([bf4d903](https://github.com/botanix-labs/Macbeth/commit/bf4d903c4f711b6f4dac8a3b8fb76f4eb73d75a4))
* refactor release flow to publish only stable releases to public repo ([b4e4d5b](https://github.com/botanix-labs/Macbeth/commit/b4e4d5b0e1c7e0f0241b000cad264e958c6bcb83))
* refactor release flow to publish only stable releases to public repo ([#896](https://github.com/botanix-labs/Macbeth/issues/896)) ([5e17625](https://github.com/botanix-labs/Macbeth/commit/5e17625e72a61663516803fcfa23546ed3ba016a))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.2/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.2/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.2/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.2/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.2
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-hotfix.2
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.2 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.2

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-hotfix.2
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.2/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
