# Examples

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#managedblockchainquery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[managedblockchain-query]` package installed.

Write your `ManagedBlockchainQuery` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ManagedBlockchainQueryClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("managedblockchain-query") as client:  # (1)
    result = await client.batch_get_token_balance()  # (2)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. result: [:material-code-braces: BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef)



#### Paginator usage example

```python
# ListAssetContractsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("managedblockchain-query") as client:  # (1)
    paginator = client.get_paginator("list_asset_contracts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
3. item: [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[managedblockchain-query]`
or a standalone `types_aiobotocore_managedblockchain_query` package, you have to explicitly specify
`client: ManagedBlockchainQueryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ManagedBlockchainQueryClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient
from types_aiobotocore_managedblockchain_query.type_defs import BatchGetTokenBalanceOutputTypeDef
from types_aiobotocore_managedblockchain_query.type_defs import BatchGetTokenBalanceInputTypeDef


session = Session()

client: ManagedBlockchainQueryClient
async with session.client("managedblockchain-query") as client:  # (1)
    kwargs: BatchGetTokenBalanceInputTypeDef = {...}  # (2)
    result: BatchGetTokenBalanceOutputTypeDef = await client.batch_get_token_balance(**kwargs)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetTokenBalanceInputTypeDef](./type_defs.md#batchgettokenbalanceinputtypedef)
3. result: [:material-code-braces: BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef)



#### Paginator usage example

```python
# ListAssetContractsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient
from types_aiobotocore_managedblockchain_query.paginator import ListAssetContractsPaginator
from types_aiobotocore_managedblockchain_query.type_defs import ListAssetContractsOutputTypeDef


session = Session()

client: ManagedBlockchainQueryClient
async with session.client("managedblockchain-query") as client:  # (1)
    paginator: ListAssetContractsPaginator = client.get_paginator("list_asset_contracts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetContractsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
3. item: [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef)




