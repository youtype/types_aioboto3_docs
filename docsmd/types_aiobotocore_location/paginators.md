# Paginators

> [Index](../README.md) > [LocationService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## GetDevicePositionHistoryPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("get_device_position_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import GetDevicePositionHistoryPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: GetDevicePositionHistoryPaginator = client.get_paginator("get_device_position_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetDevicePositionHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
3. item: [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetDevicePositionHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DeviceId: str,
    TrackerName: str,
    EndTimeExclusive: Union[datetime, str] = ...,
    StartTimeInclusive: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDevicePositionHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = {  # (1)
    "DeviceId": ...,
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef](./type_defs.md#getdevicepositionhistoryrequestgetdevicepositionhistorypaginatetypedef) 
## ListDevicePositionsPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_device_positions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListDevicePositionsPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListDevicePositionsPaginator = client.get_paginator("list_device_positions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicePositionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListDevicePositionsPaginator](./paginators.md#listdevicepositionspaginator)
3. item: [:material-code-braces: ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicePositionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TrackerName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDevicePositionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDevicePositionsRequestListDevicePositionsPaginateTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicePositionsRequestListDevicePositionsPaginateTypeDef](./type_defs.md#listdevicepositionsrequestlistdevicepositionspaginatetypedef) 
## ListGeofenceCollectionsPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_geofence_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListGeofenceCollectionsPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListGeofenceCollectionsPaginator = client.get_paginator("list_geofence_collections")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeofenceCollectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListGeofenceCollectionsPaginator](./paginators.md#listgeofencecollectionspaginator)
3. item: [:material-code-braces: ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGeofenceCollectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGeofenceCollectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef](./type_defs.md#listgeofencecollectionsrequestlistgeofencecollectionspaginatetypedef) 
## ListGeofencesPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_geofences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListGeofencesPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListGeofencesPaginator = client.get_paginator("list_geofences")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeofencesResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListGeofencesPaginator](./paginators.md#listgeofencespaginator)
3. item: [:material-code-braces: ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGeofencesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CollectionName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGeofencesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGeofencesRequestListGeofencesPaginateTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeofencesRequestListGeofencesPaginateTypeDef](./type_defs.md#listgeofencesrequestlistgeofencespaginatetypedef) 
## ListMapsPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_maps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListMapsPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListMapsPaginator = client.get_paginator("list_maps")  # (2)
    async for item in paginator.paginate(...):
        item: ListMapsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListMapsPaginator](./paginators.md#listmapspaginator)
3. item: [:material-code-braces: ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMapsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMapsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMapsRequestListMapsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMapsRequestListMapsPaginateTypeDef](./type_defs.md#listmapsrequestlistmapspaginatetypedef) 
## ListPlaceIndexesPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_place_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListPlaceIndexesPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlaceIndexesResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListPlaceIndexesPaginator](./paginators.md#listplaceindexespaginator)
3. item: [:material-code-braces: ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlaceIndexesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPlaceIndexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef](./type_defs.md#listplaceindexesrequestlistplaceindexespaginatetypedef) 
## ListRouteCalculatorsPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_route_calculators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListRouteCalculatorsPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")  # (2)
    async for item in paginator.paginate(...):
        item: ListRouteCalculatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListRouteCalculatorsPaginator](./paginators.md#listroutecalculatorspaginator)
3. item: [:material-code-braces: ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRouteCalculatorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRouteCalculatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef](./type_defs.md#listroutecalculatorsrequestlistroutecalculatorspaginatetypedef) 
## ListTrackerConsumersPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_tracker_consumers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListTrackerConsumersPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrackerConsumersResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListTrackerConsumersPaginator](./paginators.md#listtrackerconsumerspaginator)
3. item: [:material-code-braces: ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrackerConsumersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TrackerName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrackerConsumersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef](./type_defs.md#listtrackerconsumersrequestlisttrackerconsumerspaginatetypedef) 
## ListTrackersPaginator

Type annotations and code completion for `#!python session.client("location").get_paginator("list_trackers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_location.paginator import ListTrackersPaginator

session = Session()

session = get_session()
async with session.client("location") as client:  # (1)
    paginator: ListTrackersPaginator = client.get_paginator("list_trackers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrackersResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListTrackersPaginator](./paginators.md#listtrackerspaginator)
3. item: [:material-code-braces: ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrackersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrackersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTrackersRequestListTrackersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrackersRequestListTrackersPaginateTypeDef](./type_defs.md#listtrackersrequestlisttrackerspaginatetypedef) 
