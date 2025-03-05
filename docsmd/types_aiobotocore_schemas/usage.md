# Examples

> [Index](../README.md) > [Schemas](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#schemas)
    type annotations stubs module [types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[schemas]` package installed.

Write your `Schemas` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SchemasClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("schemas") as client:  # (1)
    result = await client.create_discoverer()  # (2)
```

1. client: [SchemasClient](./client.md)
2. result: [:material-code-braces: CreateDiscovererResponseTypeDef](./type_defs.md#creatediscovererresponsetypedef)



#### Paginator usage example

```python
# ListDiscoverersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("schemas") as client:  # (1)
    paginator = client.get_paginator("list_discoverers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListDiscoverersPaginator](./paginators.md#listdiscovererspaginator)
3. item: [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef)



#### Waiter usage example

```python
# CodeBindingExistsWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("schemas") as client:  # (1)
    waiter = client.get_waiter("code_binding_exists")  # (2)
    await waiter.wait(...)
```

1. client: [SchemasClient](./client.md)
2. waiter: [CodeBindingExistsWaiter](./waiters.md#codebindingexistswaiter)


### Explicit type annotations

With `types-aioboto3-lite[schemas]`
or a standalone `types_aiobotocore_schemas` package, you have to explicitly specify
`client: SchemasClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SchemasClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.type_defs import CreateDiscovererResponseTypeDef
from types_aiobotocore_schemas.type_defs import CreateDiscovererRequestTypeDef


session = Session()

client: SchemasClient
async with session.client("schemas") as client:  # (1)
    kwargs: CreateDiscovererRequestTypeDef = {...}  # (2)
    result: CreateDiscovererResponseTypeDef = await client.create_discoverer(**kwargs)  # (3)
```

1. client: [SchemasClient](./client.md)
2. kwargs: [:material-code-braces: CreateDiscovererRequestTypeDef](./type_defs.md#creatediscovererrequesttypedef)
3. result: [:material-code-braces: CreateDiscovererResponseTypeDef](./type_defs.md#creatediscovererresponsetypedef)



#### Paginator usage example

```python
# ListDiscoverersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.paginator import ListDiscoverersPaginator
from types_aiobotocore_schemas.type_defs import ListDiscoverersResponseTypeDef


session = Session()

client: SchemasClient
async with session.client("schemas") as client:  # (1)
    paginator: ListDiscoverersPaginator = client.get_paginator("list_discoverers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoverersResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListDiscoverersPaginator](./paginators.md#listdiscovererspaginator)
3. item: [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef)



#### Waiter usage example

```python
# CodeBindingExistsWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_schemas.client import SchemasClient
from types_aiobotocore_schemas.waiter import CodeBindingExistsWaiter


session = Session()

async with session.client("schemas") as client:  # (1)
    waiter = client.get_waiter("code_binding_exists")  # (2)
    await waiter.wait(...)
```

1. client: [SchemasClient](./client.md)
2. waiter: [CodeBindingExistsWaiter](./waiters.md#codebindingexistswaiter)


