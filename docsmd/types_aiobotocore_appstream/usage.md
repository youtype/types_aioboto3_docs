# Examples

> [Index](../README.md) > [AppStream](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#appstream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appstream]` package installed.

Write your `AppStream` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AppStreamClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("appstream") as client:  # (1)
    result = await client.associate_app_block_builder_app_block()  # (2)
```

1. client: [AppStreamClient](./client.md)
2. result: [:material-code-braces: AssociateAppBlockBuilderAppBlockResultTypeDef](./type_defs.md#associateappblockbuilderappblockresulttypedef)



#### Paginator usage example

```python
# DescribeDirectoryConfigsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("appstream") as client:  # (1)
    paginator = client.get_paginator("describe_directory_configs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef)



#### Waiter usage example

```python
# FleetStartedWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("appstream") as client:  # (1)
    waiter = client.get_waiter("fleet_started")  # (2)
    await waiter.wait(...)
```

1. client: [AppStreamClient](./client.md)
2. waiter: [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[appstream]`
or a standalone `types_aiobotocore_appstream` package, you have to explicitly specify
`client: AppStreamClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AppStreamClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.type_defs import AssociateAppBlockBuilderAppBlockResultTypeDef
from types_aiobotocore_appstream.type_defs import AssociateAppBlockBuilderAppBlockRequestTypeDef


session = Session()

client: AppStreamClient
async with session.client("appstream") as client:  # (1)
    kwargs: AssociateAppBlockBuilderAppBlockRequestTypeDef = {...}  # (2)
    result: AssociateAppBlockBuilderAppBlockResultTypeDef = await client.associate_app_block_builder_app_block(**kwargs)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. kwargs: [:material-code-braces: AssociateAppBlockBuilderAppBlockRequestTypeDef](./type_defs.md#associateappblockbuilderappblockrequesttypedef)
3. result: [:material-code-braces: AssociateAppBlockBuilderAppBlockResultTypeDef](./type_defs.md#associateappblockbuilderappblockresulttypedef)



#### Paginator usage example

```python
# DescribeDirectoryConfigsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator
from types_aiobotocore_appstream.type_defs import DescribeDirectoryConfigsResultTypeDef


session = Session()

client: AppStreamClient
async with session.client("appstream") as client:  # (1)
    paginator: DescribeDirectoryConfigsPaginator = client.get_paginator("describe_directory_configs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDirectoryConfigsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef)



#### Waiter usage example

```python
# FleetStartedWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_appstream.client import AppStreamClient
from types_aiobotocore_appstream.waiter import FleetStartedWaiter


session = Session()

async with session.client("appstream") as client:  # (1)
    waiter = client.get_waiter("fleet_started")  # (2)
    await waiter.wait(...)
```

1. client: [AppStreamClient](./client.md)
2. waiter: [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)


