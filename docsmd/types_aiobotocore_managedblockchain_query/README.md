# ManagedBlockchainQuery module

> [Index](../README.md) > ManagedBlockchainQuery


!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#managedblockchainquery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `ManagedBlockchainQuery` service.
1. Use provided commands to install generated packages.



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
- [ListFilteredTransactionEventsPaginator](./paginators.md#listfilteredtransactioneventspaginator)
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
- [ListFilteredTransactionEventsPaginatorName](./literals.md#listfilteredtransactioneventspaginatorname)
- [ListFilteredTransactionEventsSortByType](./literals.md#listfilteredtransactioneventssortbytype)
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

- [AddressIdentifierFilterTypeDef](./type_defs.md#addressidentifierfiltertypedef)
- [ContractIdentifierTypeDef](./type_defs.md#contractidentifiertypedef)
- [BlockchainInstantOutputTypeDef](./type_defs.md#blockchaininstantoutputtypedef)
- [OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef)
- [TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef)
- [ContractFilterTypeDef](./type_defs.md#contractfiltertypedef)
- [ContractMetadataTypeDef](./type_defs.md#contractmetadatatypedef)
- [GetTransactionInputRequestTypeDef](./type_defs.md#gettransactioninputrequesttypedef)
- [TransactionTypeDef](./type_defs.md#transactiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListFilteredTransactionEventsSortTypeDef](./type_defs.md#listfilteredtransactioneventssorttypedef)
- [VoutFilterTypeDef](./type_defs.md#voutfiltertypedef)
- [OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef)
- [TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef)
- [ListTransactionEventsInputRequestTypeDef](./type_defs.md#listtransactioneventsinputrequesttypedef)
- [ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef)
- [TransactionOutputItemTypeDef](./type_defs.md#transactionoutputitemtypedef)
- [AssetContractTypeDef](./type_defs.md#assetcontracttypedef)
- [GetAssetContractInputRequestTypeDef](./type_defs.md#getassetcontractinputrequesttypedef)
- [TransactionEventTypeDef](./type_defs.md#transactioneventtypedef)
- [BatchGetTokenBalanceErrorItemTypeDef](./type_defs.md#batchgettokenbalanceerroritemtypedef)
- [BatchGetTokenBalanceOutputItemTypeDef](./type_defs.md#batchgettokenbalanceoutputitemtypedef)
- [TokenBalanceTypeDef](./type_defs.md#tokenbalancetypedef)
- [GetTokenBalanceOutputTypeDef](./type_defs.md#gettokenbalanceoutputtypedef)
- [BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef)
- [ListAssetContractsInputRequestTypeDef](./type_defs.md#listassetcontractsinputrequesttypedef)
- [GetAssetContractOutputTypeDef](./type_defs.md#getassetcontractoutputtypedef)
- [GetTransactionOutputTypeDef](./type_defs.md#gettransactionoutputtypedef)
- [ListAssetContractsInputPaginateTypeDef](./type_defs.md#listassetcontractsinputpaginatetypedef)
- [ListTransactionEventsInputPaginateTypeDef](./type_defs.md#listtransactioneventsinputpaginatetypedef)
- [ListTokenBalancesInputPaginateTypeDef](./type_defs.md#listtokenbalancesinputpaginatetypedef)
- [ListTokenBalancesInputRequestTypeDef](./type_defs.md#listtokenbalancesinputrequesttypedef)
- [ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef)
- [ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef)
- [ListFilteredTransactionEventsOutputTypeDef](./type_defs.md#listfilteredtransactioneventsoutputtypedef)
- [ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef)
- [BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef)
- [ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef)
- [BlockchainInstantUnionTypeDef](./type_defs.md#blockchaininstantuniontypedef)
- [GetTokenBalanceInputRequestTypeDef](./type_defs.md#gettokenbalanceinputrequesttypedef)
- [ListTransactionsInputPaginateTypeDef](./type_defs.md#listtransactionsinputpaginatetypedef)
- [ListTransactionsInputRequestTypeDef](./type_defs.md#listtransactionsinputrequesttypedef)
- [TimeFilterTypeDef](./type_defs.md#timefiltertypedef)
- [BatchGetTokenBalanceInputItemTypeDef](./type_defs.md#batchgettokenbalanceinputitemtypedef)
- [ListFilteredTransactionEventsInputPaginateTypeDef](./type_defs.md#listfilteredtransactioneventsinputpaginatetypedef)
- [ListFilteredTransactionEventsInputRequestTypeDef](./type_defs.md#listfilteredtransactioneventsinputrequesttypedef)
- [BatchGetTokenBalanceInputRequestTypeDef](./type_defs.md#batchgettokenbalanceinputrequesttypedef)
