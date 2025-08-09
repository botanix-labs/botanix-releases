# Botanix hotfix Channel Changelog

All notable changes to the hotfix release channel will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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


