# Examples

> [Index](../README.md) > [SESV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sesv2]` package installed.

Write your `SESV2` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SESV2Client usage example

from aioboto3.session import Session


session = Session()

async with session.client("sesv2") as client:  # (1)
    result = await client.batch_get_metric_data()  # (2)
```

1. client: [SESV2Client](./client.md)
2. result: [:material-code-braces: BatchGetMetricDataResponseTypeDef](./type_defs.md#batchgetmetricdataresponsetypedef)



#### Paginator usage example

```python
# ListMultiRegionEndpointsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("sesv2") as client:  # (1)
    paginator = client.get_paginator("list_multi_region_endpoints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListMultiRegionEndpointsPaginator](./paginators.md#listmultiregionendpointspaginator)
3. item: [:material-code-braces: ListMultiRegionEndpointsResponseTypeDef](./type_defs.md#listmultiregionendpointsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[sesv2]`
or a standalone `types_aiobotocore_sesv2` package, you have to explicitly specify
`client: SESV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SESV2Client usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sesv2.client import SESV2Client
from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataResponseTypeDef
from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataRequestTypeDef


session = Session()

client: SESV2Client
async with session.client("sesv2") as client:  # (1)
    kwargs: BatchGetMetricDataRequestTypeDef = {...}  # (2)
    result: BatchGetMetricDataResponseTypeDef = await client.batch_get_metric_data(**kwargs)  # (3)
```

1. client: [SESV2Client](./client.md)
2. kwargs: [:material-code-braces: BatchGetMetricDataRequestTypeDef](./type_defs.md#batchgetmetricdatarequesttypedef)
3. result: [:material-code-braces: BatchGetMetricDataResponseTypeDef](./type_defs.md#batchgetmetricdataresponsetypedef)



#### Paginator usage example

```python
# ListMultiRegionEndpointsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sesv2.client import SESV2Client
from types_aiobotocore_sesv2.paginator import ListMultiRegionEndpointsPaginator
from types_aiobotocore_sesv2.type_defs import ListMultiRegionEndpointsResponseTypeDef


session = Session()

client: SESV2Client
async with session.client("sesv2") as client:  # (1)
    paginator: ListMultiRegionEndpointsPaginator = client.get_paginator("list_multi_region_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListMultiRegionEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListMultiRegionEndpointsPaginator](./paginators.md#listmultiregionendpointspaginator)
3. item: [:material-code-braces: ListMultiRegionEndpointsResponseTypeDef](./type_defs.md#listmultiregionendpointsresponsetypedef)




