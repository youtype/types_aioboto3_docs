# Examples

> [Index](../README.md) > [IdentityStore](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#identitystore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[identitystore]` package installed.

Write your `IdentityStore` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IdentityStoreClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("identitystore") as client:  # (1)
    result = await client.create_group()  # (2)
```

1. client: [IdentityStoreClient](./client.md)
2. result: [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)



#### Paginator usage example

```python
# ListGroupMembershipsForMemberPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("identitystore") as client:  # (1)
    paginator = client.get_paginator("list_group_memberships_for_member")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListGroupMembershipsForMemberPaginator](./paginators.md#listgroupmembershipsformemberpaginator)
3. item: [:material-code-braces: ListGroupMembershipsForMemberResponseTypeDef](./type_defs.md#listgroupmembershipsformemberresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[identitystore]`
or a standalone `types_aiobotocore_identitystore` package, you have to explicitly specify
`client: IdentityStoreClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IdentityStoreClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_identitystore.client import IdentityStoreClient
from types_aiobotocore_identitystore.type_defs import CreateGroupResponseTypeDef
from types_aiobotocore_identitystore.type_defs import CreateGroupRequestTypeDef


session = Session()

client: IdentityStoreClient
async with session.client("identitystore") as client:  # (1)
    kwargs: CreateGroupRequestTypeDef = {...}  # (2)
    result: CreateGroupResponseTypeDef = await client.create_group(**kwargs)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. kwargs: [:material-code-braces: CreateGroupRequestTypeDef](./type_defs.md#creategrouprequesttypedef)
3. result: [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef)



#### Paginator usage example

```python
# ListGroupMembershipsForMemberPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_identitystore.client import IdentityStoreClient
from types_aiobotocore_identitystore.paginator import ListGroupMembershipsForMemberPaginator
from types_aiobotocore_identitystore.type_defs import ListGroupMembershipsForMemberResponseTypeDef


session = Session()

client: IdentityStoreClient
async with session.client("identitystore") as client:  # (1)
    paginator: ListGroupMembershipsForMemberPaginator = client.get_paginator("list_group_memberships_for_member")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupMembershipsForMemberResponseTypeDef
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListGroupMembershipsForMemberPaginator](./paginators.md#listgroupmembershipsformemberpaginator)
3. item: [:material-code-braces: ListGroupMembershipsForMemberResponseTypeDef](./type_defs.md#listgroupmembershipsformemberresponsetypedef)




