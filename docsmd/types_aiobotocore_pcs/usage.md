# Examples

> [Index](../README.md) > [ParallelComputingService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[pcs]` package installed.

Write your `ParallelComputingService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ParallelComputingServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("pcs") as client:  # (1)
    result = await client.create_cluster()  # (2)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)



#### Paginator usage example

```python
# ListClustersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("pcs") as client:  # (1)
    paginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[pcs]`
or a standalone `types_aiobotocore_pcs` package, you have to explicitly specify
`client: ParallelComputingServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ParallelComputingServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pcs.client import ParallelComputingServiceClient
from types_aiobotocore_pcs.type_defs import CreateClusterResponseTypeDef
from types_aiobotocore_pcs.type_defs import CreateClusterRequestTypeDef


session = Session()

client: ParallelComputingServiceClient
async with session.client("pcs") as client:  # (1)
    kwargs: CreateClusterRequestTypeDef = {...}  # (2)
    result: CreateClusterResponseTypeDef = await client.create_cluster(**kwargs)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. kwargs: [:material-code-braces: CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef)
3. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)



#### Paginator usage example

```python
# ListClustersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_pcs.client import ParallelComputingServiceClient
from types_aiobotocore_pcs.paginator import ListClustersPaginator
from types_aiobotocore_pcs.type_defs import ListClustersResponseTypeDef


session = Session()

client: ParallelComputingServiceClient
async with session.client("pcs") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)




