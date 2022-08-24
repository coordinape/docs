---
description: Description of the smart contracts that power the Coordinape Vaults.
---

# CoVaults Techincal

### Key Roles and Contracts

* The **vault factory** ([ApeVaultFactory](https://github.com/coordinape/coordinape-protocol/blob/main/contracts/ApeProtocol/wrapper/beacon/ApeVaultFactory.sol)) creates new **vaults** ([ApeVault)](https://github.com/coordinape/coordinape-protocol/blob/main/contracts/ApeProtocol/wrapper/beacon/ApeVault.sol) containing funds for a different organization using Coordinape.
* According to a Merkle tree, the **distributor** ([ApeDistributor](https://github.com/coordinape/coordinape-protocol/blob/main/contracts/ApeProtocol/ApeDistributor.sol)) distributes tokens to contributors. When a distribution occurs, tokens are transferred from a vault to the distributor. Only the vault's owner can submit a distribution.
* When tokens are deposited into or withdrawn from vaults, the **router** ([ApeRouter](https://github.com/coordinape/coordinape-protocol/blob/main/contracts/ApeProtocol/ApeRouter.sol)) manages the process to make tracking TVL easier.
* The **registry** ([ApeRegistry](https://github.com/coordinape/coordinape-protocol/blob/main/contracts/ApeProtocol/ApeRegistry.sol)) contains system-wide settings.

![](<../../.gitbook/assets/coordinape system diagram.png>)

The links above go to our Github repo for contracts, [coordinape/coordinape-protocol](https://github.com/coordinape/coordinape-protocol), which also contains a test suite written with [a brownie](https://github.com/eth-brownie/brownie). Additional tests that exercise the contracts on a Ganache test chain can be found in [our frontend repo](https://github.com/coordinape/coordinape).

### Two Types of Vaults

Vaults can be initialized as Yearn Vaults (with a non-zero `_token` constructor argument) or Basic Vaults (with a non-zero `_simpleToken` constructor argument). A Yearn Vault for a token converts deposits into the corresponding yield-bearing Yearn wrapper token, e.g. `yvDAI` for `DAI`, and stores that in the vault. Yearn Vaults, therefore, support only tokens for which Yearn wrapper tokens are available. Basic Vaults can store any ERC-20 token.

### Security and Upgradability

Any address can deposit funds into a vault, but only the vault's owner can withdraw any funds.

The **registry** determines which factory, distributor, and router are in use. These can be changed by the registry owner, which is currently the Coordinape [multisig](https://etherscan.io/address/0x15b513f658f7390d8720dce321f50974b28672ef). These changes are time-locked, so vault users have time to withdraw their tokens if the registry is somehow compromised.

The registry also references a fee registry component, as seen in the diagram above, which can be used to charge fees on distributions from vaults. There are no plans to charge any fees.

The vaults use the [Beacon Proxy](https://docs.openzeppelin.com/contracts/3.x/api/proxy#BeaconProxy) pattern for upgradability so that all existing vaults can be upgraded with a single transaction to add functionality or fix a bug. This is also executable only by the beacon owner (the Coordinape multisig) and time-locked.

A vault owner can "opt-out" of upgrades by calling `setBeaconDeploymentPrefs`. Please ask in [our Discord](https://discord.coordinape.com/) if you would like more details about this.

See below for links to our security audits.

### Contract Addresses

The addresses currently in use on [app.coordinape.com](https://app.coordinape.com) are stored in [deploymentInfo.json](https://github.com/coordinape/coordinape/blob/main/hardhat/deploymentInfo.json). The top-level sections in that JSON file are keyed by chain ID, i.e. `1` is mainnet and `5` is Görli.

### Future Functionality

There is some functionality present in the contracts that are not supported by our front-end app:

* The distributor can send tokens directly to end-user addresses, rather than having their claim from a Merkle root (`ApeDistributor.tapEpochAndDistribute`).
* A vault owner can designate one address per circle as a "distribution manager" (`ApeVault.updateCircleAdmin`), and set a time-limited allowance (`ApeVault.updateAllowance`) for that address to distribute tokens from their vault.
* A vault can be initialized with a Yearn-backed token address and a basic/simple token address and receive and distribute both of those tokens independently. (This use case is unlikely to be supported on the front-end for the sake of UX simplicity.)

### Audits

Coordinape's vault contracts underwent two thorough security audits. Both audits deemed the use of our contracts to be "Low Risk".\
\
**Primary Audit:** [**https://github.com/blocksecteam/audit-reports/blob/main/solidity/blocksec\_coordinape\_v1.1\_signed.pdf**](https://github.com/blocksecteam/audit-reports/blob/main/solidity/blocksec\_coordinape\_v1.1\_signed.pdf)****

After the primary audit with BlockSec, additional features were added to the contracts. A secondary audit was performed by SlowMist.

**Secondary Audit:** [**https://github.com/slowmist/Knowledge-Base/blob/master/open-report-V2/smart-contract/SlowMist%20Audit%20Report%20-%20Coordinape%20protocol\_en-us.pdf**](https://github.com/slowmist/Knowledge-Base/blob/master/open-report-V2/smart-contract/SlowMist%20Audit%20Report%20-%20Coordinape%20protocol\_en-us.pdf)
