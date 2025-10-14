# Botanix v1.2.0-rc.10

**Release Channel:** `rc`
**Release Date:** 2025-10-14 16:41:29 UTC
**Git Tag:** `v1.2.0-rc.10`
**Git SHA:** `7e3668cd9edb7e244a6db4978f7ac13944f27a0c`

## Release Notes


### Features

* **btc-utils:** Implement  functionality ([#986](https://github.com/botanix-labs/Macbeth/issues/986)) ([15b5971](https://github.com/botanix-labs/Macbeth/commit/15b59712e01a37a8bb4ea56084d744e7363d2ee2))
* **reth:** support dns hostnames in config ([#1007](https://github.com/botanix-labs/Macbeth/issues/1007)) ([4cee490](https://github.com/botanix-labs/Macbeth/commit/4cee49046cce034399ad712c6cc3ae1d624c5b5e))

### Miscellaneous

* **deps:** bump actions/setup-node from 4 to 5 ([#977](https://github.com/botanix-labs/Macbeth/issues/977)) ([b342af0](https://github.com/botanix-labs/Macbeth/commit/b342af026324e4dfcfd4e179b12375c463cbc624))
* **deps:** bump clechasseur/rs-clippy-check from 4.0.5 to 5.0.1 ([9f32ea9](https://github.com/botanix-labs/Macbeth/commit/9f32ea9329238d1a8aebbbf71de81f641b5b23e8))
* **deps:** bump clechasseur/rs-fmt-check from 2.0.11 to 3.0.0 ([bfaa89c](https://github.com/botanix-labs/Macbeth/commit/bfaa89cd7f1a15341604741c5c48c7684f036799))
* **deps:** bump cycjimmy/semantic-release-action from 4 to 5 ([508e56f](https://github.com/botanix-labs/Macbeth/commit/508e56f9076ae5912d9366c38f382f919f4784cf))
* **deps:** bump google-github-actions/auth from 2 to 3 ([#1006](https://github.com/botanix-labs/Macbeth/issues/1006)) ([ff7435c](https://github.com/botanix-labs/Macbeth/commit/ff7435ca047ae6e4ab04c839d7eaddfb233660ba))
* **deps:** bump google-github-actions/setup-gcloud from 2 to 3 ([adfdfe0](https://github.com/botanix-labs/Macbeth/commit/adfdfe03e64f55f3e8679ec62bf9e0beacc4a9df))
* **deps:** bump sigstore/cosign-installer from 3.9.2 to 3.10.0 ([#1005](https://github.com/botanix-labs/Macbeth/issues/1005)) ([9b94808](https://github.com/botanix-labs/Macbeth/commit/9b948089343c3ba54abdd1f0c155ef66f6a72d25))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.10/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.10/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.10/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.10/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.10
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.10
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.10 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.10

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.10
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.10/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
