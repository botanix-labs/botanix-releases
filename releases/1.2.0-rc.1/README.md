# Botanix v1.2.0-rc.1

**Release Channel:** `rc`
**Release Date:** 2025-07-25 18:15:39 UTC
**Git Tag:** `v1.2.0-rc.1`
**Git SHA:** `388333f37d99632beca216816edfe2d4dc1a2a96`

## Release Notes


### Features

* **ABCI/storage:** Insert pegins & pegouts into database on finalizing commit ([#756](https://github.com/botanix-labs/Macbeth/issues/756)) ([c3f9609](https://github.com/botanix-labs/Macbeth/commit/c3f960956d659e12708fa04420184c7888395a29))
* **btc-server:** Decoupled btc-server from old alloy deps and added … ([#827](https://github.com/botanix-labs/Macbeth/issues/827)) ([c550608](https://github.com/botanix-labs/Macbeth/commit/c550608cabaedc92e9c732f2e6df855147bc0f99))
* **btc-server:** pegout tx fee and coin selection improvements ([#871](https://github.com/botanix-labs/Macbeth/issues/871)) ([388333f](https://github.com/botanix-labs/Macbeth/commit/388333f37d99632beca216816edfe2d4dc1a2a96))
* **btc-server:** reworked all btc-server metrics ([#792](https://github.com/botanix-labs/Macbeth/issues/792)) ([f28c6b3](https://github.com/botanix-labs/Macbeth/commit/f28c6b3fb0bedffd3c95c9f275dd1269b7debca8))
* **ndd:** integrate NDD changes in ABCI interface ([4649990](https://github.com/botanix-labs/Macbeth/commit/464999027abb1d0dae960139ba15510eb609a666))
* **ndd:** make NDD deserialization forward-compatible ([6155db9](https://github.com/botanix-labs/Macbeth/commit/6155db9a95ea7ec05b3b7455360cd15cca82d375))
* **parser:** moved prost_parser.rs file from botanix consensus into reth_data_parser crate ([#815](https://github.com/botanix-labs/Macbeth/issues/815)) ([25a8145](https://github.com/botanix-labs/Macbeth/commit/25a814596853493dd90ba6f4bd6e74bb0d5974c3))
* **pegouts:** check pending pegout not finalized before storing ([#837](https://github.com/botanix-labs/Macbeth/issues/837)) ([dab889e](https://github.com/botanix-labs/Macbeth/commit/dab889e659cc2d64ca10bfb4ee2eca9536a8b40f))
* **reth:** Added botanix prefix to owned crates ([#826](https://github.com/botanix-labs/Macbeth/issues/826)) ([223f4aa](https://github.com/botanix-labs/Macbeth/commit/223f4aadcbad0d5dd2bb5c85d91253b4f30c8c68))
* **reth:** Added botanix-authority-edh and botanix-authority-peg crates ([#838](https://github.com/botanix-labs/Macbeth/issues/838)) ([8e697f4](https://github.com/botanix-labs/Macbeth/commit/8e697f4ac4ae77ec4444baac4893a747ed4acb1b))
* **reth:** Added botanix-cli-args crate ([#867](https://github.com/botanix-labs/Macbeth/issues/867)) ([b44144a](https://github.com/botanix-labs/Macbeth/commit/b44144a0d37a8bae6d9d0237c0071f10924e3df7))
* **reth:** Added botanix-cli-parsers crate ([#865](https://github.com/botanix-labs/Macbeth/issues/865)) ([c8069f0](https://github.com/botanix-labs/Macbeth/commit/c8069f0a3e87f4d9a5dde9118388887807a732e6))
* **reth:** added healthcheck checks with metrics update ([#811](https://github.com/botanix-labs/Macbeth/issues/811)) ([dee1123](https://github.com/botanix-labs/Macbeth/commit/dee1123fff4e746dcf77d46062d6c49d312b5d68))
* **reth:** Extracted functionalities out of authority consensus into new crates ([#836](https://github.com/botanix-labs/Macbeth/issues/836)) ([b6e945e](https://github.com/botanix-labs/Macbeth/commit/b6e945e1ee596ccab830f913e8d5d144b8425c98))
* **reth:** Split up monolith rpc server into botanix-specific logic … ([#839](https://github.com/botanix-labs/Macbeth/issues/839)) ([9d874b4](https://github.com/botanix-labs/Macbeth/commit/9d874b4ca11e7f7a29218bd1003a6dec606907f5))

### Bug Fixes

* **abci:** panic on check_tx ([#757](https://github.com/botanix-labs/Macbeth/issues/757)) ([c51d4b2](https://github.com/botanix-labs/Macbeth/commit/c51d4b2a6a20044c38304ebfa691c8b42311a40c))
* **authority:** non-deterministic bitcoin checkpoint validation ([#694](https://github.com/botanix-labs/Macbeth/issues/694)) ([6197458](https://github.com/botanix-labs/Macbeth/commit/61974587d29bd7e63d9c2f7862c8831719649614))
* **btc-server:** fixed protofile tags indexing ([#810](https://github.com/botanix-labs/Macbeth/issues/810)) ([7801381](https://github.com/botanix-labs/Macbeth/commit/7801381872ed8f9980182a686a94606097cb39f6))
* **docs:** Run fmt on md and toml files ([#812](https://github.com/botanix-labs/Macbeth/issues/812)) ([9dd4cfa](https://github.com/botanix-labs/Macbeth/commit/9dd4cfa1562c360a6f5567497054307167bb09d1))
* **poa:** empty payload panic logs ([ab8b1cf](https://github.com/botanix-labs/Macbeth/commit/ab8b1cf4659a6d6373046776f87bc5a1b434c8f4))
* **storage:**  methods aren't persisting data ([#785](https://github.com/botanix-labs/Macbeth/issues/785)) ([8afe8d7](https://github.com/botanix-labs/Macbeth/commit/8afe8d794effa46d42da4cad8401511337cd29a6))

### Code Refactoring

* **abci:** track hash of block to be finalized before committing ([54e3608](https://github.com/botanix-labs/Macbeth/commit/54e360890d2e04a833e473b75d970fa0c6249370))
* **authority:** bring back NDD to authority crate ([#856](https://github.com/botanix-labs/Macbeth/issues/856)) ([2d9f5c9](https://github.com/botanix-labs/Macbeth/commit/2d9f5c9a9cb45f14f28fe9c8e0fe0355376b5100))
* split botanix and reth databases ([#835](https://github.com/botanix-labs/Macbeth/issues/835)) ([bd859ae](https://github.com/botanix-labs/Macbeth/commit/bd859ae9ac4e45235ddafc2f93dbf50e69328641))

### Documentation

* developer git flow ([#768](https://github.com/botanix-labs/Macbeth/issues/768)) ([4147b6b](https://github.com/botanix-labs/Macbeth/commit/4147b6bfbefd2642c51eadef5937d3d734aa7797))
* release strategy ([#771](https://github.com/botanix-labs/Macbeth/issues/771)) ([b6dd108](https://github.com/botanix-labs/Macbeth/commit/b6dd108cc1c470b61c0830052cfef763a7be7a80))

### Tests

* **ndd:** update unit tests to reflect changes ([8f7588b](https://github.com/botanix-labs/Macbeth/commit/8f7588bf914e1223d26db4083c80257c18a93ec3))
* **pegins:** Fix pegin v1 test ([#762](https://github.com/botanix-labs/Macbeth/issues/762)) ([e7ea12f](https://github.com/botanix-labs/Macbeth/commit/e7ea12f3f5cb695114061afed708ffe0c28d0488))
* **signing:** Fix dust limit error in signing flow test ([#766](https://github.com/botanix-labs/Macbeth/issues/766)) ([c1c4bdf](https://github.com/botanix-labs/Macbeth/commit/c1c4bdf5f00e7b7822f4b166fdbd2f26e778fcfa))

### Build System

* adjust reth log filter in  ([#775](https://github.com/botanix-labs/Macbeth/issues/775)) ([1baef9c](https://github.com/botanix-labs/Macbeth/commit/1baef9c32837e9ada9f1701cba3d557724835fe9))
* autoload bitcoin wallet for local setup ([#774](https://github.com/botanix-labs/Macbeth/issues/774)) ([75bd82d](https://github.com/botanix-labs/Macbeth/commit/75bd82d5e64c8f7f1bdd15f3455119e0bbe0e76c))
* non-strict PR checks with coderabbit ([#784](https://github.com/botanix-labs/Macbeth/issues/784)) ([125ef81](https://github.com/botanix-labs/Macbeth/commit/125ef81ec5dd55800a681c5955041e14894be191))
* rework local network setup with docker ([#765](https://github.com/botanix-labs/Macbeth/issues/765)) ([43953db](https://github.com/botanix-labs/Macbeth/commit/43953dba64c2841799422e576b866ae0862f6a86)), closes [#734](https://github.com/botanix-labs/Macbeth/issues/734)

### Continuous Integration

* added PR template ([#782](https://github.com/botanix-labs/Macbeth/issues/782)) ([997c755](https://github.com/botanix-labs/Macbeth/commit/997c7559ffb35b9994e96e0b0536fbfda2fa2e19))
* check PR assignees and linked issues ([#781](https://github.com/botanix-labs/Macbeth/issues/781)) ([df5d651](https://github.com/botanix-labs/Macbeth/commit/df5d6510dab26aa95c2f7de931565333cea2fbb4))
* check signed commits ([#780](https://github.com/botanix-labs/Macbeth/issues/780)) ([c260cc9](https://github.com/botanix-labs/Macbeth/commit/c260cc9b6f3347cbb8d4d6340ee1cb1322ac727d))
* make coderabbit review all PRs ([#797](https://github.com/botanix-labs/Macbeth/issues/797)) ([a8ce74e](https://github.com/botanix-labs/Macbeth/commit/a8ce74e66d757a6da14f1505b016cb1d511c1e92))
* PR checks ([#778](https://github.com/botanix-labs/Macbeth/issues/778)) ([23f76c3](https://github.com/botanix-labs/Macbeth/commit/23f76c3798032e0475257faf27a3fb5d8008b2f0))
* semantic release flow ([#749](https://github.com/botanix-labs/Macbeth/issues/749)) ([09d9cef](https://github.com/botanix-labs/Macbeth/commit/09d9cef45e451d4b9f7f1f3b0c13b174c8e8dec3))
* update base branches ([#779](https://github.com/botanix-labs/Macbeth/issues/779)) ([440167a](https://github.com/botanix-labs/Macbeth/commit/440167a73cab22fe6237ee5016fa0223825c144e))
* verbose clippy and fmt checks ([#783](https://github.com/botanix-labs/Macbeth/issues/783)) ([41109f3](https://github.com/botanix-labs/Macbeth/commit/41109f3af4ebfc8a32b9db9189001fe0fe007452))
* **workflows:** add dev branch to workflows ([740267a](https://github.com/botanix-labs/Macbeth/commit/740267ac2461328f248cb0da425b4ac8656cec6b))

### Miscellaneous

* **abci:** missing response logging ([#758](https://github.com/botanix-labs/Macbeth/issues/758)) ([9531e3b](https://github.com/botanix-labs/Macbeth/commit/9531e3b6e4294aee389dbabb10930e5b6d786294))
* **codeowners:** update codeowners ([#760](https://github.com/botanix-labs/Macbeth/issues/760)) ([7947ffd](https://github.com/botanix-labs/Macbeth/commit/7947ffd7adfdc2c388ca8aab6646f30338e90847))
* **deps:** bump clechasseur/rs-clippy-check from 4.0.2 to 4.0.3 ([#789](https://github.com/botanix-labs/Macbeth/issues/789)) ([36ad5aa](https://github.com/botanix-labs/Macbeth/commit/36ad5aa1257452569415a0cb3dbee155c2e33c3f))
* **deps:** bump clechasseur/rs-clippy-check from 4.0.3 to 4.0.4 ([#818](https://github.com/botanix-labs/Macbeth/issues/818)) ([13c5ad2](https://github.com/botanix-labs/Macbeth/commit/13c5ad260858df61d4744bb26c0cdf762fa197d0))
* **deps:** bump clechasseur/rs-fmt-check from 2.0.8 to 2.0.9 ([#788](https://github.com/botanix-labs/Macbeth/issues/788)) ([95bc58d](https://github.com/botanix-labs/Macbeth/commit/95bc58d6e4048c634f0e8281e2b21d34e004e6f3))
* **deps:** bump clechasseur/rs-fmt-check from 2.0.9 to 2.0.10 ([#819](https://github.com/botanix-labs/Macbeth/issues/819)) ([e264366](https://github.com/botanix-labs/Macbeth/commit/e264366fee87baede921fc5f8f258eefeb2e2548))
* **deps:** bump sigstore/cosign-installer from 3.8.2 to 3.9.0 ([#790](https://github.com/botanix-labs/Macbeth/issues/790)) ([a33ea02](https://github.com/botanix-labs/Macbeth/commit/a33ea0271ff17a2b47eae09226619a0f07eb35ce))
* **deps:** bump sigstore/cosign-installer from 3.9.0 to 3.9.1 ([#813](https://github.com/botanix-labs/Macbeth/issues/813)) ([bfab083](https://github.com/botanix-labs/Macbeth/commit/bfab083906ad0a9833ce0e0718c1fe073c04429c))
* log poa command errors ([ab6dc8f](https://github.com/botanix-labs/Macbeth/commit/ab6dc8f09db561bb27b230654ee72bdf21826f93))
* merge main into develop ([#859](https://github.com/botanix-labs/Macbeth/issues/859)) ([fe01935](https://github.com/botanix-labs/Macbeth/commit/fe01935427aec3f7edbb903fbffac4c0ad92f857))
* **release:** back merge main to develop ([#807](https://github.com/botanix-labs/Macbeth/issues/807)) ([bc9558e](https://github.com/botanix-labs/Macbeth/commit/bc9558e0c36ac9e2c40089fe4deeacc62fafd7a4))
* **release:** back-merge v1.1.13 from main to develop ([#870](https://github.com/botanix-labs/Macbeth/issues/870)) ([d00f072](https://github.com/botanix-labs/Macbeth/commit/d00f07283d2cf2a96deba52e1a574143a622dcb6))
* reth cli reads envs ([#737](https://github.com/botanix-labs/Macbeth/issues/737)) ([903220d](https://github.com/botanix-labs/Macbeth/commit/903220dd90b668ef8adbf6db2d8c9c8df034a369)), closes [#734](https://github.com/botanix-labs/Macbeth/issues/734)


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.1/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.1/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.1/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/rc/1.2.0-rc.1/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.1
docker pull ghcr.io/botanix-labs/botanix-btc-server:rc
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.1
docker pull ghcr.io/botanix-labs/botanix-reth-node:rc
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.1 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0-rc.1

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0-rc.1
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/rc/1.2.0-rc.1/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
