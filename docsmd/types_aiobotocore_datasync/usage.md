# Examples

> [Index](../README.md) > [DataSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[datasync]` package installed.

Write your `DataSync` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DataSyncClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("datasync") as client:  # (1)
    result = await client.add_storage_system()  # (2)
```

1. client: [DataSyncClient](./client.md)
2. result: [:material-code-braces: AddStorageSystemResponseTypeDef](./type_defs.md#addstoragesystemresponsetypedef)



#### Paginator usage example

```python
# DescribeStorageSystemResourceMetricsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("datasync") as client:  # (1)
    paginator = client.get_paginator("describe_storage_system_resource_metrics")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [DescribeStorageSystemResourceMetricsPaginator](./paginators.md#describestoragesystemresourcemetricspaginator)
3. item: [:material-code-braces: DescribeStorageSystemResourceMetricsResponseTypeDef](./type_defs.md#describestoragesystemresourcemetricsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[datasync]`
or a standalone `types_aiobotocore_datasync` package, you have to explicitly specify
`client: DataSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DataSyncClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_datasync.client import DataSyncClient
from types_aiobotocore_datasync.type_defs import AddStorageSystemResponseTypeDef
from types_aiobotocore_datasync.type_defs import AddStorageSystemRequestTypeDef


session = Session()

client: DataSyncClient
async with session.client("datasync") as client:  # (1)
    kwargs: AddStorageSystemRequestTypeDef = {...}  # (2)
    result: AddStorageSystemResponseTypeDef = await client.add_storage_system(**kwargs)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. kwargs: [:material-code-braces: AddStorageSystemRequestTypeDef](./type_defs.md#addstoragesystemrequesttypedef)
3. result: [:material-code-braces: AddStorageSystemResponseTypeDef](./type_defs.md#addstoragesystemresponsetypedef)



#### Paginator usage example

```python
# DescribeStorageSystemResourceMetricsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_datasync.client import DataSyncClient
from types_aiobotocore_datasync.paginator import DescribeStorageSystemResourceMetricsPaginator
from types_aiobotocore_datasync.type_defs import DescribeStorageSystemResourceMetricsResponseTypeDef


session = Session()

client: DataSyncClient
async with session.client("datasync") as client:  # (1)
    paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator("describe_storage_system_resource_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStorageSystemResourceMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [DescribeStorageSystemResourceMetricsPaginator](./paginators.md#describestoragesystemresourcemetricspaginator)
3. item: [:material-code-braces: DescribeStorageSystemResourceMetricsResponseTypeDef](./type_defs.md#describestoragesystemresourcemetricsresponsetypedef)




