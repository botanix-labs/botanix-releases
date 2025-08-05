# Botanix v1.2.0-hotfix.1

**Release Channel:** `hotfix`
**Release Date:** 2025-08-05 01:38:13 UTC
**Git Tag:** `v1.2.0-hotfix.1`
**Git SHA:** `9a5e728825a2bc0d414c5bd23d546972bb04cecc`

## Release Notes


### Features

* **abci:** Adjust floor base fee per gas & GPO default values (hotfix) ([#893](https://github.com/botanix-labs/Macbeth/issues/893)) ([9a5e728](https://github.com/botanix-labs/Macbeth/commit/9a5e728825a2bc0d414c5bd23d546972bb04cecc))

### Bug Fixes

* **clippy:** use keep() ([3633747](https://github.com/botanix-labs/Macbeth/commit/363374788ff0d1bb8da7ad663eb17ac444457451))
* **fee:** add base fee to tx cost ([1bdcf7d](https://github.com/botanix-labs/Macbeth/commit/1bdcf7d1b9db972e994d8d033292ae8624d7dad2))
* **fee:** fn effective tip per gas returns the final fee instead of the priority fee ([#891](https://github.com/botanix-labs/Macbeth/issues/891)) ([38553e5](https://github.com/botanix-labs/Macbeth/commit/38553e59385b99c0aca14ebb14ee5032e6e3cf31))
* **fee:** fn effective_tip_per_gas returns final fee ([50e0a7e](https://github.com/botanix-labs/Macbeth/commit/50e0a7e98c68ebea7432e92d9a3669c97d0ddb61))
* **fee:** use 0 if no basefee ([7ff4f3f](https://github.com/botanix-labs/Macbeth/commit/7ff4f3f7e854b0ad082ecb68d7f2d81f174304f0))

### Miscellaneous

* **docs:** remove network launch docs until upstream merge ([2d2b256](https://github.com/botanix-labs/Macbeth/commit/2d2b25697e0c56a7bc928a3893055e0eff9ef152))
* **release:** bump version to 1.1.14-hotfix.3 ([ad6386e](https://github.com/botanix-labs/Macbeth/commit/ad6386e676a9253db28c614ee0a08ffc8e483392))
* **version:** rollback to correct version ([1183147](https://github.com/botanix-labs/Macbeth/commit/1183147a485d2da1be6c5ad1a767ec4a82723e46))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.1/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/hotfix/1.2.0-hotfix.1/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-btc-server:hotfix
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-hotfix.1
docker pull ghcr.io/botanix-labs/botanix-reth-node:hotfix
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.1 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-hotfix.1

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-hotfix.1
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/hotfix/1.2.0-hotfix.1/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
