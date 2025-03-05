# Examples

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[internetmonitor]` package installed.

Write your `CloudWatchInternetMonitor` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudWatchInternetMonitorClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("internetmonitor") as client:  # (1)
    result = await client.create_monitor()  # (2)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef)



#### Paginator usage example

```python
# ListHealthEventsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("internetmonitor") as client:  # (1)
    paginator = client.get_paginator("list_health_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. paginator: [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
3. item: [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[internetmonitor]`
or a standalone `types_aiobotocore_internetmonitor` package, you have to explicitly specify
`client: CloudWatchInternetMonitorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudWatchInternetMonitorClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient
from types_aiobotocore_internetmonitor.type_defs import CreateMonitorOutputTypeDef
from types_aiobotocore_internetmonitor.type_defs import CreateMonitorInputTypeDef


session = Session()

client: CloudWatchInternetMonitorClient
async with session.client("internetmonitor") as client:  # (1)
    kwargs: CreateMonitorInputTypeDef = {...}  # (2)
    result: CreateMonitorOutputTypeDef = await client.create_monitor(**kwargs)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. kwargs: [:material-code-braces: CreateMonitorInputTypeDef](./type_defs.md#createmonitorinputtypedef)
3. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef)



#### Paginator usage example

```python
# ListHealthEventsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient
from types_aiobotocore_internetmonitor.paginator import ListHealthEventsPaginator
from types_aiobotocore_internetmonitor.type_defs import ListHealthEventsOutputTypeDef


session = Session()

client: CloudWatchInternetMonitorClient
async with session.client("internetmonitor") as client:  # (1)
    paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListHealthEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchInternetMonitorClient](./client.md)
2. paginator: [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
3. item: [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef)




