# Examples

> [Index](../README.md) > [IoTAnalytics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotanalytics]` package installed.

Write your `IoTAnalytics` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IoTAnalyticsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotanalytics") as client:  # (1)
    result = await client.batch_put_message()  # (2)
```

1. client: [IoTAnalyticsClient](./client.md)
2. result: [:material-code-braces: BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef)



#### Paginator usage example

```python
# ListChannelsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotanalytics") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[iotanalytics]`
or a standalone `types_aiobotocore_iotanalytics` package, you have to explicitly specify
`client: IoTAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IoTAnalyticsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient
from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageResponseTypeDef
from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageRequestTypeDef


session = Session()

client: IoTAnalyticsClient
async with session.client("iotanalytics") as client:  # (1)
    kwargs: BatchPutMessageRequestTypeDef = {...}  # (2)
    result: BatchPutMessageResponseTypeDef = await client.batch_put_message(**kwargs)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. kwargs: [:material-code-braces: BatchPutMessageRequestTypeDef](./type_defs.md#batchputmessagerequesttypedef)
3. result: [:material-code-braces: BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef)



#### Paginator usage example

```python
# ListChannelsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient
from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator
from types_aiobotocore_iotanalytics.type_defs import ListChannelsResponseTypeDef


session = Session()

client: IoTAnalyticsClient
async with session.client("iotanalytics") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)




