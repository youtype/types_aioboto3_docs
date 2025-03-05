# Examples

> [Index](../README.md) > [IAMRolesAnywhere](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#iamrolesanywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rolesanywhere]` package installed.

Write your `IAMRolesAnywhere` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IAMRolesAnywhereClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("rolesanywhere") as client:  # (1)
    result = await client.create_profile()  # (2)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. result: [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef)



#### Paginator usage example

```python
# ListCrlsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("rolesanywhere") as client:  # (1)
    paginator = client.get_paginator("list_crls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. paginator: [ListCrlsPaginator](./paginators.md#listcrlspaginator)
3. item: [:material-code-braces: ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[rolesanywhere]`
or a standalone `types_aiobotocore_rolesanywhere` package, you have to explicitly specify
`client: IAMRolesAnywhereClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IAMRolesAnywhereClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rolesanywhere.client import IAMRolesAnywhereClient
from types_aiobotocore_rolesanywhere.type_defs import ProfileDetailResponseTypeDef
from types_aiobotocore_rolesanywhere.type_defs import CreateProfileRequestTypeDef


session = Session()

client: IAMRolesAnywhereClient
async with session.client("rolesanywhere") as client:  # (1)
    kwargs: CreateProfileRequestTypeDef = {...}  # (2)
    result: ProfileDetailResponseTypeDef = await client.create_profile(**kwargs)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. kwargs: [:material-code-braces: CreateProfileRequestTypeDef](./type_defs.md#createprofilerequesttypedef)
3. result: [:material-code-braces: ProfileDetailResponseTypeDef](./type_defs.md#profiledetailresponsetypedef)



#### Paginator usage example

```python
# ListCrlsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_rolesanywhere.client import IAMRolesAnywhereClient
from types_aiobotocore_rolesanywhere.paginator import ListCrlsPaginator
from types_aiobotocore_rolesanywhere.type_defs import ListCrlsResponseTypeDef


session = Session()

client: IAMRolesAnywhereClient
async with session.client("rolesanywhere") as client:  # (1)
    paginator: ListCrlsPaginator = client.get_paginator("list_crls")  # (2)
    async for item in paginator.paginate(...):
        item: ListCrlsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. paginator: [ListCrlsPaginator](./paginators.md#listcrlspaginator)
3. item: [:material-code-braces: ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef)




