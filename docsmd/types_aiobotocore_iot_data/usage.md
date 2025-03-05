# Examples

> [Index](../README.md) > [IoTDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iot-data]` package installed.

Write your `IoTDataPlane` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IoTDataPlaneClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iot-data") as client:  # (1)
    result = await client.delete_thing_shadow()  # (2)
```

1. client: [IoTDataPlaneClient](./client.md)
2. result: [:material-code-braces: DeleteThingShadowResponseTypeDef](./type_defs.md#deletethingshadowresponsetypedef)



#### Paginator usage example

```python
# ListRetainedMessagesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("iot-data") as client:  # (1)
    paginator = client.get_paginator("list_retained_messages")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTDataPlaneClient](./client.md)
2. paginator: [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)
3. item: [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[iot-data]`
or a standalone `types_aiobotocore_iot_data` package, you have to explicitly specify
`client: IoTDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IoTDataPlaneClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient
from types_aiobotocore_iot_data.type_defs import DeleteThingShadowResponseTypeDef
from types_aiobotocore_iot_data.type_defs import DeleteThingShadowRequestTypeDef


session = Session()

client: IoTDataPlaneClient
async with session.client("iot-data") as client:  # (1)
    kwargs: DeleteThingShadowRequestTypeDef = {...}  # (2)
    result: DeleteThingShadowResponseTypeDef = await client.delete_thing_shadow(**kwargs)  # (3)
```

1. client: [IoTDataPlaneClient](./client.md)
2. kwargs: [:material-code-braces: DeleteThingShadowRequestTypeDef](./type_defs.md#deletethingshadowrequesttypedef)
3. result: [:material-code-braces: DeleteThingShadowResponseTypeDef](./type_defs.md#deletethingshadowresponsetypedef)



#### Paginator usage example

```python
# ListRetainedMessagesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient
from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator
from types_aiobotocore_iot_data.type_defs import ListRetainedMessagesResponseTypeDef


session = Session()

client: IoTDataPlaneClient
async with session.client("iot-data") as client:  # (1)
    paginator: ListRetainedMessagesPaginator = client.get_paginator("list_retained_messages")  # (2)
    async for item in paginator.paginate(...):
        item: ListRetainedMessagesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTDataPlaneClient](./client.md)
2. paginator: [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)
3. item: [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef)




