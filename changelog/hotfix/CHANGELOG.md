# Botanix hotfix Channel Changelog

All notable changes to the hotfix release channel will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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


