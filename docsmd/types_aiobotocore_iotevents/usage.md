# Examples

> [Index](../README.md) > [IoTEvents](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#iotevents)
    type annotations stubs module [types-aiobotocore-iotevents](https://pypi.org/project/types-aiobotocore-iotevents/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotevents]` package installed.

Write your `IoTEvents` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IoTEventsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotevents") as client:  # (1)
    result = await client.create_alarm_model()  # (2)
```

1. client: [IoTEventsClient](./client.md)
2. result: [:material-code-braces: CreateAlarmModelResponseTypeDef](./type_defs.md#createalarmmodelresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[iotevents]`
or a standalone `types_aiobotocore_iotevents` package, you have to explicitly specify
`client: IoTEventsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IoTEventsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotevents.client import IoTEventsClient
from types_aiobotocore_iotevents.type_defs import CreateAlarmModelResponseTypeDef
from types_aiobotocore_iotevents.type_defs import CreateAlarmModelRequestTypeDef


session = Session()

client: IoTEventsClient
async with session.client("iotevents") as client:  # (1)
    kwargs: CreateAlarmModelRequestTypeDef = {...}  # (2)
    result: CreateAlarmModelResponseTypeDef = await client.create_alarm_model(**kwargs)  # (3)
```

1. client: [IoTEventsClient](./client.md)
2. kwargs: [:material-code-braces: CreateAlarmModelRequestTypeDef](./type_defs.md#createalarmmodelrequesttypedef)
3. result: [:material-code-braces: CreateAlarmModelResponseTypeDef](./type_defs.md#createalarmmodelresponsetypedef)






