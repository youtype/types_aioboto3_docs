# Examples

> [Index](../README.md) > [WorkSpacesThinClient](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workspaces-thin-client]` package installed.

Write your `WorkSpacesThinClient` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# WorkSpacesThinClientClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("workspaces-thin-client") as client:  # (1)
    result = await client.create_environment()  # (2)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)



#### Paginator usage example

```python
# ListDevicesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("workspaces-thin-client") as client:  # (1)
    paginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[workspaces-thin-client]`
or a standalone `types_aiobotocore_workspaces_thin_client` package, you have to explicitly specify
`client: WorkSpacesThinClientClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# WorkSpacesThinClientClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient
from types_aiobotocore_workspaces_thin_client.type_defs import CreateEnvironmentResponseTypeDef
from types_aiobotocore_workspaces_thin_client.type_defs import CreateEnvironmentRequestTypeDef


session = Session()

client: WorkSpacesThinClientClient
async with session.client("workspaces-thin-client") as client:  # (1)
    kwargs: CreateEnvironmentRequestTypeDef = {...}  # (2)
    result: CreateEnvironmentResponseTypeDef = await client.create_environment(**kwargs)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. kwargs: [:material-code-braces: CreateEnvironmentRequestTypeDef](./type_defs.md#createenvironmentrequesttypedef)
3. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)



#### Paginator usage example

```python
# ListDevicesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient
from types_aiobotocore_workspaces_thin_client.paginator import ListDevicesPaginator
from types_aiobotocore_workspaces_thin_client.type_defs import ListDevicesResponseTypeDef


session = Session()

client: WorkSpacesThinClientClient
async with session.client("workspaces-thin-client") as client:  # (1)
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesThinClientClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)




