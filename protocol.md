protocol 





```

```







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



|  |  |
| :--- | :--- |
| defaultOperator | Freight Trust, _Network Operations _ |
| AuthorizedOperator | 3rd Party \(e.g. Invoice Factoring, Insurance, etc\) |
| RevokedOperator |  |
| setManager | Deployed On-Contracts, _Network Operations_ |
|  |  |



