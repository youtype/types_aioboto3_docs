# Examples

> [Index](../README.md) > [ControlCatalog](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[controlcatalog]` package installed.

Write your `ControlCatalog` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ControlCatalogClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("controlcatalog") as client:  # (1)
    result = await client.get_control()  # (2)
```

1. client: [ControlCatalogClient](./client.md)
2. result: [:material-code-braces: GetControlResponseTypeDef](./type_defs.md#getcontrolresponsetypedef)



#### Paginator usage example

```python
# ListCommonControlsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("controlcatalog") as client:  # (1)
    paginator = client.get_paginator("list_common_controls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListCommonControlsPaginator](./paginators.md#listcommoncontrolspaginator)
3. item: [:material-code-braces: ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[controlcatalog]`
or a standalone `types_aiobotocore_controlcatalog` package, you have to explicitly specify
`client: ControlCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ControlCatalogClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_controlcatalog.client import ControlCatalogClient
from types_aiobotocore_controlcatalog.type_defs import GetControlResponseTypeDef
from types_aiobotocore_controlcatalog.type_defs import GetControlRequestTypeDef


session = Session()

client: ControlCatalogClient
async with session.client("controlcatalog") as client:  # (1)
    kwargs: GetControlRequestTypeDef = {...}  # (2)
    result: GetControlResponseTypeDef = await client.get_control(**kwargs)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. kwargs: [:material-code-braces: GetControlRequestTypeDef](./type_defs.md#getcontrolrequesttypedef)
3. result: [:material-code-braces: GetControlResponseTypeDef](./type_defs.md#getcontrolresponsetypedef)



#### Paginator usage example

```python
# ListCommonControlsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_controlcatalog.client import ControlCatalogClient
from types_aiobotocore_controlcatalog.paginator import ListCommonControlsPaginator
from types_aiobotocore_controlcatalog.type_defs import ListCommonControlsResponseTypeDef


session = Session()

client: ControlCatalogClient
async with session.client("controlcatalog") as client:  # (1)
    paginator: ListCommonControlsPaginator = client.get_paginator("list_common_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommonControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListCommonControlsPaginator](./paginators.md#listcommoncontrolspaginator)
3. item: [:material-code-braces: ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef)




