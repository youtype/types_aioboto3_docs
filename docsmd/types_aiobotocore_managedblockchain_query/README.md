# ManagedBlockchainQuery module

> [Index](../README.md) > ManagedBlockchainQuery


!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `ManagedBlockchainQuery` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[managedblockchain-query]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[managedblockchain-query]'


# standalone installation
python -m pip install types-aiobotocore-managedblockchain-query
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-managedblockchain-query
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ManagedBlockchainQueryClient

Type annotations and code completion for  `#!python session.client("managedblockchain-query")` as [ManagedBlockchainQueryClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# ManagedBlockchainQueryClient usage example

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient


session = Session()
async with session.client("managedblockchain-query") as client:
    client: ManagedBlockchainQueryClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("managedblockchain-query").get_paginator("...")`.

```python
# ListAssetContractsPaginator usage example

from types_aiobotocore_managedblockchain_query.paginator import ListAssetContractsPaginator

def get_list_asset_contracts_paginator() -> ListAssetContractsPaginator:
    return client.get_paginator("list_asset_contracts"))
```

- [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
- [ListTokenBalancesPaginator](./paginators.md#listtokenbalancespaginator)
- [ListTransactionEventsPaginator](./paginators.md#listtransactioneventspaginator)
- [ListTransactionsPaginator](./paginators.md#listtransactionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConfirmationStatusType usage example

from types_aiobotocore_managedblockchain_query.literals import ConfirmationStatusType

def get_value() -> ConfirmationStatusType:
    return "FINAL"
```

- [ConfirmationStatusType](./literals.md#confirmationstatustype)
- [ErrorTypeType](./literals.md#errortypetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [ListAssetContractsPaginatorName](./literals.md#listassetcontractspaginatorname)
- [ListTokenBalancesPaginatorName](./literals.md#listtokenbalancespaginatorname)
- [ListTransactionEventsPaginatorName](./literals.md#listtransactioneventspaginatorname)
- [ListTransactionsPaginatorName](./literals.md#listtransactionspaginatorname)
- [ListTransactionsSortByType](./literals.md#listtransactionssortbytype)
- [QueryNetworkType](./literals.md#querynetworktype)
- [QueryTokenStandardType](./literals.md#querytokenstandardtype)
- [QueryTransactionEventTypeType](./literals.md#querytransactioneventtypetype)
- [SortOrderType](./literals.md#sortordertype)
- [ManagedBlockchainQueryServiceName](./literals.md#managedblockchainqueryservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ContractIdentifierTypeDef](./type_defs.md#contractidentifiertypedef)
- [OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef)
- [TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef)
- [ContractFilterTypeDef](./type_defs.md#contractfiltertypedef)
- [ContractMetadataTypeDef](./type_defs.md#contractmetadatatypedef)
- [GetTransactionInputRequestTypeDef](./type_defs.md#gettransactioninputrequesttypedef)
- [TransactionTypeDef](./type_defs.md#transactiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef)
- [TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef)
- [ListTransactionEventsInputRequestTypeDef](./type_defs.md#listtransactioneventsinputrequesttypedef)
- [TransactionEventTypeDef](./type_defs.md#transactioneventtypedef)
- [ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef)
- [TransactionOutputItemTypeDef](./type_defs.md#transactionoutputitemtypedef)
- [AssetContractTypeDef](./type_defs.md#assetcontracttypedef)
- [GetAssetContractInputRequestTypeDef](./type_defs.md#getassetcontractinputrequesttypedef)
- [TokenBalancePaginatorTypeDef](./type_defs.md#tokenbalancepaginatortypedef)
- [BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef)
- [ListAssetContractsInputRequestTypeDef](./type_defs.md#listassetcontractsinputrequesttypedef)
- [GetAssetContractOutputTypeDef](./type_defs.md#getassetcontractoutputtypedef)
- [GetTransactionOutputTypeDef](./type_defs.md#gettransactionoutputtypedef)
- [ListAssetContractsInputListAssetContractsPaginateTypeDef](./type_defs.md#listassetcontractsinputlistassetcontractspaginatetypedef)
- [ListTransactionEventsInputListTransactionEventsPaginateTypeDef](./type_defs.md#listtransactioneventsinputlisttransactioneventspaginatetypedef)
- [ListTokenBalancesInputListTokenBalancesPaginateTypeDef](./type_defs.md#listtokenbalancesinputlisttokenbalancespaginatetypedef)
- [ListTokenBalancesInputRequestTypeDef](./type_defs.md#listtokenbalancesinputrequesttypedef)
- [ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef)
- [ListTransactionsInputListTransactionsPaginateTypeDef](./type_defs.md#listtransactionsinputlisttransactionspaginatetypedef)
- [ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef)
- [ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef)
- [ListTokenBalancesOutputPaginatorTypeDef](./type_defs.md#listtokenbalancesoutputpaginatortypedef)
- [BatchGetTokenBalanceErrorItemTypeDef](./type_defs.md#batchgettokenbalanceerroritemtypedef)
- [BatchGetTokenBalanceInputItemTypeDef](./type_defs.md#batchgettokenbalanceinputitemtypedef)
- [BatchGetTokenBalanceOutputItemTypeDef](./type_defs.md#batchgettokenbalanceoutputitemtypedef)
- [GetTokenBalanceInputRequestTypeDef](./type_defs.md#gettokenbalanceinputrequesttypedef)
- [GetTokenBalanceOutputTypeDef](./type_defs.md#gettokenbalanceoutputtypedef)
- [ListTransactionsInputRequestTypeDef](./type_defs.md#listtransactionsinputrequesttypedef)
- [TokenBalanceTypeDef](./type_defs.md#tokenbalancetypedef)
- [BatchGetTokenBalanceInputRequestTypeDef](./type_defs.md#batchgettokenbalanceinputrequesttypedef)
- [BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef)
- [ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef)

