# netmind-proposal

management proposal and update

Management Contract Method Invocation Description：

## 1.addNodePropose

For proposals that add node addresses, only the added node addresses have the right to propose and vote.

## 2.deleteNodePropose

Delete the node address proposal, the deleted node address will no longer have the power of proposal and voting.

## 3.excContractPropose

A proposal to perform a contract operation, used to call the relevant methods of the corresponding contract

## 4.excContractProposes

Multiple calls to method 3 above can be done in a single transaction

## 5.updateAdminOwnerPropose

Change the address with the permission of the TransparentProxy contract owner. This owner is the address with the permission to upgrade the contract. This method should only be called when you change to a new management contract.

## 6.updateTransparentProxyAdminPropose

Propose to change the ProxyAdmin of the contract

## 7.updateTransparentProxyUpgradPropose

Upgrade the logical contract of the corresponding contract

## 8.vote

Vote for the specified proposal. If the number of votes exceeds half of the nodes, the corresponding operation is performed.

## 9.votes

Multiple calls to method 7 above to complete multiple polls within a single transaction


