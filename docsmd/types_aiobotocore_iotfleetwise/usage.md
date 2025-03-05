# Examples

> [Index](../README.md) > [IoTFleetWise](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#iotfleetwise)
    type annotations stubs module [types-aiobotocore-iotfleetwise](https://pypi.org/project/types-aiobotocore-iotfleetwise/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iotfleetwise]` package installed.

Write your `IoTFleetWise` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IoTFleetWiseClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotfleetwise") as client:  # (1)
    result = await client.batch_create_vehicle()  # (2)
```

1. client: [IoTFleetWiseClient](./client.md)
2. result: [:material-code-braces: BatchCreateVehicleResponseTypeDef](./type_defs.md#batchcreatevehicleresponsetypedef)



#### Paginator usage example

```python
# GetVehicleStatusPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("iotfleetwise") as client:  # (1)
    paginator = client.get_paginator("get_vehicle_status")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [GetVehicleStatusPaginator](./paginators.md#getvehiclestatuspaginator)
3. item: [:material-code-braces: GetVehicleStatusResponseTypeDef](./type_defs.md#getvehiclestatusresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[iotfleetwise]`
or a standalone `types_aiobotocore_iotfleetwise` package, you have to explicitly specify
`client: IoTFleetWiseClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IoTFleetWiseClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotfleetwise.client import IoTFleetWiseClient
from types_aiobotocore_iotfleetwise.type_defs import BatchCreateVehicleResponseTypeDef
from types_aiobotocore_iotfleetwise.type_defs import BatchCreateVehicleRequestTypeDef


session = Session()

client: IoTFleetWiseClient
async with session.client("iotfleetwise") as client:  # (1)
    kwargs: BatchCreateVehicleRequestTypeDef = {...}  # (2)
    result: BatchCreateVehicleResponseTypeDef = await client.batch_create_vehicle(**kwargs)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. kwargs: [:material-code-braces: BatchCreateVehicleRequestTypeDef](./type_defs.md#batchcreatevehiclerequesttypedef)
3. result: [:material-code-braces: BatchCreateVehicleResponseTypeDef](./type_defs.md#batchcreatevehicleresponsetypedef)



#### Paginator usage example

```python
# GetVehicleStatusPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_iotfleetwise.client import IoTFleetWiseClient
from types_aiobotocore_iotfleetwise.paginator import GetVehicleStatusPaginator
from types_aiobotocore_iotfleetwise.type_defs import GetVehicleStatusResponseTypeDef


session = Session()

client: IoTFleetWiseClient
async with session.client("iotfleetwise") as client:  # (1)
    paginator: GetVehicleStatusPaginator = client.get_paginator("get_vehicle_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetVehicleStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [GetVehicleStatusPaginator](./paginators.md#getvehiclestatuspaginator)
3. item: [:material-code-braces: GetVehicleStatusResponseTypeDef](./type_defs.md#getvehiclestatusresponsetypedef)




