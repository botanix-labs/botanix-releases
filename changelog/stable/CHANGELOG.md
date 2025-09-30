# Botanix stable Channel Changelog

All notable changes to the stable release channel will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.4.0] - 2025-09-30


### Features

* **btc-utils:** Init binary & implement export/import mechanism for Frost keys ([#973](https://github.com/botanix-labs/Macbeth/issues/973)) ([2b87751](https://github.com/botanix-labs/Macbeth/commit/2b87751f513fdb31e9cbf1bea2e885b86ce04db0))


**Downloads:** [Release Page](../../releases/1.4.0/)


## [1.3.2] - 2025-08-25


### Bug Fixes

* **config:** increase mainnet epoch length to 100 ([f173e7a](https://github.com/botanix-labs/Macbeth/commit/f173e7a430f8ee9a410bd1f59a77b2bafd93c551))
* **log:** set frost command log to debug ([d356455](https://github.com/botanix-labs/Macbeth/commit/d356455f81f2d5cbc190e04176ac245e18bf59c0))
* **log:** set frost command log to debug ([#954](https://github.com/botanix-labs/Macbeth/issues/954)) ([cc17edd](https://github.com/botanix-labs/Macbeth/commit/cc17edd5f888907013f665a2000efb9cdfce5097))
* **pegouts:** don't store pegout if in finalized pegouts list ([089c8fd](https://github.com/botanix-labs/Macbeth/commit/089c8fd4b10cb9c034e0e44b7336e24db28f4e6e))
* **pegouts:** don't store pegout if it has been broadcasted ([419c57a](https://github.com/botanix-labs/Macbeth/commit/419c57aa1bbcf12d4a4985d57b2dc417f92121e9))
* **pegouts:** remove finalized pegout from pending pegout list ([15c3cdf](https://github.com/botanix-labs/Macbeth/commit/15c3cdfb6e447c32a980b156263b22f37a9ed4de))
* remove finalized pegout from pending pegout list ([#944](https://github.com/botanix-labs/Macbeth/issues/944)) ([e55c0f6](https://github.com/botanix-labs/Macbeth/commit/e55c0f6e86e8bb1a9670f461c6662639a6ea5440))
* **wallet-sync:** change log levels ([33f6446](https://github.com/botanix-labs/Macbeth/commit/33f6446c009fdc28653281bc6d7a551a0f04f1c2))
* **wallet-sync:** increase epoch length ([#953](https://github.com/botanix-labs/Macbeth/issues/953)) ([99ae576](https://github.com/botanix-labs/Macbeth/commit/99ae5768edfc4cad6950cbf946bbbeb39b902937))

### Miscellaneous

* **logs:** set wallet state logs to trace for btc-server ([cd375e9](https://github.com/botanix-labs/Macbeth/commit/cd375e9be9433b2526fa5b06100e91c9bacd1d16))
* merge hotfix into main ([#945](https://github.com/botanix-labs/Macbeth/issues/945)) ([ae90781](https://github.com/botanix-labs/Macbeth/commit/ae90781ff7e9d89945006709ef7725efd6ab5f61))
* **release:** back-merge v1.3.1 from main to hotfix ([f2da833](https://github.com/botanix-labs/Macbeth/commit/f2da83302796c23d6a2da491c78b77d94eb3a679))
* **release:** bump version to 1.3.2-hotfix.1 ([7aa665d](https://github.com/botanix-labs/Macbeth/commit/7aa665d8a3639a18e61c6840fb508b4e7fd5d46f))
* **release:** bump version to 1.3.2-hotfix.2 ([4cc466f](https://github.com/botanix-labs/Macbeth/commit/4cc466fbf0b127d5a01fffbe01b7ecc74c1e8d8c))
* **release:** bump version to 1.3.2-hotfix.3 ([ec3d903](https://github.com/botanix-labs/Macbeth/commit/ec3d903d948ce83993d3e014a204cdd0f8689305))


**Downloads:** [Release Page](../../releases/1.3.2/)


## [1.3.1] - 2025-08-21


### Bug Fixes

* **btc-server:** check is_coordinator before resetting pending pegouts ([#932](https://github.com/botanix-labs/Macbeth/issues/932)) ([6cacf76](https://github.com/botanix-labs/Macbeth/commit/6cacf7616408b8c93cbee423465b7bf92e8cef37))
* **btc-server:** pending pegout race condition ([#934](https://github.com/botanix-labs/Macbeth/issues/934)) ([34bb0a4](https://github.com/botanix-labs/Macbeth/commit/34bb0a4e41363905644edb40455795249b431206))
* pending pegouts race condition ([#938](https://github.com/botanix-labs/Macbeth/issues/938)) ([41dd0fd](https://github.com/botanix-labs/Macbeth/commit/41dd0fd56a7b7d36e5489e02ea64f89afd9725d2))

### Miscellaneous

* **release:** back-merge v1.3.0 from main to hotfix ([e874240](https://github.com/botanix-labs/Macbeth/commit/e874240667e96681f0c593b5a268e90c9faf1e7f))
* **release:** bump version to 1.3.1-hotfix.1 ([2689a0d](https://github.com/botanix-labs/Macbeth/commit/2689a0d0ed3b89703f18000352b60ccc6a2c95c1))


**Downloads:** [Release Page](../../releases/1.3.1/)


## [1.3.0] - 2025-08-11


### Features

*  command to rollback blocks ([#908](https://github.com/botanix-labs/Macbeth/issues/908)) ([ad84301](https://github.com/botanix-labs/Macbeth/commit/ad84301e6373e2048c1a97c0083b9c3cf7b4eb96))
*  command to rollback blocks ([#909](https://github.com/botanix-labs/Macbeth/issues/909)) ([45d3044](https://github.com/botanix-labs/Macbeth/commit/45d30446e77ce8e32d99ec6751c4d3ef88f12425))

### Bug Fixes

* **abci:** set version 0 to recover testnet ([#914](https://github.com/botanix-labs/Macbeth/issues/914)) ([1b9f87c](https://github.com/botanix-labs/Macbeth/commit/1b9f87c0f36c1848656236390523fed431271c61))
* **botanix-up:** pass is_rpc_node param ([1cb555a](https://github.com/botanix-labs/Macbeth/commit/1cb555a09e5c6d3d223b1a0fa3412c4ffd251d23))
* **import:** remove duplicate import ([b6621dc](https://github.com/botanix-labs/Macbeth/commit/b6621dcacbe689991704671393e32c8659b698c7))

### Code Refactoring

* **peers:** add upstream trusted peers logic ([ffd5d95](https://github.com/botanix-labs/Macbeth/commit/ffd5d95f56921ca5f290a0d566f813b8ee34714e))
* **peers:** add upstream trusted peers logic ([#913](https://github.com/botanix-labs/Macbeth/issues/913)) ([0bb1c0d](https://github.com/botanix-labs/Macbeth/commit/0bb1c0d91e59ae33c35883f2de460b01b1bac79b))

### Tests

* **rpc_node:** port changes from closed pr 740 ([0dff40d](https://github.com/botanix-labs/Macbeth/commit/0dff40d726615eef24c0fa112b632e471e3fe952))
* **rpc_node:** refactor setup and test ([eef415a](https://github.com/botanix-labs/Macbeth/commit/eef415a58528bfc10835dde053b4e384d6e0d0c3))
* **rpc_node:** spawn cometbft node for each rpc node ([6acf5ac](https://github.com/botanix-labs/Macbeth/commit/6acf5ace0c4d797f7c60cc63b01efe113595f17e))
* **rpc:** and zmq address to bitcoind ([274477d](https://github.com/botanix-labs/Macbeth/commit/274477d28edd80f195f6bc3816bcd8996c86c25a))

### Build System

* **import:** add back missed import ([c5c23c8](https://github.com/botanix-labs/Macbeth/commit/c5c23c8eb5ab2865ed9a8bdc368a81d0e4cad553))

### Miscellaneous

* **release:** back-merge v1.2.0 from main to hotfix ([e1cf64f](https://github.com/botanix-labs/Macbeth/commit/e1cf64f988188ed9e4fffa782569df4a74e189d4))
* **release:** bump version to 1.3.0-hotfix.1 ([4ac14db](https://github.com/botanix-labs/Macbeth/commit/4ac14db43faa1db42651124d3fc1691c6ffc1c00))
* **release:** bump version to 1.3.0-hotfix.2 ([8676d1c](https://github.com/botanix-labs/Macbeth/commit/8676d1c66e03ea9a022b3a72a2ff2966260f2c83))
* **release:** bump version to 1.3.0-hotfix.3 ([4c98011](https://github.com/botanix-labs/Macbeth/commit/4c98011fd3df42216137b32b1324366447903f49))
* **release:** bump version to 1.3.0-hotfix.4 ([89c4926](https://github.com/botanix-labs/Macbeth/commit/89c4926c7ab8c42ec7fa70b0c6f6ef56ee3f9e6d))
* **release:** bump version to 1.3.0-hotfix.5 ([72abd13](https://github.com/botanix-labs/Macbeth/commit/72abd138b3855669b29f6674a2cce485bf23a0c5))


**Downloads:** [Release Page](../../releases/1.3.0/)


## [1.2.0] - 2025-08-05


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


**Downloads:** [Release Page](../../releases/1.2.0/)


## [1.0.5] - 2025-08-05


### Continuous Integration

* publish public fixes ([71d2fc5](https://github.com/botanix-labs/macbeth-release/commit/71d2fc536d0093ab1dd2910e9c550187fe2686df))

### Miscellaneous

* **release:** back-merge v1.0.4 from main to hotfix ([eb09b03](https://github.com/botanix-labs/macbeth-release/commit/eb09b03e9ea67bcaf27ca5d7401f711e8b9e6daa))
* **release:** bump version to 1.0.5-hotfix.1 ([ed905ba](https://github.com/botanix-labs/macbeth-release/commit/ed905ba88e78713de9fdae123a01ed779b405e49))


**Downloads:** [Release Page](../../releases/1.0.5/)


## [1.0.4] - 2025-08-05


### Continuous Integration

* test fix for public repo ([be79803](https://github.com/botanix-labs/macbeth-release/commit/be79803c748874dc26739e82e3b85126e25ac055))

### Miscellaneous

* **release:** back-merge v1.0.3 from main to hotfix ([2adbcb8](https://github.com/botanix-labs/macbeth-release/commit/2adbcb834a03513f02c210aca9ad3c4242e732c1))
* **release:** bump version to 1.0.4-hotfix.1 ([54dc98d](https://github.com/botanix-labs/macbeth-release/commit/54dc98d2406c630042beaa16bc0759e8113c6d99))


**Downloads:** [Release Page](../../releases/1.0.4/)


## [1.1.13] - 2025-07-22


### Continuous Integration

* fix building docker images job in release workflow ([#866](https://github.com/botanix-labs/Macbeth/issues/866)) ([ea35f16](https://github.com/botanix-labs/Macbeth/commit/ea35f165c8aab93b7b0b5aedb9a6e29ff57ca69b))

### Miscellaneous

* **release:** back-merge v1.1.12 from main to hotfix ([1d2a0c4](https://github.com/botanix-labs/Macbeth/commit/1d2a0c4eb77e2e66efa8b2a041594dc9a0aea538))
* **release:** bump version to 1.1.13-hotfix.1 ([ac356c3](https://github.com/botanix-labs/Macbeth/commit/ac356c33f0476a12e8b7d37cf13c44e017de0be2))


**Downloads:** [Release Page](../../releases/1.1.13/)


## [1.1.12] - 2025-07-21


### Continuous Integration

* semantic release flow ([#749](https://github.com/botanix-labs/Macbeth/issues/749)) ([316400d](https://github.com/botanix-labs/Macbeth/commit/316400d2b8375234c598788f05b96ac620b8c135))

### Miscellaneous

* bump to v1.1.12 ([ddb0e92](https://github.com/botanix-labs/Macbeth/commit/ddb0e9228326d9d0e8842a5ed6ab5d6719bc3fba))
* merge hotfix into main ([#862](https://github.com/botanix-labs/Macbeth/issues/862)) ([2e730b1](https://github.com/botanix-labs/Macbeth/commit/2e730b166a2d18bcf8b9441f7a4d1dbb03656709))
* **release:** bump version to 1.1.11-hotfix.1 ([997becb](https://github.com/botanix-labs/Macbeth/commit/997becb3dc820d01d435ece4a426de15023af8b5))


**Downloads:** [Release Page](../../releases/1.1.12/)


## [1.1.2-hotfix] - 2025-06-30



**Downloads:** [Release Page](../../releases/1.1.2-hotfix/)


## [1.1.2] - 2025-06-30



**Downloads:** [Release Page](../../releases/1.1.2/)


