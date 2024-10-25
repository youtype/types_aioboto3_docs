# Examples

> [Index](../README.md) > [ResourceExplorer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[resource-explorer-2]` package installed.

Write your `ResourceExplorer` code as usual,
type checking and code completion should work out of the box.



```python
# ResourceExplorerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("resource-explorer-2") as client:  # (1)
    result = await client.associate_default_view()  # (2)
```

1. client: [ResourceExplorerClient](./client.md)
2. result: [:material-code-braces: AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef) 



```python
# ListIndexesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("resource-explorer-2") as client:  # (1)
    paginator = client.get_paginator("list_indexes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesPaginator](./paginators.md#listindexespaginator)
3. item: [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[resource-explorer-2]`
or a standalone `types_aiobotocore_resource_explorer_2` package, you have to explicitly specify
`client: ResourceExplorerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ResourceExplorerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient
from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewOutputTypeDef
from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputRequestTypeDef


session = Session()

client: ResourceExplorerClient
async with session.client("resource-explorer-2") as client:  # (1)
    kwargs: AssociateDefaultViewInputRequestTypeDef = {...}  # (2)
    result: AssociateDefaultViewOutputTypeDef = await client.associate_default_view(**kwargs)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. kwargs: [:material-code-braces: AssociateDefaultViewInputRequestTypeDef](./type_defs.md#associatedefaultviewinputrequesttypedef) 
3. result: [:material-code-braces: AssociateDefaultViewOutputTypeDef](./type_defs.md#associatedefaultviewoutputtypedef) 



```python
# ListIndexesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_resource_explorer_2.client import ResourceExplorerClient
from types_aiobotocore_resource_explorer_2.paginator import ListIndexesPaginator
from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesOutputTypeDef


session = Session()

client: ResourceExplorerClient
async with session.client("resource-explorer-2") as client:  # (1)
    paginator: ListIndexesPaginator = client.get_paginator("list_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceExplorerClient](./client.md)
2. paginator: [ListIndexesPaginator](./paginators.md#listindexespaginator)
3. item: [:material-code-braces: ListIndexesOutputTypeDef](./type_defs.md#listindexesoutputtypedef) 




