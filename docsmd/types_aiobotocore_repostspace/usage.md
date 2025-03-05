# Examples

> [Index](../README.md) > [RePostPrivate](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[repostspace]` package installed.

Write your `RePostPrivate` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# RePostPrivateClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("repostspace") as client:  # (1)
    result = await client.batch_add_role()  # (2)
```

1. client: [RePostPrivateClient](./client.md)
2. result: [:material-code-braces: BatchAddRoleOutputTypeDef](./type_defs.md#batchaddroleoutputtypedef)



#### Paginator usage example

```python
# ListSpacesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("repostspace") as client:  # (1)
    paginator = client.get_paginator("list_spaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RePostPrivateClient](./client.md)
2. paginator: [ListSpacesPaginator](./paginators.md#listspacespaginator)
3. item: [:material-code-braces: ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[repostspace]`
or a standalone `types_aiobotocore_repostspace` package, you have to explicitly specify
`client: RePostPrivateClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# RePostPrivateClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.type_defs import BatchAddRoleOutputTypeDef
from types_aiobotocore_repostspace.type_defs import BatchAddRoleInputTypeDef


session = Session()

client: RePostPrivateClient
async with session.client("repostspace") as client:  # (1)
    kwargs: BatchAddRoleInputTypeDef = {...}  # (2)
    result: BatchAddRoleOutputTypeDef = await client.batch_add_role(**kwargs)  # (3)
```

1. client: [RePostPrivateClient](./client.md)
2. kwargs: [:material-code-braces: BatchAddRoleInputTypeDef](./type_defs.md#batchaddroleinputtypedef)
3. result: [:material-code-braces: BatchAddRoleOutputTypeDef](./type_defs.md#batchaddroleoutputtypedef)



#### Paginator usage example

```python
# ListSpacesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_repostspace.client import RePostPrivateClient
from types_aiobotocore_repostspace.paginator import ListSpacesPaginator
from types_aiobotocore_repostspace.type_defs import ListSpacesOutputTypeDef


session = Session()

client: RePostPrivateClient
async with session.client("repostspace") as client:  # (1)
    paginator: ListSpacesPaginator = client.get_paginator("list_spaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListSpacesOutputTypeDef
        print(item)  # (3)
```

1. client: [RePostPrivateClient](./client.md)
2. paginator: [ListSpacesPaginator](./paginators.md#listspacespaginator)
3. item: [:material-code-braces: ListSpacesOutputTypeDef](./type_defs.md#listspacesoutputtypedef)




