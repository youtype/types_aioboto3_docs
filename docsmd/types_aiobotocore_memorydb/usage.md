# Examples

> [Index](../README.md) > [MemoryDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#memorydb)
    type annotations stubs module [types-aiobotocore-memorydb](https://pypi.org/project/types-aiobotocore-memorydb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[memorydb]` package installed.

Write your `MemoryDB` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MemoryDBClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("memorydb") as client:  # (1)
    result = await client.batch_update_cluster()  # (2)
```

1. client: [MemoryDBClient](./client.md)
2. result: [:material-code-braces: BatchUpdateClusterResponseTypeDef](./type_defs.md#batchupdateclusterresponsetypedef)



#### Paginator usage example

```python
# DescribeACLsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("memorydb") as client:  # (1)
    paginator = client.get_paginator("describe_acls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeACLsPaginator](./paginators.md#describeaclspaginator)
3. item: [:material-code-braces: DescribeACLsResponseTypeDef](./type_defs.md#describeaclsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[memorydb]`
or a standalone `types_aiobotocore_memorydb` package, you have to explicitly specify
`client: MemoryDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MemoryDBClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_memorydb.client import MemoryDBClient
from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterResponseTypeDef
from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterRequestTypeDef


session = Session()

client: MemoryDBClient
async with session.client("memorydb") as client:  # (1)
    kwargs: BatchUpdateClusterRequestTypeDef = {...}  # (2)
    result: BatchUpdateClusterResponseTypeDef = await client.batch_update_cluster(**kwargs)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. kwargs: [:material-code-braces: BatchUpdateClusterRequestTypeDef](./type_defs.md#batchupdateclusterrequesttypedef)
3. result: [:material-code-braces: BatchUpdateClusterResponseTypeDef](./type_defs.md#batchupdateclusterresponsetypedef)



#### Paginator usage example

```python
# DescribeACLsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_memorydb.client import MemoryDBClient
from types_aiobotocore_memorydb.paginator import DescribeACLsPaginator
from types_aiobotocore_memorydb.type_defs import DescribeACLsResponseTypeDef


session = Session()

client: MemoryDBClient
async with session.client("memorydb") as client:  # (1)
    paginator: DescribeACLsPaginator = client.get_paginator("describe_acls")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeACLsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeACLsPaginator](./paginators.md#describeaclspaginator)
3. item: [:material-code-braces: DescribeACLsResponseTypeDef](./type_defs.md#describeaclsresponsetypedef)




