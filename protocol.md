# 

# Protocol Outline

100% EDI

100% Electronic to Paper

#### 

#### 

#### Protocol Structure

A protocol consists of the following components:

* **Exchange**
  . The protocol exchange is the series of messages exchanged between all parties in the state channel, as well as dependencies between messages.
* **Message**
  . A message is the set of information that must be exchanged by the parties to recreate and validate the commitment signatures and associated transactions that those signatures enable. Each protocol may in general contain multiple message types.
* **Commitments**
  . A protocol produces one or more commitments. Both the signatures and the data contained within the commitments must be stored.

## Freight Protocol

## 

```markdown
,  

Unique Address, 0x

Agreement Identifier, 

x.509 Cert

XML


Contract Instrument Semi-NFT 

STANDARDS UTILIZED 

137
191
725
777
1077
1154
1400
1613
1775

NEW

?NUM0x1
?NUM0x2
```

#### Contract Instrument Semi-NFT

|  |  |
| :--- | :--- |
| ERC1400 |  |
| ERC1643 Document Managment |  |
| ERC1154 |  |
| EIP 1077: Executable Signed Messages |  |
| EIP 1775 |  |
| "Bishop" Kernel |  |
| "Fulcrum" Adaptor |  |

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

**Ethereum Registration Authority / Trusted Certificate Authority**

```
Data Field for Signature Injection <Triggering_Event>

function transferWithData(address recipient, uint256 value, bytes data)
```

**ERC1643 implementation**

AddressID specifices which package is used for that operation/interogatives and subordinate clauses

Enables Agreement to be as homogonized or unique as needed, thereby extending possiblity of liquidity

?NUM0x1

Assign

### 

---

### 

## Smart Contract Package

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

**Stand Alone:**    Package has no external dependencies \(i.e. no build\_dependencies\), contains all contract data needed without reaching into another package.

**Dependent:   ** Package does not contain all necessary contract data \(i.e. has build\_dependencies\), must reach into a package dependency to retrieve data.

**Inheritable**:    Contract doesn’t provide useful functionality on it’s own and is meant to serve as a base contract for others to inherit from.

**Reusable: **   Contract is useful on it’s own, meant to be used as-is. This applies only to kernel level contracts.

**Deployed Contract/Library:**

```
 Refers to an instance of a contract/library that has already been deployed to a specific address on a chain.
```

**Package Dependency:**

```
 External dependency directly referenced via the build\_dependencies of the package.
```

**Deep Dependency:**

```
 External dependency referenced via the build\_dependencies of a package dependency 
 (or by reaching down dependency tree as far as necessary\).
```

| &lt;/&gt; | Action |
| :--- | :--- |
| defaultOperator | Freight Trust, _Network Operations _ |
| AuthorizedOperator | 3rd Party \(e.g. Invoice Factoring, Insurance, etc\) |
| RevokedOperator |  |
| setManager | Deployed On-Contracts, _Network Operations_ |
| getAttributeTypeID |  |
| hasAttribute |  |
| symbol | Self Describing Contract Parameters |
|  |  |
| **Legal Aspects** |  |
| documentationIdentification |  |
| legalAgreement |  |
| masterAgreement |  |
| tradeAgreement |  |
| uniqueAgreement |  |
| effectiveDate |  |
| eventDate |  |
| eventQualifier |  |
| eventIdentifier |  |
| lineage |  |
| contractKeyUID |  |
|  |  |

#### 

#### 



* [SystemController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#system_controller)
* [DriverController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#driver_controller)
* [ShipperController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#shipper_controller)
* [CarrierController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#carrier_controller)
* [ReceiverController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#receiver_controller)
* [DriverPassportController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#driver_passport_controller)
* [AddDriverController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#add_driver_controller)
* [CreateDriverPassportController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#create_driver_passport_controller)
* [UpdateDriverPassportController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#update_driver_passport_controller)
* [ChangeDriverCarrierController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#change_driver_carrier_controller)
* [RemoveDriverCarrierController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#remove_driver_carrier_controller)
* [DailyLogDefectsReportController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#daily_log_defects_report_controller)
* [DailyLogController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#daily_log_controller)
* [DriverDailyLogTickController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#driver_daily_log_tick_controller)
* [BillOfLadingController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#bill_of_lading_controller)
* [DetentionController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#detention_controller)
* [QuoteController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#quote_controller)
* [LoadController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#load_controller)
* [AssignDriverToLoadController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#assign_driver_to_load_controller)
* [OriginArrivalController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#origin_arrival_controller)
* [LoadPickupController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#load_pickup_controller)
* [DestinationArrivalController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#destination_arrival_controller)
* [LoadDropOffController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#load_drop_off_controller)
* [ListLoadController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#list_load_controller)
* [SubmitQuoteController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#submit_quote_controller)
* [AcceptQuoteController](https://bitbucket.org/blockarraygroup/seal/src/AS2/#accept_quote_controller)

####  Get singleton instance

#### The singleton instance of the`SystemController`class can be accessed from the API Client.

```
SystemController system = client.System;
```

### GetSystemPing {#markdown-header-a-nameget_system_pinga-getsystemping}

> _Tags:_`Skips Authentication`
>
> Test the connection to the network

```
Task
<
Models
.
PingResponse
>GetSystemPing()
```

#### Example Usage {#markdown-header-example-usage}

```
Models
.
PingResponse
result
=
await
system
.
GetSystemPing
()
```

#### 

#### 

#### Templates, Agreements and Parameters

A template is an electronic representation of a legal document as issued by a standards body — for example, by the International Swaps and Derivatives Association \(ISDA\). As illustrated in Figure 2, a template contains both legal prose and parameters, where each parameter has an identity \(a unique name\), a type, and may \(but need not\) have a value.d

> > ![](/assets/Screenshot 2019-05-03 11.49.26.png)

A template may contain both legal prose and parameters. Each parameter has an identifier \(a name\), a type, and an optional value. Agreements are derived from templates, and both the legal prose and parameters may be customised during negotiation. Values are mandatory for all parameters in a signed agreement.

---

~~A Viable Systems Model approach~~

~~Contracts~~

### Linking Legal Agreements to Contracts and Events

This referencing of the legal agreement from the`Contract`is done through the`documentation`attribute. Alongside with providing the ability to identify some of the key terms of a governing legal agreement \(such as the agreement identifier, the publisher, the document vintage and the agreement date\) as part of the`documentationIdentification`attribute, the associated`Documentation`class provides the ability to reference a legal agreement that is electronically represented on-chain through the`legalAgreement`attribute, which has a reference key into the instance agreement.

The below snippet represents this`Documentation`class, which`legalAgreement`attribute carries the`reference`qualifier.

