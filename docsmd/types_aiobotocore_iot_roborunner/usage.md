# Examples

> [Index](../README.md) > [IoTRoboRunner](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTRoboRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
    type annotations stubs module [types-aiobotocore-iot-roborunner](https://pypi.org/project/types-aiobotocore-iot-roborunner/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iot-roborunner]` package installed.

Write your `IoTRoboRunner` code as usual,
type checking and code completion should work out of the box.



```python
# IoTRoboRunnerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iot-roborunner") as client:  # (1)
    result = await client.create_destination()  # (2)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. result: [:material-code-braces: CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef) 



```python
# ListDestinationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("iot-roborunner") as client:  # (1)
    paginator = client.get_paginator("list_destinations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
3. item: [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[iot-roborunner]`
or a standalone `types_aiobotocore_iot_roborunner` package, you have to explicitly specify
`client: IoTRoboRunnerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTRoboRunnerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iot_roborunner.client import IoTRoboRunnerClient
from types_aiobotocore_iot_roborunner.type_defs import CreateDestinationResponseTypeDef
from types_aiobotocore_iot_roborunner.type_defs import CreateDestinationRequestRequestTypeDef


session = Session()

client: IoTRoboRunnerClient
async with session.client("iot-roborunner") as client:  # (1)
    kwargs: CreateDestinationRequestRequestTypeDef = {...}  # (2)
    result: CreateDestinationResponseTypeDef = await client.create_destination(**kwargs)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. kwargs: [:material-code-braces: CreateDestinationRequestRequestTypeDef](./type_defs.md#createdestinationrequestrequesttypedef) 
3. result: [:material-code-braces: CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef) 



```python
# ListDestinationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iot_roborunner.client import IoTRoboRunnerClient
from types_aiobotocore_iot_roborunner.paginator import ListDestinationsPaginator
from types_aiobotocore_iot_roborunner.type_defs import ListDestinationsResponseTypeDef


session = Session()

client: IoTRoboRunnerClient
async with session.client("iot-roborunner") as client:  # (1)
    paginator: ListDestinationsPaginator = client.get_paginator("list_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
3. item: [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 




