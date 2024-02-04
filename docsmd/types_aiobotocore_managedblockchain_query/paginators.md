# Paginators

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## ListAssetContractsPaginator

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_paginator("list_asset_contracts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListAssetContracts)

```python
# ListAssetContractsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.paginator import ListAssetContractsPaginator

session = Session()

session = get_session()
async with session.client("managedblockchain-query") as client:  # (1)
    paginator: ListAssetContractsPaginator = client.get_paginator("list_asset_contracts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetContractsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
3. item: [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetContractsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    contractFilter: ContractFilterTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAssetContractsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ContractFilterTypeDef](./type_defs.md#contractfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetContractsInputListAssetContractsPaginateTypeDef = {  # (1)
    "contractFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetContractsInputListAssetContractsPaginateTypeDef](./type_defs.md#listassetcontractsinputlistassetcontractspaginatetypedef) 
## ListTokenBalancesPaginator

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_paginator("list_token_balances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTokenBalances)

```python
# ListTokenBalancesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.paginator import ListTokenBalancesPaginator

session = Session()

session = get_session()
async with session.client("managedblockchain-query") as client:  # (1)
    paginator: ListTokenBalancesPaginator = client.get_paginator("list_token_balances")  # (2)
    async for item in paginator.paginate(...):
        item: ListTokenBalancesOutputPaginatorTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListTokenBalancesPaginator](./paginators.md#listtokenbalancespaginator)
3. item: [:material-code-braces: ListTokenBalancesOutputPaginatorTypeDef](./type_defs.md#listtokenbalancesoutputpaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListTokenBalancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    tokenFilter: TokenFilterTypeDef,  # (1)
    ownerFilter: OwnerFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListTokenBalancesOutputPaginatorTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef) 
2. See [:material-code-braces: OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListTokenBalancesOutputPaginatorTypeDef](./type_defs.md#listtokenbalancesoutputpaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTokenBalancesInputListTokenBalancesPaginateTypeDef = {  # (1)
    "tokenFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTokenBalancesInputListTokenBalancesPaginateTypeDef](./type_defs.md#listtokenbalancesinputlisttokenbalancespaginatetypedef) 
## ListTransactionEventsPaginator

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_paginator("list_transaction_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactionEvents)

```python
# ListTransactionEventsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.paginator import ListTransactionEventsPaginator

session = Session()

session = get_session()
async with session.client("managedblockchain-query") as client:  # (1)
    paginator: ListTransactionEventsPaginator = client.get_paginator("list_transaction_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListTransactionEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListTransactionEventsPaginator](./paginators.md#listtransactioneventspaginator)
3. item: [:material-code-braces: ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTransactionEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    transactionHash: str,
    network: QueryNetworkType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListTransactionEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTransactionEventsInputListTransactionEventsPaginateTypeDef = {  # (1)
    "transactionHash": ...,
    "network": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTransactionEventsInputListTransactionEventsPaginateTypeDef](./type_defs.md#listtransactioneventsinputlisttransactioneventspaginatetypedef) 
## ListTransactionsPaginator

Type annotations and code completion for `#!python session.client("managedblockchain-query").get_paginator("list_transactions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Paginator.ListTransactions)

```python
# ListTransactionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.paginator import ListTransactionsPaginator

session = Session()

session = get_session()
async with session.client("managedblockchain-query") as client:  # (1)
    paginator: ListTransactionsPaginator = client.get_paginator("list_transactions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTransactionsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListTransactionsPaginator](./paginators.md#listtransactionspaginator)
3. item: [:material-code-braces: ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTransactionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    address: str,
    network: QueryNetworkType,  # (1)
    fromBlockchainInstant: BlockchainInstantPaginatorTypeDef = ...,  # (2)
    toBlockchainInstant: BlockchainInstantPaginatorTypeDef = ...,  # (2)
    sort: ListTransactionsSortTypeDef = ...,  # (4)
    confirmationStatusFilter: ConfirmationStatusFilterTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AsyncIterator[ListTransactionsOutputTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef) 
3. See [:material-code-braces: BlockchainInstantPaginatorTypeDef](./type_defs.md#blockchaininstantpaginatortypedef) 
4. See [:material-code-braces: ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef) 
5. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTransactionsInputListTransactionsPaginateTypeDef = {  # (1)
    "address": ...,
    "network": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTransactionsInputListTransactionsPaginateTypeDef](./type_defs.md#listtransactionsinputlisttransactionspaginatetypedef) 
