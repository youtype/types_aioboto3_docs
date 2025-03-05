# Examples

> [Index](../README.md) > [DeadlineCloud](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#deadlinecloud)
    type annotations stubs module [types-aiobotocore-deadline](https://pypi.org/project/types-aiobotocore-deadline/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[deadline]` package installed.

Write your `DeadlineCloud` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DeadlineCloudClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("deadline") as client:  # (1)
    result = await client.assume_fleet_role_for_read()  # (2)
```

1. client: [DeadlineCloudClient](./client.md)
2. result: [:material-code-braces: AssumeFleetRoleForReadResponseTypeDef](./type_defs.md#assumefleetroleforreadresponsetypedef)



#### Paginator usage example

```python
# GetSessionsStatisticsAggregationPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("deadline") as client:  # (1)
    paginator = client.get_paginator("get_sessions_statistics_aggregation")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DeadlineCloudClient](./client.md)
2. paginator: [GetSessionsStatisticsAggregationPaginator](./paginators.md#getsessionsstatisticsaggregationpaginator)
3. item: [:material-code-braces: GetSessionsStatisticsAggregationResponseTypeDef](./type_defs.md#getsessionsstatisticsaggregationresponsetypedef)



#### Waiter usage example

```python
# FleetActiveWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("deadline") as client:  # (1)
    waiter = client.get_waiter("fleet_active")  # (2)
    await waiter.wait(...)
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [FleetActiveWaiter](./waiters.md#fleetactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[deadline]`
or a standalone `types_aiobotocore_deadline` package, you have to explicitly specify
`client: DeadlineCloudClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DeadlineCloudClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_deadline.client import DeadlineCloudClient
from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForReadResponseTypeDef
from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForReadRequestTypeDef


session = Session()

client: DeadlineCloudClient
async with session.client("deadline") as client:  # (1)
    kwargs: AssumeFleetRoleForReadRequestTypeDef = {...}  # (2)
    result: AssumeFleetRoleForReadResponseTypeDef = await client.assume_fleet_role_for_read(**kwargs)  # (3)
```

1. client: [DeadlineCloudClient](./client.md)
2. kwargs: [:material-code-braces: AssumeFleetRoleForReadRequestTypeDef](./type_defs.md#assumefleetroleforreadrequesttypedef)
3. result: [:material-code-braces: AssumeFleetRoleForReadResponseTypeDef](./type_defs.md#assumefleetroleforreadresponsetypedef)



#### Paginator usage example

```python
# GetSessionsStatisticsAggregationPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_deadline.client import DeadlineCloudClient
from types_aiobotocore_deadline.paginator import GetSessionsStatisticsAggregationPaginator
from types_aiobotocore_deadline.type_defs import GetSessionsStatisticsAggregationResponseTypeDef


session = Session()

client: DeadlineCloudClient
async with session.client("deadline") as client:  # (1)
    paginator: GetSessionsStatisticsAggregationPaginator = client.get_paginator("get_sessions_statistics_aggregation")  # (2)
    async for item in paginator.paginate(...):
        item: GetSessionsStatisticsAggregationResponseTypeDef
        print(item)  # (3)
```

1. client: [DeadlineCloudClient](./client.md)
2. paginator: [GetSessionsStatisticsAggregationPaginator](./paginators.md#getsessionsstatisticsaggregationpaginator)
3. item: [:material-code-braces: GetSessionsStatisticsAggregationResponseTypeDef](./type_defs.md#getsessionsstatisticsaggregationresponsetypedef)



#### Waiter usage example

```python
# FleetActiveWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_deadline.client import DeadlineCloudClient
from types_aiobotocore_deadline.waiter import FleetActiveWaiter


session = Session()

async with session.client("deadline") as client:  # (1)
    waiter = client.get_waiter("fleet_active")  # (2)
    await waiter.wait(...)
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [FleetActiveWaiter](./waiters.md#fleetactivewaiter)


