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

## 5.updateProxyAdminPropose

Change the address of the contract admin. This admin is the permission address of the upgrade contract. This method needs to be called only when you change the new management contract.

## 6.updateProxyUpgradPropose

Upgrade the logical contract of the corresponding contract

## 7.vote

Vote for the specified proposal. If the number of votes exceeds half of the nodes, the corresponding operation is performed.

## 8.votes

Multiple calls to method 7 above to complete multiple polls within a single transaction



