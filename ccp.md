## The Clearing House Process

source: DAML Github

| **1. The scenario**Two parties want to transact a repo trade. | [![](https://github.com/digital-asset/ex-repo-market/raw/master/docs/img/scenario.png "img/scenario.png")](https://github.com/digital-asset/ex-repo-market/blob/master/docs/img/scenario.png) |
| :--- | :--- |
| **2. Novation**The clearing house becomes a central counterparty for the trading partners: that is, it**novates**the trade, turning a single trade into two trades with a central counterparty. | [![](https://github.com/digital-asset/ex-repo-market/raw/master/docs/img/novation.png "img/novation.png")](https://github.com/digital-asset/ex-repo-market/blob/master/docs/img/novation.png) |
| **3. Transfer**The clearing house takes ownership of collateral from both parties. | [![](https://github.com/digital-asset/ex-repo-market/raw/master/docs/img/transfer.png "img/transfer.png")](https://github.com/digital-asset/ex-repo-market/blob/master/docs/img/transfer.png) |
| **4. Grouping**Rather than executing transfers individually, the clearing house groups them based on:counterpartysettlement datesecurity CUSIP \(an identifier for financial instruments\)currency |  |
| **5. Netting**The clearing house bundles the grouped trades into Net Broker Obligations: this is called**netting**.It uses these to create Delivery versus Payment contracts that reflect the net trades of each trading party and their obligations to the clearing house. | [![](https://github.com/digital-asset/ex-repo-market/raw/master/docs/img/netting.png "img/netting.png")](https://github.com/digital-asset/ex-repo-market/blob/master/docs/img/netting.png) |
| **6. Settling**Finally, according to these obligations, collateral is transferred to and from the clearing house. This**settles**all trades. | [![](https://github.com/digital-asset/ex-repo-market/raw/master/docs/img/settling.png "img/settling.png")](https://github.com/digital-asset/ex-repo-market/blob/master/docs/img/settling.png) |



