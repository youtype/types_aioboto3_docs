# Examples

> [Index](../README.md) > [EventBridge](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#eventbridge)
    type annotations stubs module [types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[events]` package installed.

Write your `EventBridge` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EventBridgeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("events") as client:  # (1)
    result = await client.activate_event_source()  # (2)
```

1. client: [EventBridgeClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListRuleNamesByTargetPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("events") as client:  # (1)
    paginator = client.get_paginator("list_rule_names_by_target")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EventBridgeClient](./client.md)
2. paginator: [ListRuleNamesByTargetPaginator](./paginators.md#listrulenamesbytargetpaginator)
3. item: [:material-code-braces: ListRuleNamesByTargetResponseTypeDef](./type_defs.md#listrulenamesbytargetresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[events]`
or a standalone `types_aiobotocore_events` package, you have to explicitly specify
`client: EventBridgeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EventBridgeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_events.client import EventBridgeClient
from types_aiobotocore_events.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_events.type_defs import ActivateEventSourceRequestTypeDef


session = Session()

client: EventBridgeClient
async with session.client("events") as client:  # (1)
    kwargs: ActivateEventSourceRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.activate_event_source(**kwargs)  # (3)
```

1. client: [EventBridgeClient](./client.md)
2. kwargs: [:material-code-braces: ActivateEventSourceRequestTypeDef](./type_defs.md#activateeventsourcerequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListRuleNamesByTargetPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_events.client import EventBridgeClient
from types_aiobotocore_events.paginator import ListRuleNamesByTargetPaginator
from types_aiobotocore_events.type_defs import ListRuleNamesByTargetResponseTypeDef


session = Session()

client: EventBridgeClient
async with session.client("events") as client:  # (1)
    paginator: ListRuleNamesByTargetPaginator = client.get_paginator("list_rule_names_by_target")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleNamesByTargetResponseTypeDef
        print(item)  # (3)
```

1. client: [EventBridgeClient](./client.md)
2. paginator: [ListRuleNamesByTargetPaginator](./paginators.md#listrulenamesbytargetpaginator)
3. item: [:material-code-braces: ListRuleNamesByTargetResponseTypeDef](./type_defs.md#listrulenamesbytargetresponsetypedef)




