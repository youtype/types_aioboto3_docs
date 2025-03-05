# Examples

> [Index](../README.md) > [AppFabric](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#appfabric)
    type annotations stubs module [types-aiobotocore-appfabric](https://pypi.org/project/types-aiobotocore-appfabric/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appfabric]` package installed.

Write your `AppFabric` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AppFabricClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("appfabric") as client:  # (1)
    result = await client.batch_get_user_access_tasks()  # (2)
```

1. client: [AppFabricClient](./client.md)
2. result: [:material-code-braces: BatchGetUserAccessTasksResponseTypeDef](./type_defs.md#batchgetuseraccesstasksresponsetypedef)



#### Paginator usage example

```python
# ListAppAuthorizationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("appfabric") as client:  # (1)
    paginator = client.get_paginator("list_app_authorizations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListAppAuthorizationsPaginator](./paginators.md#listappauthorizationspaginator)
3. item: [:material-code-braces: ListAppAuthorizationsResponseTypeDef](./type_defs.md#listappauthorizationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[appfabric]`
or a standalone `types_aiobotocore_appfabric` package, you have to explicitly specify
`client: AppFabricClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AppFabricClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appfabric.client import AppFabricClient
from types_aiobotocore_appfabric.type_defs import BatchGetUserAccessTasksResponseTypeDef
from types_aiobotocore_appfabric.type_defs import BatchGetUserAccessTasksRequestTypeDef


session = Session()

client: AppFabricClient
async with session.client("appfabric") as client:  # (1)
    kwargs: BatchGetUserAccessTasksRequestTypeDef = {...}  # (2)
    result: BatchGetUserAccessTasksResponseTypeDef = await client.batch_get_user_access_tasks(**kwargs)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetUserAccessTasksRequestTypeDef](./type_defs.md#batchgetuseraccesstasksrequesttypedef)
3. result: [:material-code-braces: BatchGetUserAccessTasksResponseTypeDef](./type_defs.md#batchgetuseraccesstasksresponsetypedef)



#### Paginator usage example

```python
# ListAppAuthorizationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appfabric.client import AppFabricClient
from types_aiobotocore_appfabric.paginator import ListAppAuthorizationsPaginator
from types_aiobotocore_appfabric.type_defs import ListAppAuthorizationsResponseTypeDef


session = Session()

client: AppFabricClient
async with session.client("appfabric") as client:  # (1)
    paginator: ListAppAuthorizationsPaginator = client.get_paginator("list_app_authorizations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppAuthorizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AppFabricClient](./client.md)
2. paginator: [ListAppAuthorizationsPaginator](./paginators.md#listappauthorizationspaginator)
3. item: [:material-code-braces: ListAppAuthorizationsResponseTypeDef](./type_defs.md#listappauthorizationsresponsetypedef)




