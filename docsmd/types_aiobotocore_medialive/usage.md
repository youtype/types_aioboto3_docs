# Examples

> [Index](../README.md) > [MediaLive](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#medialive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[medialive]` package installed.

Write your `MediaLive` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MediaLiveClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("medialive") as client:  # (1)
    result = await client.batch_delete()  # (2)
```

1. client: [MediaLiveClient](./client.md)
2. result: [:material-code-braces: BatchDeleteResponseTypeDef](./type_defs.md#batchdeleteresponsetypedef)



#### Paginator usage example

```python
# DescribeSchedulePaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("medialive") as client:  # (1)
    paginator = client.get_paginator("describe_schedule")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [DescribeSchedulePaginator](./paginators.md#describeschedulepaginator)
3. item: [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef)



#### Waiter usage example

```python
# ChannelCreatedWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("medialive") as client:  # (1)
    waiter = client.get_waiter("channel_created")  # (2)
    await waiter.wait(...)
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelCreatedWaiter](./waiters.md#channelcreatedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[medialive]`
or a standalone `types_aiobotocore_medialive` package, you have to explicitly specify
`client: MediaLiveClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MediaLiveClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.type_defs import BatchDeleteResponseTypeDef
from types_aiobotocore_medialive.type_defs import BatchDeleteRequestTypeDef


session = Session()

client: MediaLiveClient
async with session.client("medialive") as client:  # (1)
    kwargs: BatchDeleteRequestTypeDef = {...}  # (2)
    result: BatchDeleteResponseTypeDef = await client.batch_delete(**kwargs)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteRequestTypeDef](./type_defs.md#batchdeleterequesttypedef)
3. result: [:material-code-braces: BatchDeleteResponseTypeDef](./type_defs.md#batchdeleteresponsetypedef)



#### Paginator usage example

```python
# DescribeSchedulePaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.paginator import DescribeSchedulePaginator
from types_aiobotocore_medialive.type_defs import DescribeScheduleResponseTypeDef


session = Session()

client: MediaLiveClient
async with session.client("medialive") as client:  # (1)
    paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScheduleResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaLiveClient](./client.md)
2. paginator: [DescribeSchedulePaginator](./paginators.md#describeschedulepaginator)
3. item: [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef)



#### Waiter usage example

```python
# ChannelCreatedWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_medialive.client import MediaLiveClient
from types_aiobotocore_medialive.waiter import ChannelCreatedWaiter


session = Session()

async with session.client("medialive") as client:  # (1)
    waiter = client.get_waiter("channel_created")  # (2)
    await waiter.wait(...)
```

1. client: [MediaLiveClient](./client.md)
2. waiter: [ChannelCreatedWaiter](./waiters.md#channelcreatedwaiter)


