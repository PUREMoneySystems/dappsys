`dappsys`
===

`dappsys` is a **contract system framework**. It is a collection of contracts **mixins**, **factories**, and **interfaces** written in Solidity that were created to support a system with many interacting Ethereum contracts.

The core feature of `dappsys` is the `DSKernel` contract type.*
This contract will be a "fully dynamic object". The creator owns a contract which can be modified arbitraily, including the ability to "solidify" and constrain its ability to change itself. It is the union of several generalizations:

* A *dynamic ABI* (`dynin`)
* Ability to do *dynamic calls* (`dynout`)
* Ability to do *dynamic events* (`dynlog`)
* A managed subsystem (`auth`)

The value of the first 3 components


* certain restrictions in the Solidity language definition prevent us from creating this contract in pure Solidity. For now, the Kernel is split into component contracts, giving you several workaround options. Fortunately these critical features are still on the official solidity roadmap.
