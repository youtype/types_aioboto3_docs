# Examples

> [Index](../README.md) > [UserNotifications](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[notifications]` package installed.

Write your `UserNotifications` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# UserNotificationsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("notifications") as client:  # (1)
    result = await client.create_event_rule()  # (2)
```

1. client: [UserNotificationsClient](./client.md)
2. result: [:material-code-braces: CreateEventRuleResponseTypeDef](./type_defs.md#createeventruleresponsetypedef)



#### Paginator usage example

```python
# ListChannelsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("notifications") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[notifications]`
or a standalone `types_aiobotocore_notifications` package, you have to explicitly specify
`client: UserNotificationsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# UserNotificationsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_notifications.client import UserNotificationsClient
from types_aiobotocore_notifications.type_defs import CreateEventRuleResponseTypeDef
from types_aiobotocore_notifications.type_defs import CreateEventRuleRequestTypeDef


session = Session()

client: UserNotificationsClient
async with session.client("notifications") as client:  # (1)
    kwargs: CreateEventRuleRequestTypeDef = {...}  # (2)
    result: CreateEventRuleResponseTypeDef = await client.create_event_rule(**kwargs)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. kwargs: [:material-code-braces: CreateEventRuleRequestTypeDef](./type_defs.md#createeventrulerequesttypedef)
3. result: [:material-code-braces: CreateEventRuleResponseTypeDef](./type_defs.md#createeventruleresponsetypedef)



#### Paginator usage example

```python
# ListChannelsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_notifications.client import UserNotificationsClient
from types_aiobotocore_notifications.paginator import ListChannelsPaginator
from types_aiobotocore_notifications.type_defs import ListChannelsResponseTypeDef


session = Session()

client: UserNotificationsClient
async with session.client("notifications") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [UserNotificationsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)




