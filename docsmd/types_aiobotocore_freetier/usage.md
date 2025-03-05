# Examples

> [Index](../README.md) > [FreeTier](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[freetier]` package installed.

Write your `FreeTier` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# FreeTierClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("freetier") as client:  # (1)
    result = await client.get_free_tier_usage()  # (2)
```

1. client: [FreeTierClient](./client.md)
2. result: [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef)



#### Paginator usage example

```python
# GetFreeTierUsagePaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("freetier") as client:  # (1)
    paginator = client.get_paginator("get_free_tier_usage")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FreeTierClient](./client.md)
2. paginator: [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)
3. item: [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[freetier]`
or a standalone `types_aiobotocore_freetier` package, you have to explicitly specify
`client: FreeTierClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# FreeTierClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_freetier.client import FreeTierClient
from types_aiobotocore_freetier.type_defs import GetFreeTierUsageResponseTypeDef
from types_aiobotocore_freetier.type_defs import GetFreeTierUsageRequestTypeDef


session = Session()

client: FreeTierClient
async with session.client("freetier") as client:  # (1)
    kwargs: GetFreeTierUsageRequestTypeDef = {...}  # (2)
    result: GetFreeTierUsageResponseTypeDef = await client.get_free_tier_usage(**kwargs)  # (3)
```

1. client: [FreeTierClient](./client.md)
2. kwargs: [:material-code-braces: GetFreeTierUsageRequestTypeDef](./type_defs.md#getfreetierusagerequesttypedef)
3. result: [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef)



#### Paginator usage example

```python
# GetFreeTierUsagePaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_freetier.client import FreeTierClient
from types_aiobotocore_freetier.paginator import GetFreeTierUsagePaginator
from types_aiobotocore_freetier.type_defs import GetFreeTierUsageResponseTypeDef


session = Session()

client: FreeTierClient
async with session.client("freetier") as client:  # (1)
    paginator: GetFreeTierUsagePaginator = client.get_paginator("get_free_tier_usage")  # (2)
    async for item in paginator.paginate(...):
        item: GetFreeTierUsageResponseTypeDef
        print(item)  # (3)
```

1. client: [FreeTierClient](./client.md)
2. paginator: [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)
3. item: [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef)




