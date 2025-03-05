# Examples

> [Index](../README.md) > [MailManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mailmanager]` package installed.

Write your `MailManager` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MailManagerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("mailmanager") as client:  # (1)
    result = await client.create_addon_instance()  # (2)
```

1. client: [MailManagerClient](./client.md)
2. result: [:material-code-braces: CreateAddonInstanceResponseTypeDef](./type_defs.md#createaddoninstanceresponsetypedef)



#### Paginator usage example

```python
# ListAddonInstancesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("mailmanager") as client:  # (1)
    paginator = client.get_paginator("list_addon_instances")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddonInstancesPaginator](./paginators.md#listaddoninstancespaginator)
3. item: [:material-code-braces: ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[mailmanager]`
or a standalone `types_aiobotocore_mailmanager` package, you have to explicitly specify
`client: MailManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MailManagerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mailmanager.client import MailManagerClient
from types_aiobotocore_mailmanager.type_defs import CreateAddonInstanceResponseTypeDef
from types_aiobotocore_mailmanager.type_defs import CreateAddonInstanceRequestTypeDef


session = Session()

client: MailManagerClient
async with session.client("mailmanager") as client:  # (1)
    kwargs: CreateAddonInstanceRequestTypeDef = {...}  # (2)
    result: CreateAddonInstanceResponseTypeDef = await client.create_addon_instance(**kwargs)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. kwargs: [:material-code-braces: CreateAddonInstanceRequestTypeDef](./type_defs.md#createaddoninstancerequesttypedef)
3. result: [:material-code-braces: CreateAddonInstanceResponseTypeDef](./type_defs.md#createaddoninstanceresponsetypedef)



#### Paginator usage example

```python
# ListAddonInstancesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mailmanager.client import MailManagerClient
from types_aiobotocore_mailmanager.paginator import ListAddonInstancesPaginator
from types_aiobotocore_mailmanager.type_defs import ListAddonInstancesResponseTypeDef


session = Session()

client: MailManagerClient
async with session.client("mailmanager") as client:  # (1)
    paginator: ListAddonInstancesPaginator = client.get_paginator("list_addon_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListAddonInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [MailManagerClient](./client.md)
2. paginator: [ListAddonInstancesPaginator](./paginators.md#listaddoninstancespaginator)
3. item: [:material-code-braces: ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef)




