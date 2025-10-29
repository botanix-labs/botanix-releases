# Botanix hotfix Channel Changelog

All notable changes to the hotfix release channel will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.5.2-hotfix.1] - 2025-10-29


### Bug Fixes

* **pegouts:** remove all finalized pegouts from pending pegouts list ([0d8e12d](https://github.com/botanix-labs/Macbeth/commit/0d8e12dbc2fc75839bf6489f79f80ad6c3a203ab))
* **pegouts:** remove all finalized pegouts from pending pegouts list ([#1019](https://github.com/botanix-labs/Macbeth/issues/1019)) ([53394e9](https://github.com/botanix-labs/Macbeth/commit/53394e93ae6dc3e9f8ba376f473d483b5fb9c7ca))

### Tests

* **outputs:** add test to validate finalized pegouts are removed from pending pegouts ([70bec97](https://github.com/botanix-labs/Macbeth/commit/70bec97a7fae2676bddac9476d43c13bc3794346))

### Miscellaneous

* **release:** back-merge v1.5.1 from main to hotfix ([bb55593](https://github.com/botanix-labs/Macbeth/commit/bb555939c84538c688eba862002f258ebbaa06da))


**Downloads:** [Release Page](../../releases/1.5.2-hotfix.1/)


## [1.5.1-hotfix.1] - 2025-10-16


### Miscellaneous

* dummy change to force build ([5189e28](https://github.com/botanix-labs/Macbeth/commit/5189e280b04d2ea0833c8ee29bc25d03ead2cbf9))
* **release:** back-merge v1.5.0 from main to hotfix ([402699a](https://github.com/botanix-labs/Macbeth/commit/402699ac7d4b051171ed456bc1a75c82802ec5d0))


**Downloads:** [Release Page](../../releases/1.5.1-hotfix.1/)


## [1.4.0-hotfix.2] - 2025-10-01


### Features

* **btc-server:** add jwt validation to recover_missing_utxos ([2745e60](https://github.com/botanix-labs/Macbeth/commit/2745e607788ce37067c989c8d2bd1dd98ddc31d9))
* **btc-server:** add recover_missing_utxos method to BtcServerExtendedApi ([4364675](https://github.com/botanix-labs/Macbeth/commit/43646754e45263613a80952e36a641e29a94e201))
* **btc-server:** recover_missing_utxo grpc endpoint ([a479c28](https://github.com/botanix-labs/Macbeth/commit/a479c28494fa08cffaff3b878343845e0bc35e22))
* **btc-server:** update merkle root and flush when recovering missing utxos ([2881f67](https://github.com/botanix-labs/Macbeth/commit/2881f672b81234d0b156320cd5b7e1253d39b1a9))
* **reth:** add missing utxos on reth startup ([a5f0040](https://github.com/botanix-labs/Macbeth/commit/a5f004056f8a6cda5df9dd79037baf54ac2aaecb))
* **reth:** add optional argument for utxo recovery file ([cf62419](https://github.com/botanix-labs/Macbeth/commit/cf6241984c2d3e9a71535f648a20e9de52e6766e))

### Bug Fixes

* **btc-server:** utxo recovery - script deserialization ([bde5277](https://github.com/botanix-labs/Macbeth/commit/bde5277a3789edc97a388d5e1f93ab0b20444cf8))
* **test:** fix script_hex in mockbitcoind ([8a837b3](https://github.com/botanix-labs/Macbeth/commit/8a837b3695e3a4011062bbf926f0d67795aac232))

### Code Refactoring

* ** btc-server:** handle error properly instead of unwrap ([8128764](https://github.com/botanix-labs/Macbeth/commit/8128764d324ebe606f0b67f464374f81cae273ee))
* **authority:** utxo recovery file json to use camelCase ([1f221f1](https://github.com/botanix-labs/Macbeth/commit/1f221f1092151a811ee961fc88953de73e5a80b5))
* **btc-server:** code readability ([6a534db](https://github.com/botanix-labs/Macbeth/commit/6a534db66423fe7a48e568443176e959d7cf4905))
* **btc-server:** more logging around utxo recovery ([ed4e3a6](https://github.com/botanix-labs/Macbeth/commit/ed4e3a6a09348df492f7206cc2d998c3b82771c2))
* **btc-server:** move utxo recovery file reading logic to btc-server ([ee6a0b6](https://github.com/botanix-labs/Macbeth/commit/ee6a0b6e06363a5a0e51077631f7cce59b7e8109))
* **btc-server:** use centralized OutPoint conversion in utxo recovery ([9e72e2a](https://github.com/botanix-labs/Macbeth/commit/9e72e2aa8ede19183161a2d250f4f03b4e2bd6ba))
* **btc-server:** use TryFrom for reading utxo recovery file ([8e5059f](https://github.com/botanix-labs/Macbeth/commit/8e5059f50e898b9e3a09e3c650b0eba07ff893b0))
* **btc-server:** utxo recovery log ([b4af328](https://github.com/botanix-labs/Macbeth/commit/b4af3282ec26db554b4c747a4c5fd54e85af25cd))
* fixing merge conflicts when moving to hotfix branch ([f9860ab](https://github.com/botanix-labs/Macbeth/commit/f9860abb71921161388ac84029116b33f26a3daa))

### Tests

* **authority:** add unit tests for adding utxos on startup ([db773e4](https://github.com/botanix-labs/Macbeth/commit/db773e4f0ee715778fa9e3053db3a82c6461b405))
* **authority:** update utxo recovery unit test with real examples ([41b24a8](https://github.com/botanix-labs/Macbeth/commit/41b24a89f8995b08000b0bc6e287296711b89d41))
* **btc-server:** add integration test for utxo recovery ([1fe5855](https://github.com/botanix-labs/Macbeth/commit/1fe5855765156dc40bf8339d1526ff00443d15d7))
* **btc-server:** extend unit test - test_utxo_recovery_data_conversion ([74c4b83](https://github.com/botanix-labs/Macbeth/commit/74c4b838c1213e8a0ecd13de336b20215712a617))

### Miscellaneous

* **ci:** robust prepare binary for upload ([ab1cc6b](https://github.com/botanix-labs/Macbeth/commit/ab1cc6b8b494dd0297ce02406c95d72436722d2a))
* **ci:** switch build binaries to k8 runners ([8ca0ba2](https://github.com/botanix-labs/Macbeth/commit/8ca0ba2de95c2042fa57ecb812dfde193124484b))
* **test:** add utxo_recovery integration test ([48ceb48](https://github.com/botanix-labs/Macbeth/commit/48ceb4846bc1d33f00d5fb87dcd76e89affbaa9a))


**Downloads:** [Release Page](../../releases/1.4.0-hotfix.2/)


## [1.4.0-hotfix.1] - 2025-09-29


### Features

* **btc-server:** add flag excluded_eth_addresses for coin selection ([7631ed9](https://github.com/botanix-labs/Macbeth/commit/7631ed98b3cddd45dc40b7f9799c3edf921e4859))

### Code Refactoring

* **btc-server:** remove unused error type ([8598590](https://github.com/botanix-labs/Macbeth/commit/8598590ee0ef8e4dcf00c1f845a81d5630e3af92))

### Miscellaneous

* **ci:** bump rust version on clippy checks ([3193291](https://github.com/botanix-labs/Macbeth/commit/3193291717f1e58f9532d46fc14fb0eb8e1605b8))
* **ci:** fix clippy cmdline ([5bdc045](https://github.com/botanix-labs/Macbeth/commit/5bdc04518473e52e7248c67fcc53ec21e0337fa2))
* **ci:** relax result-large-err clippy warning ([3a641ae](https://github.com/botanix-labs/Macbeth/commit/3a641aed5bdd4a6e51c67f4895a4d0c3c9127b46))
* **ci:** use clippy action ([993dfaa](https://github.com/botanix-labs/Macbeth/commit/993dfaabd9593173e1d61ce6514d4aae8dbbc38f))


**Downloads:** [Release Page](../../releases/1.4.0-hotfix.1/)


## [1.3.3-hotfix.1] - 2025-09-29


### Bug Fixes

* **test:** fix client import ([f754831](https://github.com/botanix-labs/Macbeth/commit/f7548313928b8771ce33eeb136551d172fb16321))

### Code Refactoring

* **test:** rename conflicting input to prevent resigning pegout ([83b0fcd](https://github.com/botanix-labs/Macbeth/commit/83b0fcd2271b0a49eb5e0c4091462ed039f4dba6))

### Tests

* **btc-server:** update conflictring input test to account for new behavior ([9c3ed77](https://github.com/botanix-labs/Macbeth/commit/9c3ed77d31d01d6cf9b38a9a99c167ac574f7bf5))

### Miscellaneous

* **release:** back-merge v1.3.2 from main to hotfix ([01d63ee](https://github.com/botanix-labs/Macbeth/commit/01d63ee91c6a186d6e873068daebb6e1e0f70e61))


**Downloads:** [Release Page](../../releases/1.3.3-hotfix.1/)


## [1.3.2-hotfix.3] - 2025-08-25


### Bug Fixes

* **log:** set frost command log to debug ([d356455](https://github.com/botanix-labs/Macbeth/commit/d356455f81f2d5cbc190e04176ac245e18bf59c0))
* **log:** set frost command log to debug ([#954](https://github.com/botanix-labs/Macbeth/issues/954)) ([cc17edd](https://github.com/botanix-labs/Macbeth/commit/cc17edd5f888907013f665a2000efb9cdfce5097))


**Downloads:** [Release Page](../../releases/1.3.2-hotfix.3/)


## [1.3.2-hotfix.2] - 2025-08-25


### Bug Fixes

* **config:** increase mainnet epoch length to 100 ([f173e7a](https://github.com/botanix-labs/Macbeth/commit/f173e7a430f8ee9a410bd1f59a77b2bafd93c551))
* **wallet-sync:** change log levels ([33f6446](https://github.com/botanix-labs/Macbeth/commit/33f6446c009fdc28653281bc6d7a551a0f04f1c2))
* **wallet-sync:** increase epoch length ([#953](https://github.com/botanix-labs/Macbeth/issues/953)) ([99ae576](https://github.com/botanix-labs/Macbeth/commit/99ae5768edfc4cad6950cbf946bbbeb39b902937))


**Downloads:** [Release Page](../../releases/1.3.2-hotfix.2/)


## [1.3.2-hotfix.1] - 2025-08-22


### Bug Fixes

* **pegouts:** don't store pegout if in finalized pegouts list ([089c8fd](https://github.com/botanix-labs/Macbeth/commit/089c8fd4b10cb9c034e0e44b7336e24db28f4e6e))
* **pegouts:** don't store pegout if it has been broadcasted ([419c57a](https://github.com/botanix-labs/Macbeth/commit/419c57aa1bbcf12d4a4985d57b2dc417f92121e9))
* **pegouts:** remove finalized pegout from pending pegout list ([15c3cdf](https://github.com/botanix-labs/Macbeth/commit/15c3cdfb6e447c32a980b156263b22f37a9ed4de))
* remove finalized pegout from pending pegout list ([#944](https://github.com/botanix-labs/Macbeth/issues/944)) ([e55c0f6](https://github.com/botanix-labs/Macbeth/commit/e55c0f6e86e8bb1a9670f461c6662639a6ea5440))

### Miscellaneous

* **logs:** set wallet state logs to trace for btc-server ([cd375e9](https://github.com/botanix-labs/Macbeth/commit/cd375e9be9433b2526fa5b06100e91c9bacd1d16))
* **release:** back-merge v1.3.1 from main to hotfix ([f2da833](https://github.com/botanix-labs/Macbeth/commit/f2da83302796c23d6a2da491c78b77d94eb3a679))


**Downloads:** [Release Page](../../releases/1.3.2-hotfix.1/)


## [1.3.1-hotfix.1] - 2025-08-20


### Bug Fixes

* **btc-server:** check is_coordinator before resetting pending pegouts ([#932](https://github.com/botanix-labs/Macbeth/issues/932)) ([6cacf76](https://github.com/botanix-labs/Macbeth/commit/6cacf7616408b8c93cbee423465b7bf92e8cef37))
* **btc-server:** pending pegout race condition ([#934](https://github.com/botanix-labs/Macbeth/issues/934)) ([34bb0a4](https://github.com/botanix-labs/Macbeth/commit/34bb0a4e41363905644edb40455795249b431206))

### Miscellaneous

* **release:** back-merge v1.3.0 from main to hotfix ([e874240](https://github.com/botanix-labs/Macbeth/commit/e874240667e96681f0c593b5a268e90c9faf1e7f))


**Downloads:** [Release Page](../../releases/1.3.1-hotfix.1/)


## [1.3.0-hotfix.5] - 2025-08-09



**Downloads:** [Release Page](../../releases/1.3.0-hotfix.5/)


## [1.3.0-hotfix.4] - 2025-08-09


### Bug Fixes

* **abci:** set version 0 to recover testnet ([3f51e91](https://github.com/botanix-labs/Macbeth/commit/3f51e91877fe489f87a5ceb283c931f7187a6ecd))
* **abci:** set version 0 to recover testnet ([#914](https://github.com/botanix-labs/Macbeth/issues/914)) ([1b9f87c](https://github.com/botanix-labs/Macbeth/commit/1b9f87c0f36c1848656236390523fed431271c61))


**Downloads:** [Release Page](../../releases/1.3.0-hotfix.4/)


## [1.3.0-hotfix.3] - 2025-08-08


### Bug Fixes

* **import:** remove duplicate import ([b6621dc](https://github.com/botanix-labs/Macbeth/commit/b6621dcacbe689991704671393e32c8659b698c7))

### Code Refactoring

* **peers:** add upstream trusted peers logic ([ffd5d95](https://github.com/botanix-labs/Macbeth/commit/ffd5d95f56921ca5f290a0d566f813b8ee34714e))
* **peers:** add upstream trusted peers logic ([#913](https://github.com/botanix-labs/Macbeth/issues/913)) ([0bb1c0d](https://github.com/botanix-labs/Macbeth/commit/0bb1c0d91e59ae33c35883f2de460b01b1bac79b))


**Downloads:** [Release Page](../../releases/1.3.0-hotfix.3/)


## [1.3.0-hotfix.2] - 2025-08-08


### Bug Fixes

* **botanix-up:** pass is_rpc_node param ([1cb555a](https://github.com/botanix-labs/Macbeth/commit/1cb555a09e5c6d3d223b1a0fa3412c4ffd251d23))

### Tests

* **rpc_node:** port changes from closed pr 740 ([0dff40d](https://github.com/botanix-labs/Macbeth/commit/0dff40d726615eef24c0fa112b632e471e3fe952))
* **rpc_node:** refactor setup and test ([eef415a](https://github.com/botanix-labs/Macbeth/commit/eef415a58528bfc10835dde053b4e384d6e0d0c3))
* **rpc_node:** spawn cometbft node for each rpc node ([6acf5ac](https://github.com/botanix-labs/Macbeth/commit/6acf5ace0c4d797f7c60cc63b01efe113595f17e))
* **rpc:** and zmq address to bitcoind ([274477d](https://github.com/botanix-labs/Macbeth/commit/274477d28edd80f195f6bc3816bcd8996c86c25a))

### Build System

* **import:** add back missed import ([c5c23c8](https://github.com/botanix-labs/Macbeth/commit/c5c23c8eb5ab2865ed9a8bdc368a81d0e4cad553))


**Downloads:** [Release Page](../../releases/1.3.0-hotfix.2/)


## [1.3.0-hotfix.1] - 2025-08-06


### Features

*  command to rollback blocks ([#908](https://github.com/botanix-labs/Macbeth/issues/908)) ([ad84301](https://github.com/botanix-labs/Macbeth/commit/ad84301e6373e2048c1a97c0083b9c3cf7b4eb96))
*  command to rollback blocks ([#909](https://github.com/botanix-labs/Macbeth/issues/909)) ([45d3044](https://github.com/botanix-labs/Macbeth/commit/45d30446e77ce8e32d99ec6751c4d3ef88f12425))

### Miscellaneous

* **release:** back-merge v1.2.0 from main to hotfix ([e1cf64f](https://github.com/botanix-labs/Macbeth/commit/e1cf64f988188ed9e4fffa782569df4a74e189d4))


**Downloads:** [Release Page](../../releases/1.3.0-hotfix.1/)


## [1.2.0-hotfix.3] - 2025-08-05


### Features

* runtime version 3 adjust floor base fee! ([#901](https://github.com/botanix-labs/Macbeth/issues/901)) ([2ad22b0](https://github.com/botanix-labs/Macbeth/commit/2ad22b078fe98427b9ead87b57b683b27ae872ce))

### Code Refactoring

* set floor base fee to 0.0005 GWEI ([fb62d01](https://github.com/botanix-labs/Macbeth/commit/fb62d010b396712e5b816565d488092fb9085efa))

### Continuous Integration

* allow for stable release to persist ([b0cb977](https://github.com/botanix-labs/Macbeth/commit/b0cb977544dbc0f825f579f17499ff1975b2bc4e))
* allow for stable release to persist ([#898](https://github.com/botanix-labs/Macbeth/issues/898)) ([9785f86](https://github.com/botanix-labs/Macbeth/commit/9785f86cc0b99e6a1812aa2df3fb00f3a6e4ca11))


**Downloads:** [Release Page](../../releases/1.2.0-hotfix.3/)


## [1.2.0-hotfix.2] - 2025-08-05


### Continuous Integration

* allow last stable release to persist on public release pags ([cef35fd](https://github.com/botanix-labs/Macbeth/commit/cef35fdff3eca0d1b91f13562abc9914e05e5897))
* explicit tags on readme ([bf4d903](https://github.com/botanix-labs/Macbeth/commit/bf4d903c4f711b6f4dac8a3b8fb76f4eb73d75a4))
* refactor release flow to publish only stable releases to public repo ([b4e4d5b](https://github.com/botanix-labs/Macbeth/commit/b4e4d5b0e1c7e0f0241b000cad264e958c6bcb83))
* refactor release flow to publish only stable releases to public repo ([#896](https://github.com/botanix-labs/Macbeth/issues/896)) ([5e17625](https://github.com/botanix-labs/Macbeth/commit/5e17625e72a61663516803fcfa23546ed3ba016a))


**Downloads:** [Release Page](../../releases/1.2.0-hotfix.2/)


## [1.0.5-hotfix.1] - 2025-08-05


### Continuous Integration

* publish public fixes ([71d2fc5](https://github.com/botanix-labs/macbeth-release/commit/71d2fc536d0093ab1dd2910e9c550187fe2686df))

### Miscellaneous

* **release:** back-merge v1.0.4 from main to hotfix ([eb09b03](https://github.com/botanix-labs/macbeth-release/commit/eb09b03e9ea67bcaf27ca5d7401f711e8b9e6daa))


**Downloads:** [Release Page](../../releases/1.0.5-hotfix.1/)


## [1.0.4-hotfix.1] - 2025-08-05


### Continuous Integration

* test fix for public repo ([be79803](https://github.com/botanix-labs/macbeth-release/commit/be79803c748874dc26739e82e3b85126e25ac055))

### Miscellaneous

* **release:** back-merge v1.0.3 from main to hotfix ([2adbcb8](https://github.com/botanix-labs/macbeth-release/commit/2adbcb834a03513f02c210aca9ad3c4242e732c1))


**Downloads:** [Release Page](../../releases/1.0.4-hotfix.1/)


## [1.2.0-hotfix.1] - 2025-08-05


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


**Downloads:** [Release Page](../../releases/1.2.0-hotfix.1/)


## [1.1.14-hotfix.3] - 2025-08-04


### Miscellaneous

* **docs:** remove network launch docs until upstream merge ([b37b1d6](https://github.com/botanix-labs/Macbeth/commit/b37b1d614272b8cf6fa7e94a6a8f3babcba6f74b))


**Downloads:** [Release Page](../../releases/1.1.14-hotfix.3/)


## [1.1.14-hotfix.2] - 2025-08-01


### Bug Fixes

* **priority fee:** remove enforced minimum ([80e7dd9](https://github.com/botanix-labs/Macbeth/commit/80e7dd9fb4427cf409c42e19a607e68d46625d6c))
* **priority fee:** remove enforced minimum ([#883](https://github.com/botanix-labs/Macbeth/issues/883)) ([c399b5b](https://github.com/botanix-labs/Macbeth/commit/c399b5b8fbbf20b8845b82fdfe6ff94bae2e2aa3))

### Miscellaneous

* **release:** bump version to 1.1.14-hotfix.2 ([f906a06](https://github.com/botanix-labs/Macbeth/commit/f906a0612ae01c54aafe34a4248a0c9d8933f14c))


**Downloads:** [Release Page](../../releases/1.1.14-hotfix.2/)


## [1.1.14-hotfix.2] - 2025-07-31


### Bug Fixes

* **priority fee:** remove enforced minimum ([80e7dd9](https://github.com/botanix-labs/Macbeth/commit/80e7dd9fb4427cf409c42e19a607e68d46625d6c))
* **priority fee:** remove enforced minimum ([#883](https://github.com/botanix-labs/Macbeth/issues/883)) ([c399b5b](https://github.com/botanix-labs/Macbeth/commit/c399b5b8fbbf20b8845b82fdfe6ff94bae2e2aa3))


**Downloads:** [Release Page](../../releases/1.1.14-hotfix.2/)


## [1.1.14-hotfix.1] - 2025-07-24


### Continuous Integration

* modify release flow  ([#873](https://github.com/botanix-labs/Macbeth/issues/873)) ([566d39a](https://github.com/botanix-labs/Macbeth/commit/566d39ab5e32bfd0d80d37813210a3602ed94567))

### Miscellaneous

* **release:** back-merge v1.1.13 from main to hotfix ([29fdbf5](https://github.com/botanix-labs/Macbeth/commit/29fdbf51b66c4c516316078c3d02bdd30d90ab99))


**Downloads:** [Release Page](../../releases/1.1.14-hotfix.1/)


## [1.1.13-hotfix.1] - 2025-07-22


### Continuous Integration

* fix building docker images job in release workflow ([#866](https://github.com/botanix-labs/Macbeth/issues/866)) ([ea35f16](https://github.com/botanix-labs/Macbeth/commit/ea35f165c8aab93b7b0b5aedb9a6e29ff57ca69b))

### Miscellaneous

* **release:** back-merge v1.1.12 from main to hotfix ([1d2a0c4](https://github.com/botanix-labs/Macbeth/commit/1d2a0c4eb77e2e66efa8b2a041594dc9a0aea538))


**Downloads:** [Release Page](../../releases/1.1.13-hotfix.1/)


## [1.1.11-hotfix.1] - 2025-07-21


### Bug Fixes

* **change-outputs:** remove list of change outputs ([#853](https://github.com/botanix-labs/Macbeth/issues/853)) ([7515c8d](https://github.com/botanix-labs/Macbeth/commit/7515c8d1d1d25fe03dace1a234bf73dc022368a3))
* **change-outputs:** set scan to false ([107b390](https://github.com/botanix-labs/Macbeth/commit/107b390b31d1d4bcd333411abb45b62ffd0d63bd))

### Continuous Integration

* semantic release flow ([#749](https://github.com/botanix-labs/Macbeth/issues/749)) ([316400d](https://github.com/botanix-labs/Macbeth/commit/316400d2b8375234c598788f05b96ac620b8c135))

### Miscellaneous

* bump to v1.1.12 ([ddb0e92](https://github.com/botanix-labs/Macbeth/commit/ddb0e9228326d9d0e8842a5ed6ab5d6719bc3fba))


**Downloads:** [Release Page](../../releases/1.1.11-hotfix.1/)


