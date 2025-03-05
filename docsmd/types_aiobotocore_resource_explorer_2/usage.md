# Examples

> [Index](../README.md) > [ResourceExplorer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[resource-explorer-2]` package installed.

Write your `ResourceExplorer` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ResourceExplorerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("resource-explorer-2") as client:  # (1)
    result = await client.associate_default_view()  # (2)
```

1. client: [ResourceExplorerClient](./client.md)
2. result: [:material-code-braces: AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef)



#### Paginator usage example

```python
# ListIndexesForMembersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("resource-explorer-2") as client:  # (1)
    paginator = client.get_paginator("list_indexes_for_members")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesForMembersPaginator](./paginators.md#listindexesformemberspaginator)
3. item: [:material-code-braces: ListIndexesForMembersOutputTypeDef](./type_defs.md#listindexesformembersoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[resource-explorer-2]`
or a standalone `types_aiobotocore_resource_explorer_2` package, you have to explicitly specify
`client: ResourceExplorerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ResourceExplorerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient
from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewOutputTypeDef
from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputTypeDef


session = Session()

client: ResourceExplorerClient
async with session.client("resource-explorer-2") as client:  # (1)
    kwargs: AssociateDefaultViewInputTypeDef = {...}  # (2)
    result: AssociateDefaultViewOutputTypeDef = await client.associate_default_view(**kwargs)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. kwargs: [:material-code-braces: AssociateDefaultViewInputTypeDef](./type_defs.md#associatedefaultviewinputtypedef)
3. result: [:material-code-braces: AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef)



#### Paginator usage example

```python
# ListIndexesForMembersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient
from types_aiobotocore_resource_explorer_2.paginator import ListIndexesForMembersPaginator
from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesForMembersOutputTypeDef


session = Session()

client: ResourceExplorerClient
async with session.client("resource-explorer-2") as client:  # (1)
    paginator: ListIndexesForMembersPaginator = client.get_paginator("list_indexes_for_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesForMembersOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesForMembersPaginator](./paginators.md#listindexesformemberspaginator)
3. item: [:material-code-braces: ListIndexesForMembersOutputTypeDef](./type_defs.md#listindexesformembersoutputtypedef)




