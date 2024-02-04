# Examples

> [Index](../README.md) > [QuickSight](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[quicksight]` package installed.

Write your `QuickSight` code as usual,
type checking and code completion should work out of the box.



```python
# QuickSightClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("quicksight") as client:  # (1)
    result = await client.cancel_ingestion()  # (2)
```

1. client: [QuickSightClient](./client.md)
2. result: [:material-code-braces: CancelIngestionResponseTypeDef](./type_defs.md#cancelingestionresponsetypedef) 



```python
# DescribeFolderPermissionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("quicksight") as client:  # (1)
    paginator = client.get_paginator("describe_folder_permissions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [DescribeFolderPermissionsPaginator](./paginators.md#describefolderpermissionspaginator)
3. item: [:material-code-braces: DescribeFolderPermissionsResponsePaginatorTypeDef](./type_defs.md#describefolderpermissionsresponsepaginatortypedef) 




### Explicit type annotations

With `types-aioboto3-lite[quicksight]`
or a standalone `types_aiobotocore_quicksight` package, you have to explicitly specify
`client: QuickSightClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QuickSightClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_quicksight.client import QuickSightClient
from types_aiobotocore_quicksight.type_defs import CancelIngestionResponseTypeDef
from types_aiobotocore_quicksight.type_defs import CancelIngestionRequestRequestTypeDef


session = Session()

client: QuickSightClient
async with session.client("quicksight") as client:  # (1)
    kwargs: CancelIngestionRequestRequestTypeDef = {...}  # (2)
    result: CancelIngestionResponseTypeDef = await client.cancel_ingestion(**kwargs)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. kwargs: [:material-code-braces: CancelIngestionRequestRequestTypeDef](./type_defs.md#cancelingestionrequestrequesttypedef) 
3. result: [:material-code-braces: CancelIngestionResponseTypeDef](./type_defs.md#cancelingestionresponsetypedef) 



```python
# DescribeFolderPermissionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_quicksight.client import QuickSightClient
from types_aiobotocore_quicksight.paginator import DescribeFolderPermissionsPaginator
from types_aiobotocore_quicksight.type_defs import DescribeFolderPermissionsResponsePaginatorTypeDef


session = Session()

client: QuickSightClient
async with session.client("quicksight") as client:  # (1)
    paginator: DescribeFolderPermissionsPaginator = client.get_paginator("describe_folder_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFolderPermissionsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [QuickSightClient](./client.md)
2. paginator: [DescribeFolderPermissionsPaginator](./paginators.md#describefolderpermissionspaginator)
3. item: [:material-code-braces: DescribeFolderPermissionsResponsePaginatorTypeDef](./type_defs.md#describefolderpermissionsresponsepaginatortypedef) 




