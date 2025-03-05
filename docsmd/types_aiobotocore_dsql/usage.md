# Examples

> [Index](../README.md) > [AuroraDSQL](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dsql]` package installed.

Write your `AuroraDSQL` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AuroraDSQLClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("dsql") as client:  # (1)
    result = await client.create_cluster()  # (2)
```

1. client: [AuroraDSQLClient](./client.md)
2. result: [:material-code-braces: CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef)



#### Paginator usage example

```python
# ListClustersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("dsql") as client:  # (1)
    paginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AuroraDSQLClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef)



#### Waiter usage example

```python
# ClusterActiveWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("dsql") as client:  # (1)
    waiter = client.get_waiter("cluster_active")  # (2)
    await waiter.wait(...)
```

1. client: [AuroraDSQLClient](./client.md)
2. waiter: [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[dsql]`
or a standalone `types_aiobotocore_dsql` package, you have to explicitly specify
`client: AuroraDSQLClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AuroraDSQLClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dsql.client import AuroraDSQLClient
from types_aiobotocore_dsql.type_defs import CreateClusterOutputTypeDef
from types_aiobotocore_dsql.type_defs import CreateClusterInputTypeDef


session = Session()

client: AuroraDSQLClient
async with session.client("dsql") as client:  # (1)
    kwargs: CreateClusterInputTypeDef = {...}  # (2)
    result: CreateClusterOutputTypeDef = await client.create_cluster(**kwargs)  # (3)
```

1. client: [AuroraDSQLClient](./client.md)
2. kwargs: [:material-code-braces: CreateClusterInputTypeDef](./type_defs.md#createclusterinputtypedef)
3. result: [:material-code-braces: CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef)



#### Paginator usage example

```python
# ListClustersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dsql.client import AuroraDSQLClient
from types_aiobotocore_dsql.paginator import ListClustersPaginator
from types_aiobotocore_dsql.type_defs import ListClustersOutputTypeDef


session = Session()

client: AuroraDSQLClient
async with session.client("dsql") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [AuroraDSQLClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef)



#### Waiter usage example

```python
# ClusterActiveWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dsql.client import AuroraDSQLClient
from types_aiobotocore_dsql.waiter import ClusterActiveWaiter


session = Session()

async with session.client("dsql") as client:  # (1)
    waiter = client.get_waiter("cluster_active")  # (2)
    await waiter.wait(...)
```

1. client: [AuroraDSQLClient](./client.md)
2. waiter: [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)


