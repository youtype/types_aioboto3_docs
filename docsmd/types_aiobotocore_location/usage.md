# Examples

> [Index](../README.md) > [LocationService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#locationservice)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[location]` package installed.

Write your `LocationService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# LocationServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("location") as client:  # (1)
    result = await client.batch_delete_device_position_history()  # (2)
```

1. client: [LocationServiceClient](./client.md)
2. result: [:material-code-braces: BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef)



#### Paginator usage example

```python
# ForecastGeofenceEventsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("location") as client:  # (1)
    paginator = client.get_paginator("forecast_geofence_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ForecastGeofenceEventsPaginator](./paginators.md#forecastgeofenceeventspaginator)
3. item: [:material-code-braces: ForecastGeofenceEventsResponseTypeDef](./type_defs.md#forecastgeofenceeventsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[location]`
or a standalone `types_aiobotocore_location` package, you have to explicitly specify
`client: LocationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# LocationServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_location.client import LocationServiceClient
from types_aiobotocore_location.type_defs import BatchDeleteDevicePositionHistoryResponseTypeDef
from types_aiobotocore_location.type_defs import BatchDeleteDevicePositionHistoryRequestTypeDef


session = Session()

client: LocationServiceClient
async with session.client("location") as client:  # (1)
    kwargs: BatchDeleteDevicePositionHistoryRequestTypeDef = {...}  # (2)
    result: BatchDeleteDevicePositionHistoryResponseTypeDef = await client.batch_delete_device_position_history(**kwargs)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteDevicePositionHistoryRequestTypeDef](./type_defs.md#batchdeletedevicepositionhistoryrequesttypedef)
3. result: [:material-code-braces: BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef)



#### Paginator usage example

```python
# ForecastGeofenceEventsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_location.client import LocationServiceClient
from types_aiobotocore_location.paginator import ForecastGeofenceEventsPaginator
from types_aiobotocore_location.type_defs import ForecastGeofenceEventsResponseTypeDef


session = Session()

client: LocationServiceClient
async with session.client("location") as client:  # (1)
    paginator: ForecastGeofenceEventsPaginator = client.get_paginator("forecast_geofence_events")  # (2)
    async for item in paginator.paginate(...):
        item: ForecastGeofenceEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ForecastGeofenceEventsPaginator](./paginators.md#forecastgeofenceeventspaginator)
3. item: [:material-code-braces: ForecastGeofenceEventsResponseTypeDef](./type_defs.md#forecastgeofenceeventsresponsetypedef)




