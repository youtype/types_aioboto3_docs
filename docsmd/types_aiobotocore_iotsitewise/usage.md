# Examples

> [Index](../README.md) > [IoTSiteWise](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotsitewise]` package installed.

Write your `IoTSiteWise` code as usual,
type checking and code completion should work out of the box.



```python
# IoTSiteWiseClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotsitewise") as client:  # (1)
    result = await client.associate_assets()  # (2)
```

1. client: [IoTSiteWiseClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ExecuteQueryPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotsitewise") as client:  # (1)
    paginator = client.get_paginator("execute_query")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ExecuteQueryPaginator](./paginators.md#executequerypaginator)
3. item: [:material-code-braces: ExecuteQueryResponsePaginatorTypeDef](./type_defs.md#executequeryresponsepaginatortypedef) 



```python
# AssetActiveWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotsitewise") as client:  # (1)
    waiter = client.get_waiter("asset_active")  # (2)
    await waiter.wait()
```

1. client: [IoTSiteWiseClient](./client.md)
2. waiter: [AssetActiveWaiter](./waiters.md#assetactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[iotsitewise]`
or a standalone `types_aiobotocore_iotsitewise` package, you have to explicitly specify
`client: IoTSiteWiseClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTSiteWiseClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient
from types_aiobotocore_iotsitewise.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_iotsitewise.type_defs import AssociateAssetsRequestRequestTypeDef


session = Session()

client: IoTSiteWiseClient
async with session.client("iotsitewise") as client:  # (1)
    kwargs: AssociateAssetsRequestRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.associate_assets(**kwargs)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. kwargs: [:material-code-braces: AssociateAssetsRequestRequestTypeDef](./type_defs.md#associateassetsrequestrequesttypedef) 
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ExecuteQueryPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient
from types_aiobotocore_iotsitewise.paginator import ExecuteQueryPaginator
from types_aiobotocore_iotsitewise.type_defs import ExecuteQueryResponsePaginatorTypeDef


session = Session()

client: IoTSiteWiseClient
async with session.client("iotsitewise") as client:  # (1)
    paginator: ExecuteQueryPaginator = client.get_paginator("execute_query")  # (2)
    async for item in paginator.paginate(...):
        item: ExecuteQueryResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ExecuteQueryPaginator](./paginators.md#executequerypaginator)
3. item: [:material-code-braces: ExecuteQueryResponsePaginatorTypeDef](./type_defs.md#executequeryresponsepaginatortypedef) 



```python
# AssetActiveWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotsitewise.client import IoTSiteWiseClient
from types_aiobotocore_iotsitewise.waiter import AssetActiveWaiter


session = Session()

async with session.client("iotsitewise") as client:  # (1)
    waiter = client.get_waiter("asset_active")  # (2)
    await waiter.wait()
```

1. client: [IoTSiteWiseClient](./client.md)
2. waiter: [AssetActiveWaiter](./waiters.md#assetactivewaiter)

