# Examples

> [Index](../README.md) > [Finspace](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[finspace]` package installed.

Write your `Finspace` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# FinspaceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("finspace") as client:  # (1)
    result = await client.create_environment()  # (2)
```

1. client: [FinspaceClient](./client.md)
2. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)



#### Paginator usage example

```python
# ListKxEnvironmentsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("finspace") as client:  # (1)
    paginator = client.get_paginator("list_kx_environments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FinspaceClient](./client.md)
2. paginator: [ListKxEnvironmentsPaginator](./paginators.md#listkxenvironmentspaginator)
3. item: [:material-code-braces: ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[finspace]`
or a standalone `types_aiobotocore_finspace` package, you have to explicitly specify
`client: FinspaceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# FinspaceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_finspace.client import FinspaceClient
from types_aiobotocore_finspace.type_defs import CreateEnvironmentResponseTypeDef
from types_aiobotocore_finspace.type_defs import CreateEnvironmentRequestTypeDef


session = Session()

client: FinspaceClient
async with session.client("finspace") as client:  # (1)
    kwargs: CreateEnvironmentRequestTypeDef = {...}  # (2)
    result: CreateEnvironmentResponseTypeDef = await client.create_environment(**kwargs)  # (3)
```

1. client: [FinspaceClient](./client.md)
2. kwargs: [:material-code-braces: CreateEnvironmentRequestTypeDef](./type_defs.md#createenvironmentrequesttypedef)
3. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)



#### Paginator usage example

```python
# ListKxEnvironmentsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_finspace.client import FinspaceClient
from types_aiobotocore_finspace.paginator import ListKxEnvironmentsPaginator
from types_aiobotocore_finspace.type_defs import ListKxEnvironmentsResponseTypeDef


session = Session()

client: FinspaceClient
async with session.client("finspace") as client:  # (1)
    paginator: ListKxEnvironmentsPaginator = client.get_paginator("list_kx_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListKxEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinspaceClient](./client.md)
2. paginator: [ListKxEnvironmentsPaginator](./paginators.md#listkxenvironmentspaginator)
3. item: [:material-code-braces: ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef)




