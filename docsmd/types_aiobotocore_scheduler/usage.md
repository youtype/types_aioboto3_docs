# Examples

> [Index](../README.md) > [EventBridgeScheduler](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EventBridgeScheduler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#eventbridgescheduler)
    type annotations stubs module [types-aiobotocore-scheduler](https://pypi.org/project/types-aiobotocore-scheduler/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[scheduler]` package installed.

Write your `EventBridgeScheduler` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EventBridgeSchedulerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("scheduler") as client:  # (1)
    result = await client.create_schedule()  # (2)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. result: [:material-code-braces: CreateScheduleOutputTypeDef](./type_defs.md#createscheduleoutputtypedef)



#### Paginator usage example

```python
# ListScheduleGroupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("scheduler") as client:  # (1)
    paginator = client.get_paginator("list_schedule_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. paginator: [ListScheduleGroupsPaginator](./paginators.md#listschedulegroupspaginator)
3. item: [:material-code-braces: ListScheduleGroupsOutputTypeDef](./type_defs.md#listschedulegroupsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[scheduler]`
or a standalone `types_aiobotocore_scheduler` package, you have to explicitly specify
`client: EventBridgeSchedulerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EventBridgeSchedulerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_scheduler.client import EventBridgeSchedulerClient
from types_aiobotocore_scheduler.type_defs import CreateScheduleOutputTypeDef
from types_aiobotocore_scheduler.type_defs import CreateScheduleInputTypeDef


session = Session()

client: EventBridgeSchedulerClient
async with session.client("scheduler") as client:  # (1)
    kwargs: CreateScheduleInputTypeDef = {...}  # (2)
    result: CreateScheduleOutputTypeDef = await client.create_schedule(**kwargs)  # (3)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. kwargs: [:material-code-braces: CreateScheduleInputTypeDef](./type_defs.md#createscheduleinputtypedef)
3. result: [:material-code-braces: CreateScheduleOutputTypeDef](./type_defs.md#createscheduleoutputtypedef)



#### Paginator usage example

```python
# ListScheduleGroupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_scheduler.client import EventBridgeSchedulerClient
from types_aiobotocore_scheduler.paginator import ListScheduleGroupsPaginator
from types_aiobotocore_scheduler.type_defs import ListScheduleGroupsOutputTypeDef


session = Session()

client: EventBridgeSchedulerClient
async with session.client("scheduler") as client:  # (1)
    paginator: ListScheduleGroupsPaginator = client.get_paginator("list_schedule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListScheduleGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeSchedulerClient](./client.md)
2. paginator: [ListScheduleGroupsPaginator](./paginators.md#listschedulegroupspaginator)
3. item: [:material-code-braces: ListScheduleGroupsOutputTypeDef](./type_defs.md#listschedulegroupsoutputtypedef)




