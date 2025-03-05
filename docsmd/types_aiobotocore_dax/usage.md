# Examples

> [Index](../README.md) > [DAX](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DAX](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#dax)
    type annotations stubs module [types-aiobotocore-dax](https://pypi.org/project/types-aiobotocore-dax/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dax]` package installed.

Write your `DAX` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DAXClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("dax") as client:  # (1)
    result = await client.create_cluster()  # (2)
```

1. client: [DAXClient](./client.md)
2. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)



#### Paginator usage example

```python
# DescribeClustersPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("dax") as client:  # (1)
    paginator = client.get_paginator("describe_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DAXClient](./client.md)
2. paginator: [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
3. item: [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[dax]`
or a standalone `types_aiobotocore_dax` package, you have to explicitly specify
`client: DAXClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DAXClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dax.client import DAXClient
from types_aiobotocore_dax.type_defs import CreateClusterResponseTypeDef
from types_aiobotocore_dax.type_defs import CreateClusterRequestTypeDef


session = Session()

client: DAXClient
async with session.client("dax") as client:  # (1)
    kwargs: CreateClusterRequestTypeDef = {...}  # (2)
    result: CreateClusterResponseTypeDef = await client.create_cluster(**kwargs)  # (3)
```

1. client: [DAXClient](./client.md)
2. kwargs: [:material-code-braces: CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef)
3. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)



#### Paginator usage example

```python
# DescribeClustersPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_dax.client import DAXClient
from types_aiobotocore_dax.paginator import DescribeClustersPaginator
from types_aiobotocore_dax.type_defs import DescribeClustersResponseTypeDef


session = Session()

client: DAXClient
async with session.client("dax") as client:  # (1)
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [DAXClient](./client.md)
2. paginator: [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
3. item: [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)




