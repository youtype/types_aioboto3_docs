# Examples

> [Index](../README.md) > [Drs](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[drs]` package installed.

Write your `Drs` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DrsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("drs") as client:  # (1)
    result = await client.associate_source_network_stack()  # (2)
```

1. client: [DrsClient](./client.md)
2. result: [:material-code-braces: AssociateSourceNetworkStackResponseTypeDef](./type_defs.md#associatesourcenetworkstackresponsetypedef)



#### Paginator usage example

```python
# DescribeJobLogItemsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("drs") as client:  # (1)
    paginator = client.get_paginator("describe_job_log_items")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[drs]`
or a standalone `types_aiobotocore_drs` package, you have to explicitly specify
`client: DrsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DrsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_drs.client import DrsClient
from types_aiobotocore_drs.type_defs import AssociateSourceNetworkStackResponseTypeDef
from types_aiobotocore_drs.type_defs import AssociateSourceNetworkStackRequestTypeDef


session = Session()

client: DrsClient
async with session.client("drs") as client:  # (1)
    kwargs: AssociateSourceNetworkStackRequestTypeDef = {...}  # (2)
    result: AssociateSourceNetworkStackResponseTypeDef = await client.associate_source_network_stack(**kwargs)  # (3)
```

1. client: [DrsClient](./client.md)
2. kwargs: [:material-code-braces: AssociateSourceNetworkStackRequestTypeDef](./type_defs.md#associatesourcenetworkstackrequesttypedef)
3. result: [:material-code-braces: AssociateSourceNetworkStackResponseTypeDef](./type_defs.md#associatesourcenetworkstackresponsetypedef)



#### Paginator usage example

```python
# DescribeJobLogItemsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_drs.client import DrsClient
from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator
from types_aiobotocore_drs.type_defs import DescribeJobLogItemsResponseTypeDef


session = Session()

client: DrsClient
async with session.client("drs") as client:  # (1)
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobLogItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef)




