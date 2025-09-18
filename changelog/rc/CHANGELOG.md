# Botanix rc Channel Changelog

All notable changes to the rc release channel will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.0-rc.6] - 2025-09-18


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


**Downloads:** [Release Page](../../releases/1.2.0-rc.6/)


## [1.2.0-rc.5] - 2025-09-02


### Features

* **btc-server:** enfoce maximum tx weight limit during make_tx ([373cbcb](https://github.com/botanix-labs/Macbeth/commit/373cbcb2753d5a07caf98808fdcd13d1bd3ff790))
* **btc-server:** reduce pegout upper bound to more conservative value ([4300425](https://github.com/botanix-labs/Macbeth/commit/430042532d069ff967111c7f2ee505fdd667fe62))

### Bug Fixes

* **btc-server:** enforce max transaction weight limit on make_tx ([#943](https://github.com/botanix-labs/Macbeth/issues/943)) ([74b0e46](https://github.com/botanix-labs/Macbeth/commit/74b0e468a0e689d63926b705ff56148f031e6ad7))
* **btc-server:** fix logic for upper pegout bound ([16ddfcd](https://github.com/botanix-labs/Macbeth/commit/16ddfcdc1af207dd17420b7689b54112a725065e))
* **btc-server:** Removed metrics prefix ([#966](https://github.com/botanix-labs/Macbeth/issues/966)) ([72c381c](https://github.com/botanix-labs/Macbeth/commit/72c381cd84bc3182119af1545be30124adb5ba8e))
* **btc-server:** utxo recovery - script deserialization ([78a7ca8](https://github.com/botanix-labs/Macbeth/commit/78a7ca8396f221c2083289d1e201494e081e6913))
* **test:** fix script_hex in mockbitcoind ([4e0cc44](https://github.com/botanix-labs/Macbeth/commit/4e0cc441a623474873ead83851d4168f68241d15))
* **utxo-recovery:** resolve endian/type conversion issues ([#970](https://github.com/botanix-labs/Macbeth/issues/970)) ([bbf1b54](https://github.com/botanix-labs/Macbeth/commit/bbf1b5401d6c28bc70979d02d267fd3b5ea2e477))

### Code Refactoring

* **btc-server:** more logging around utxo recovery ([e1d6567](https://github.com/botanix-labs/Macbeth/commit/e1d65670d02fe1e7e3b57d6617322b1b49cf2af4))
* **btc-server:** use centralized OutPoint conversion in utxo recovery ([b3a8681](https://github.com/botanix-labs/Macbeth/commit/b3a8681cded505a854d56e799124259e2d6547e9))
* **btc-server:** utxo recovery log ([4dedd4f](https://github.com/botanix-labs/Macbeth/commit/4dedd4f9782d81fda74a2f08e9e6bc24b519da8c))
* **ntp:** remove ntp server logic ([#961](https://github.com/botanix-labs/Macbeth/issues/961)) ([4435919](https://github.com/botanix-labs/Macbeth/commit/4435919fd1c0835cbc8c3927620b5916fa5156cb))

### Documentation

* network deployment and release testing ([#752](https://github.com/botanix-labs/Macbeth/issues/752)) ([a5f8236](https://github.com/botanix-labs/Macbeth/commit/a5f82364661af7e2c9e56711c46e508b991d54a4))
* reth upgrade proposal ([#791](https://github.com/botanix-labs/Macbeth/issues/791)) ([500737c](https://github.com/botanix-labs/Macbeth/commit/500737cfe5e5d0cd2b85727939333e96f2d9260d))

### Tests

* **btc-server:** add integration test for utxo recovery ([09cb88e](https://github.com/botanix-labs/Macbeth/commit/09cb88ece15dab8c9a9c35c5c42e92397b041b6f))
* **btc-server:** extend unit test - test_utxo_recovery_data_conversion ([4c652a3](https://github.com/botanix-labs/Macbeth/commit/4c652a34a3e1b06ce4eb561c3d8aa9f6c47a7671))
* update conflict input test ([#958](https://github.com/botanix-labs/Macbeth/issues/958)) ([cba5b22](https://github.com/botanix-labs/Macbeth/commit/cba5b224bc8033461a6071abf9b854acbb899290))

### Miscellaneous

* **btc-server:** add pegout address to info log ([553cf9b](https://github.com/botanix-labs/Macbeth/commit/553cf9b254e2fb0e8155e44c0a46f0b011e9c0a8))
* **ci:** add tx_weight_limit test to ci ([7db26ab](https://github.com/botanix-labs/Macbeth/commit/7db26abe67fb75f4d67e238c9e1289b4b1cbf265))
* **test:** add utxo_recovery integration test ([7b3c9e5](https://github.com/botanix-labs/Macbeth/commit/7b3c9e52e0c7c69059dd95848e16e8c402bd91f3))
* update codeowners ([#971](https://github.com/botanix-labs/Macbeth/issues/971)) ([0c31906](https://github.com/botanix-labs/Macbeth/commit/0c31906905ed4c64d0e3a54c923435575e75c367))


**Downloads:** [Release Page](../../releases/1.2.0-rc.5/)


## [1.2.0-rc.4] - 2025-08-26


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


**Downloads:** [Release Page](../../releases/1.2.0-rc.4/)


## [1.2.0-rc.3] - 2025-08-18


### Miscellaneous

* **version:** update to correct version ([de7ae70](https://github.com/botanix-labs/Macbeth/commit/de7ae70d338ff49cedc5a9612b76e1a8e72312d6))


**Downloads:** [Release Page](../../releases/1.2.0-rc.3/)


## [1.2.0-rc.2] - 2025-08-18


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


**Downloads:** [Release Page](../../releases/1.2.0-rc.2/)


## [1.2.0-rc.1] - 2025-07-25


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


**Downloads:** [Release Page](../../releases/1.2.0-rc.1/)


## [1.1.4-rc] - 2025-07-01



**Downloads:** [Release Page](../../releases/1.1.4-rc/)


