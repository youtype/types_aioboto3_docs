# Examples

> [Index](../README.md) > [ManagedGrafana](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[grafana]` package installed.

Write your `ManagedGrafana` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ManagedGrafanaClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("grafana") as client:  # (1)
    result = await client.associate_license()  # (2)
```

1. client: [ManagedGrafanaClient](./client.md)
2. result: [:material-code-braces: AssociateLicenseResponseTypeDef](./type_defs.md#associatelicenseresponsetypedef)



#### Paginator usage example

```python
# ListPermissionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("grafana") as client:  # (1)
    paginator = client.get_paginator("list_permissions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
3. item: [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[grafana]`
or a standalone `types_aiobotocore_grafana` package, you have to explicitly specify
`client: ManagedGrafanaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ManagedGrafanaClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_grafana.client import ManagedGrafanaClient
from types_aiobotocore_grafana.type_defs import AssociateLicenseResponseTypeDef
from types_aiobotocore_grafana.type_defs import AssociateLicenseRequestTypeDef


session = Session()

client: ManagedGrafanaClient
async with session.client("grafana") as client:  # (1)
    kwargs: AssociateLicenseRequestTypeDef = {...}  # (2)
    result: AssociateLicenseResponseTypeDef = await client.associate_license(**kwargs)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. kwargs: [:material-code-braces: AssociateLicenseRequestTypeDef](./type_defs.md#associatelicenserequesttypedef)
3. result: [:material-code-braces: AssociateLicenseResponseTypeDef](./type_defs.md#associatelicenseresponsetypedef)



#### Paginator usage example

```python
# ListPermissionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_grafana.client import ManagedGrafanaClient
from types_aiobotocore_grafana.paginator import ListPermissionsPaginator
from types_aiobotocore_grafana.type_defs import ListPermissionsResponseTypeDef


session = Session()

client: ManagedGrafanaClient
async with session.client("grafana") as client:  # (1)
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
3. item: [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)




