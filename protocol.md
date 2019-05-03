protocol

Semi-NFT

| ERC777 |
| :--- |
| ERC1400 |
| ERC1643 Document Managment |
| ERC1154 |
|  |
|  |

**ERC777 implementation - Advanced token standard for asset transfers**

* Empowerment of operators with the ability to send tokens on behalf of other addresses.
* Setup of send/receive hooks to offer token holders more control over their tokens.
* Use of ER820\(eips.ethereum.org/EIPS/eip-820\) to notify contracts and regular addresses when they receive tokens.
* Backwards compatible with ERC20.

**ERC1400 implementation - Partially fungible token standard**

* Differentiated ownership / transparent restrictions.
* Controller operations \(force transfer\).
* On-chain restriction checking with error signalling, off-chain data injection for transfer restrictions and issuance / redemption semantics.
* Document management.
* Backwards compatible with ERC20 and ERC777.

Ethereum Registration Authority / Trusted Certificate Authority

```
function transferWithData(address recipient, uint256 value, bytes data)
```

**ERC1643 implementation - Self Describing Address and Document Managment for Analog Contracts**

* AddressID specifices which package is used for that operation/interogatives and subordinate clauses  
* Enables Agreement to be as homogonized or unique as needed, thereby extending possiblity of liquidity 
* Eth

**Novel ERC &lt;EIP&gt;**

TransformAttribute

TranformInterface

DefineTransformInterface

InvokeEmission

Smart Contract

a **registry** is a deployed contract which manages a collection of packages.

a **package** is a collection of releases

a **package** is identified by a unique string name and unique bytes32 packageId within a given registry

a** release** is identified by a bytes32 releaseId which must be unique for a given package name and release version string pair.

a** releaseId **maps to a set of data that includes a manifestURI string which describes the location of an EIP 1123 package manifest. This manifest contains data about the release including the location of its component code assets.

a **manifestURI** is a URI as defined by RFC3986 which can be used to retrieve the contents of the package manifest. In addition to validation against RFC3986, each manifestURI must also contain a hash of the content as specified in the EIP 1123.

a l**ibrary** is a staticc set of standard contracts like SafeMath. **libsol **is the authoratative library.

the **Kernel** compromises interlocking contracts that execute operations by invocation or trigger

```
Registry -> Package [libsol, kernel...] -> Release [specific contract updates] -> latest release
```

Stand Alone:    Package has no external dependencies \(i.e. no build\_dependencies\), contains all contract data needed without reaching into another package.

Dependent:    Package does not contain all necessary contract data \(i.e. has build\_dependencies\), must reach into a package dependency to retrieve data.

Inheritable:    Contract doesn’t provide useful functionality on it’s own and is meant to serve as a base contract for others to inherit from.

Reusable:    Contract is useful on it’s own, meant to be used as-is.

Deployed Contract/Library:

```
 Refers to an instance of a contract/library that has already been deployed to a specific address on a chain.
```

Package Dependency:

```
 External dependency directly referenced via the build\_dependencies of a package.
```

Deep Dependency:

```
 External dependency referenced via the build\_dependencies of a package dependency \(or by reaching down dependency tree as far as necessary\).
```

|  |  |
| :--- | :--- |
| defaultOperator | Freight Trust, _Network Operations _ |
| AuthorizedOperator | 3rd Party \(e.g. Invoice Factoring, Insurance, etc\) |
| RevokedOperator |  |
| setManager | Deployed On-Contracts, _Network Operations_ |
| getAttributeTypeID |  |
| hasAttribute |  |
| symbol | Self Describing Contract Parameters |
|  |  |



'





#### Templates and Parameters 



A template is an electronic representation of a legal document as issued by a standards body — for example, by the International Swaps and Derivatives Association \(ISDA\). As illustrated in Figure 2, a template contains both legal prose and parameters, where each parameter has an identity \(a unique name\), a type, and may \(but need not\) have a value.d









> > ![](/assets/Screenshot 2019-05-03 11.49.26.png)



A template may contain both legal prose and parameters. Each parameter has an identifier \(a name\), a type, and an optional value. Agreements are derived from templates, and both the legal prose and parameters may be customised during negotiation. Values are mandatory for all parameters in a signed agreement.



 

 

 

 

 

 

 

 

---



