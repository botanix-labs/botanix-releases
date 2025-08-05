# Botanix v1.2.0

**Release Channel:** `stable`
**Release Date:** 2025-08-05 23:35:06 UTC
**Git Tag:** `v1.2.0`
**Git SHA:** `aec429e498a958291924e695ce811fb441873712`

## Release Notes


### Features

* **abci:** Adjust floor base fee per gas & GPO default values (hotfix) ([#893](https://github.com/botanix-labs/Macbeth/issues/893)) ([9a5e728](https://github.com/botanix-labs/Macbeth/commit/9a5e728825a2bc0d414c5bd23d546972bb04cecc))
* runtime version 3 adjust floor base fee! ([#901](https://github.com/botanix-labs/Macbeth/issues/901)) ([2ad22b0](https://github.com/botanix-labs/Macbeth/commit/2ad22b078fe98427b9ead87b57b683b27ae872ce))

### Bug Fixes

* **clippy:** use keep() ([3633747](https://github.com/botanix-labs/Macbeth/commit/363374788ff0d1bb8da7ad663eb17ac444457451))
* **fee:** add base fee to tx cost ([1bdcf7d](https://github.com/botanix-labs/Macbeth/commit/1bdcf7d1b9db972e994d8d033292ae8624d7dad2))
* **fee:** fn effective tip per gas returns the final fee instead of the priority fee ([#891](https://github.com/botanix-labs/Macbeth/issues/891)) ([38553e5](https://github.com/botanix-labs/Macbeth/commit/38553e59385b99c0aca14ebb14ee5032e6e3cf31))
* **fee:** fn effective_tip_per_gas returns final fee ([50e0a7e](https://github.com/botanix-labs/Macbeth/commit/50e0a7e98c68ebea7432e92d9a3669c97d0ddb61))
* **fee:** use 0 if no basefee ([7ff4f3f](https://github.com/botanix-labs/Macbeth/commit/7ff4f3f7e854b0ad082ecb68d7f2d81f174304f0))
* **priority fee:** remove enforced minimum ([80e7dd9](https://github.com/botanix-labs/Macbeth/commit/80e7dd9fb4427cf409c42e19a607e68d46625d6c))
* **priority fee:** remove enforced minimum ([#883](https://github.com/botanix-labs/Macbeth/issues/883)) ([c399b5b](https://github.com/botanix-labs/Macbeth/commit/c399b5b8fbbf20b8845b82fdfe6ff94bae2e2aa3))

### Code Refactoring

* set floor base fee to 0.0005 GWEI ([fb62d01](https://github.com/botanix-labs/Macbeth/commit/fb62d010b396712e5b816565d488092fb9085efa))

### Continuous Integration

* allow for stable release to persist ([b0cb977](https://github.com/botanix-labs/Macbeth/commit/b0cb977544dbc0f825f579f17499ff1975b2bc4e))
* allow for stable release to persist ([#898](https://github.com/botanix-labs/Macbeth/issues/898)) ([9785f86](https://github.com/botanix-labs/Macbeth/commit/9785f86cc0b99e6a1812aa2df3fb00f3a6e4ca11))
* allow last stable release to persist on public release pags ([cef35fd](https://github.com/botanix-labs/Macbeth/commit/cef35fdff3eca0d1b91f13562abc9914e05e5897))
* explicit tags on readme ([bf4d903](https://github.com/botanix-labs/Macbeth/commit/bf4d903c4f711b6f4dac8a3b8fb76f4eb73d75a4))
* modify release flow  ([#873](https://github.com/botanix-labs/Macbeth/issues/873)) ([566d39a](https://github.com/botanix-labs/Macbeth/commit/566d39ab5e32bfd0d80d37813210a3602ed94567))
* refactor release flow to publish only stable releases to public repo ([b4e4d5b](https://github.com/botanix-labs/Macbeth/commit/b4e4d5b0e1c7e0f0241b000cad264e958c6bcb83))
* refactor release flow to publish only stable releases to public repo ([#896](https://github.com/botanix-labs/Macbeth/issues/896)) ([5e17625](https://github.com/botanix-labs/Macbeth/commit/5e17625e72a61663516803fcfa23546ed3ba016a))

### Miscellaneous

* **docs:** remove network launch docs until upstream merge ([2d2b256](https://github.com/botanix-labs/Macbeth/commit/2d2b25697e0c56a7bc928a3893055e0eff9ef152))
* **release:** back-merge v1.1.13 from main to hotfix ([29fdbf5](https://github.com/botanix-labs/Macbeth/commit/29fdbf51b66c4c516316078c3d02bdd30d90ab99))
* **release:** bump version to 1.1.14-hotfix.1 ([e7cdb3e](https://github.com/botanix-labs/Macbeth/commit/e7cdb3e4b31cf766c41178402c26033e2c987587))
* **release:** bump version to 1.1.14-hotfix.2 ([3567987](https://github.com/botanix-labs/Macbeth/commit/356798790403cbc9457ad97bb1fe90ab283a733e))
* **release:** bump version to 1.1.14-hotfix.2 ([f906a06](https://github.com/botanix-labs/Macbeth/commit/f906a0612ae01c54aafe34a4248a0c9d8933f14c))
* **release:** bump version to 1.1.14-hotfix.3 ([ad6386e](https://github.com/botanix-labs/Macbeth/commit/ad6386e676a9253db28c614ee0a08ffc8e483392))
* **release:** bump version to 1.2.0-hotfix.1 ([a233dff](https://github.com/botanix-labs/Macbeth/commit/a233dff7aeb490ff2342ff66c666dd2d4518dd14))
* **release:** bump version to 1.2.0-hotfix.2 ([85589bf](https://github.com/botanix-labs/Macbeth/commit/85589bf095e471f4474e33d867fe43cec6297c1a))
* **release:** bump version to 1.2.0-hotfix.3 ([f220c38](https://github.com/botanix-labs/Macbeth/commit/f220c382d38eec50d8aedbe176ebc749a4555526))
* **version:** rollback to correct version ([1183147](https://github.com/botanix-labs/Macbeth/commit/1183147a485d2da1be6c5ad1a767ec4a82723e46))


## Downloads

### Binaries

#### Reth Node
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

#### BTC Server
- [Linux x86_64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.2.0/btc-server-x86_64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.2.0/btc-server-x86_64-unknown-linux-gnu.tar.gz.sha256sum))
- [Linux ARM64](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.2.0/btc-server-aarch64-unknown-linux-gnu.tar.gz) ([checksum](https://storage.googleapis.com/botanix-artifact-registry/releases/btc-server/stable/1.2.0/btc-server-aarch64-unknown-linux-gnu.tar.gz.sha256sum))

### Docker Images

#### BTC Server
```bash
docker pull ghcr.io/botanix-labs/botanix-btc-server:1.2.0
docker pull ghcr.io/botanix-labs/botanix-btc-server:stable
```

#### Reth Node
```bash
docker pull ghcr.io/botanix-labs/botanix-reth-node:1.2.0
docker pull ghcr.io/botanix-labs/botanix-reth-node:stable
```

## Verification

### Binary Checksums
```bash
# Download and verify checksums
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-x86_64-unknown-linux-gnu.tar.gz
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
sha256sum -c reth-x86_64-unknown-linux-gnu.tar.gz.sha256sum
```

### Docker Image Verification
```bash
# Inspect image labels
docker inspect ghcr.io/botanix-labs/botanix-btc-server:1.2.0 --format='{{.Config.Labels}}'
```

## Installation

### Quick Start with Docker
```bash
# Run BTC Server
docker run -d --name botanix-btc-server \
  -p 8080:8080 \
  ghcr.io/botanix-labs/botanix-btc-server:1.2.0

# Run Reth Node
docker run -d --name botanix-reth-node \
  -p 30303:30303 -p 8545:8545 \
  ghcr.io/botanix-labs/botanix-reth-node:1.2.0
```

### Binary Installation
```bash
# Download and extract
wget https://storage.googleapis.com/botanix-artifact-registry/releases/reth/stable/1.2.0/reth-x86_64-unknown-linux-gnu.tar.gz
tar -xzf reth-x86_64-unknown-linux-gnu.tar.gz
sudo mv reth /usr/local/bin/
```

## Previous Releases

See [all releases](../../README.md#releases) for version history.
