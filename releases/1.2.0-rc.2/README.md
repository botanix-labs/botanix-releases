# Botanix v1.2.0-rc.2

**Release Channel:** `rc`
**Release Date:** 2025-08-18 16:45:28 UTC
**Git Tag:** `v1.2.0-rc.2`
**Git SHA:** `b3b29e7c3d99d7cfa7b3e12c5cce6e8fa492d268`

## Release Notes


### Features

*  command to rollback blocks ([#908](https://github.com/botanix-labs/Macbeth/issues/908)) ([1a35b78](https://github.com/botanix-labs/Macbeth/commit/1a35b78bcaf54c5033f563d7fdb902dc45ffdd18))
* **abci:** Adjust floor base fee per gas & GPO default values ([#892](https://github.com/botanix-labs/Macbeth/issues/892)) ([1343224](https://github.com/botanix-labs/Macbeth/commit/134322426e27fcd14819ff2155cbd28f5e56471b))
* **authority:** increase epoch length to 100 ([#904](https://github.com/botanix-labs/Macbeth/issues/904)) ([4f71ef1](https://github.com/botanix-labs/Macbeth/commit/4f71ef1fbf2e6af0b60ab96b4cdee1c84792ea12))
* **btc-server:** add jwt validation to recover_missing_utxos ([d6afae5](https://github.com/botanix-labs/Macbeth/commit/d6afae5eeb88e2bb0020de23b3b52c5d0eb8954b))
* **btc-server:** add recover_missing_utxos method to BtcServerExtendedApi ([096ed87](https://github.com/botanix-labs/Macbeth/commit/096ed8715f40d63a6647ba7c4f43c375539d2fce))
* **btc-server:** Added comprehensive utxo metrics ([826ed24](https://github.com/botanix-labs/Macbeth/commit/826ed24937e2520a7929643df4da4183d0fda2b0))
* **btc-server:** Added comprehensive utxo metrics ([#882](https://github.com/botanix-labs/Macbeth/issues/882)) ([2db8951](https://github.com/botanix-labs/Macbeth/commit/2db89515d8053e1a0b12b18c46d2ad8fff786287))
* **btc-server:** recover_missing_utxo grpc endpoint ([c7684d0](https://github.com/botanix-labs/Macbeth/commit/c7684d0180d600eb232de92d9b3d04bb1aed1641))
* **btc-server:** RecoverMissingUtxos grpc endpoint ([#886](https://github.com/botanix-labs/Macbeth/issues/886)) ([e77e2a2](https://github.com/botanix-labs/Macbeth/commit/e77e2a2d404cf9679febd8e32adfe7172a29e981))
* **btc-server:** signal RBF in pegout transaction ([#923](https://github.com/botanix-labs/Macbeth/issues/923)) ([666ed87](https://github.com/botanix-labs/Macbeth/commit/666ed87a8763cbb7bc3e6d23a16b888b30498d84))
* **btc-server:** update merkle root and flush when recovering missing utxos ([d5c043f](https://github.com/botanix-labs/Macbeth/commit/d5c043f7fde7123e3dc9a9ceb6dad5c02383c732))
* **flag:** add is_devnet flag ([#879](https://github.com/botanix-labs/Macbeth/issues/879)) ([54f71f3](https://github.com/botanix-labs/Macbeth/commit/54f71f3eea0a9b033e79672a370ebf934585f5bc))
* **pegouts:** remove finalized pegout id from pending pegouts ([#880](https://github.com/botanix-labs/Macbeth/issues/880)) ([c106098](https://github.com/botanix-labs/Macbeth/commit/c10609833bcaf5393ad97bb2350e32174d4f44a0))
* **reth:** add missing utxos on reth startup ([#911](https://github.com/botanix-labs/Macbeth/issues/911)) ([a9605cb](https://github.com/botanix-labs/Macbeth/commit/a9605cb2bf9bccd914b1e5fece84329469e9079a))
* **reth:** Added botanix-configs and extended botanix-cli-args ([#881](https://github.com/botanix-labs/Macbeth/issues/881)) ([2102d8d](https://github.com/botanix-labs/Macbeth/commit/2102d8d7641882a217c972f18e3b381f59fb2295))
* **wallet:** use SIGHASH_DEFAULT instead of SIGHASH_ALL in pegout tx ([#878](https://github.com/botanix-labs/Macbeth/issues/878)) ([b52711a](https://github.com/botanix-labs/Macbeth/commit/b52711affe7bd37bf32b652b16dddc9f143667f4))

### Bug Fixes

* **btc-server:** ensure metrics server shuts down when btc-server shu… ([#922](https://github.com/botanix-labs/Macbeth/issues/922)) ([ffd9486](https://github.com/botanix-labs/Macbeth/commit/ffd948606d7d863ff98c368e29d6b733e0b1cd2b))
* **reth:** Updated all networking acc. to latest reth improvements ([#885](https://github.com/botanix-labs/Macbeth/issues/885)) ([fa4dda0](https://github.com/botanix-labs/Macbeth/commit/fa4dda0162dbcc6a109b6e30cbedd2b7f85634b2))
* **test:** reduce base fee ([#929](https://github.com/botanix-labs/Macbeth/issues/929)) ([c8b76fa](https://github.com/botanix-labs/Macbeth/commit/c8b76fa210286b44583c2736f6f3976ad6f99e95))
* **test:** rpc int test on develop times out ([#912](https://github.com/botanix-labs/Macbeth/issues/912)) ([b7900a0](https://github.com/botanix-labs/Macbeth/commit/b7900a04fe56e9d884189c8eb0f07318d2b77e5c))
* **wallet:** duplicate input bug (flakey conflicting_inputs test) ([#874](https://github.com/botanix-labs/Macbeth/issues/874)) ([7bc32f9](https://github.com/botanix-labs/Macbeth/commit/7bc32f9f32588212a91609256ed315b3f7e92004))

### Code Refactoring

* ** btc-server:** handle error properly instead of unwrap ([f774f54](https://github.com/botanix-labs/Macbeth/commit/f774f54c1ba20f6744db593b986b69aa0f124e2d))
* **btc-server:** cleanup from hotfix for recovering missing change outputs ([#915](https://github.com/botanix-labs/Macbeth/issues/915)) ([40ba4c1](https://github.com/botanix-labs/Macbeth/commit/40ba4c1be514ed5e7537d8a60b5f0f04bec21fc8))
* **btc-server:** code readability ([0f1083f](https://github.com/botanix-labs/Macbeth/commit/0f1083f77506a6713da9b0207205f04c51c7ea6e))
* consolidate btc server client ([#900](https://github.com/botanix-labs/Macbeth/issues/900)) ([d6c2067](https://github.com/botanix-labs/Macbeth/commit/d6c2067b058dd847cdc9ad686a2da62440ec20cb))

### Tests

* **test-suite:** check port availability when starting up test nodes ([#924](https://github.com/botanix-labs/Macbeth/issues/924)) ([fa9e7a6](https://github.com/botanix-labs/Macbeth/commit/fa9e7a6bf9697e7e9cde57960c9c1f17336c6737))

### Miscellaneous

* adding dariusparvin to codeowners ([#875](https://github.com/botanix-labs/Macbeth/issues/875)) ([7c44257](https://github.com/botanix-labs/Macbeth/commit/7c442578306866b806fbc413809fbf6d1cfd2f65))
* **btc-server:** add github issue link to handling of spent input ([#925](https://github.com/botanix-labs/Macbeth/issues/925)) ([7de97be](https://github.com/botanix-labs/Macbeth/commit/7de97bed358929eb551d39d25bd42e6f14dbc2de))
* **btc-server:** update btc_server.bin ([efe3fb0](https://github.com/botanix-labs/Macbeth/commit/efe3fb05ab5c365344998620d269d61d02f1ba42))
* cherry pick hotfix effective tip per gas ([#894](https://github.com/botanix-labs/Macbeth/issues/894)) ([c4371ae](https://github.com/botanix-labs/Macbeth/commit/c4371ae9e0a75ab7b1c93085f8c6f14285b579c2))
* cherry pick release flow ([#897](https://github.com/botanix-labs/Macbeth/issues/897)) ([951de4a](https://github.com/botanix-labs/Macbeth/commit/951de4addd165cee047409e839cc5a4f28bea168))
* cherry-pick adjust base fee ([#902](https://github.com/botanix-labs/Macbeth/issues/902)) ([81ea867](https://github.com/botanix-labs/Macbeth/commit/81ea867e51708c2f859204ba41f8f52e263d4741))
* **deps:** bump actions/download-artifact from 4 to 5 ([#918](https://github.com/botanix-labs/Macbeth/issues/918)) ([1b89c41](https://github.com/botanix-labs/Macbeth/commit/1b89c411fed7b399c9e7abefe5b3c46fb50eec6d))
* **deps:** bump clechasseur/rs-clippy-check from 4.0.4 to 4.0.5 ([#889](https://github.com/botanix-labs/Macbeth/issues/889)) ([7563c31](https://github.com/botanix-labs/Macbeth/commit/7563c31af8d97a041159bc8551f9a5697922a406))
* **deps:** bump clechasseur/rs-fmt-check from 2.0.10 to 2.0.11 ([40cfcb7](https://github.com/botanix-labs/Macbeth/commit/40cfcb726c1e9d4d575cc954550484fcb67ff9ab))
* **deps:** bump clechasseur/rs-fmt-check from 2.0.10 to 2.0.11 ([#890](https://github.com/botanix-labs/Macbeth/issues/890)) ([267f3a2](https://github.com/botanix-labs/Macbeth/commit/267f3a2ca5254d9c3cb6a7a105506c9b384e8cc8))
* **deps:** bump sigstore/cosign-installer from 3.9.1 to 3.9.2 ([#888](https://github.com/botanix-labs/Macbeth/issues/888)) ([9f225ce](https://github.com/botanix-labs/Macbeth/commit/9f225ce06d43fbc5bd7988f2686d2122b9f9d7cb))
* merge develop into rc ([#927](https://github.com/botanix-labs/Macbeth/issues/927)) ([b3b29e7](https://github.com/botanix-labs/Macbeth/commit/b3b29e7c3d99d7cfa7b3e12c5cce6e8fa492d268))
* **version:** update to correct version ([#907](https://github.com/botanix-labs/Macbeth/issues/907)) ([91909f9](https://github.com/botanix-labs/Macbeth/commit/91909f962953cd4ee5f456f7ffdf22b6a99f07d0))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.2/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.2/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.2/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.2/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.2
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.2
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.2 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.2

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.2
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.2/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
