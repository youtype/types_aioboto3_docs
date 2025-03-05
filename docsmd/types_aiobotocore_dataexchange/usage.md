# Examples

> [Index](../README.md) > [DataExchange](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#dataexchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dataexchange]` package installed.

Write your `DataExchange` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DataExchangeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("dataexchange") as client:  # (1)
    result = await client.accept_data_grant()  # (2)
```

1. client: [DataExchangeClient](./client.md)
2. result: [:material-code-braces: AcceptDataGrantResponseTypeDef](./type_defs.md#acceptdatagrantresponsetypedef)



#### Paginator usage example

```python
# ListDataGrantsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("dataexchange") as client:  # (1)
    paginator = client.get_paginator("list_data_grants")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataGrantsPaginator](./paginators.md#listdatagrantspaginator)
3. item: [:material-code-braces: ListDataGrantsResponseTypeDef](./type_defs.md#listdatagrantsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[dataexchange]`
or a standalone `types_aiobotocore_dataexchange` package, you have to explicitly specify
`client: DataExchangeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DataExchangeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.type_defs import AcceptDataGrantResponseTypeDef
from types_aiobotocore_dataexchange.type_defs import AcceptDataGrantRequestTypeDef


session = Session()

client: DataExchangeClient
async with session.client("dataexchange") as client:  # (1)
    kwargs: AcceptDataGrantRequestTypeDef = {...}  # (2)
    result: AcceptDataGrantResponseTypeDef = await client.accept_data_grant(**kwargs)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. kwargs: [:material-code-braces: AcceptDataGrantRequestTypeDef](./type_defs.md#acceptdatagrantrequesttypedef)
3. result: [:material-code-braces: AcceptDataGrantResponseTypeDef](./type_defs.md#acceptdatagrantresponsetypedef)



#### Paginator usage example

```python
# ListDataGrantsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dataexchange.client import DataExchangeClient
from types_aiobotocore_dataexchange.paginator import ListDataGrantsPaginator
from types_aiobotocore_dataexchange.type_defs import ListDataGrantsResponseTypeDef


session = Session()

client: DataExchangeClient
async with session.client("dataexchange") as client:  # (1)
    paginator: ListDataGrantsPaginator = client.get_paginator("list_data_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataGrantsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataExchangeClient](./client.md)
2. paginator: [ListDataGrantsPaginator](./paginators.md#listdatagrantspaginator)
3. item: [:material-code-braces: ListDataGrantsResponseTypeDef](./type_defs.md#listdatagrantsresponsetypedef)




