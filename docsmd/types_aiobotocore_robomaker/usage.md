# Examples

> [Index](../README.md) > [RoboMaker](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#robomaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[robomaker]` package installed.

Write your `RoboMaker` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# RoboMakerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("robomaker") as client:  # (1)
    result = await client.batch_delete_worlds()  # (2)
```

1. client: [RoboMakerClient](./client.md)
2. result: [:material-code-braces: BatchDeleteWorldsResponseTypeDef](./type_defs.md#batchdeleteworldsresponsetypedef)



#### Paginator usage example

```python
# ListDeploymentJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("robomaker") as client:  # (1)
    paginator = client.get_paginator("list_deployment_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
3. item: [:material-code-braces: ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[robomaker]`
or a standalone `types_aiobotocore_robomaker` package, you have to explicitly specify
`client: RoboMakerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# RoboMakerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_robomaker.client import RoboMakerClient
from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsResponseTypeDef
from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsRequestTypeDef


session = Session()

client: RoboMakerClient
async with session.client("robomaker") as client:  # (1)
    kwargs: BatchDeleteWorldsRequestTypeDef = {...}  # (2)
    result: BatchDeleteWorldsResponseTypeDef = await client.batch_delete_worlds(**kwargs)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteWorldsRequestTypeDef](./type_defs.md#batchdeleteworldsrequesttypedef)
3. result: [:material-code-braces: BatchDeleteWorldsResponseTypeDef](./type_defs.md#batchdeleteworldsresponsetypedef)



#### Paginator usage example

```python
# ListDeploymentJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_robomaker.client import RoboMakerClient
from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator
from types_aiobotocore_robomaker.type_defs import ListDeploymentJobsResponseTypeDef


session = Session()

client: RoboMakerClient
async with session.client("robomaker") as client:  # (1)
    paginator: ListDeploymentJobsPaginator = client.get_paginator("list_deployment_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
3. item: [:material-code-braces: ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef)




