# Paginators

> [Index](../README.md) > [GroundStation](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## ListConfigsPaginator

Type annotations and code completion for `#!python session.client("groundstation").get_paginator("list_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_groundstation.paginator import ListConfigsPaginator

session = Session()

session = get_session()
async with session.client("groundstation") as client:  # (1)
    paginator: ListConfigsPaginator = client.get_paginator("list_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListConfigsPaginator](./paginators.md#listconfigspaginator)
3. item: [:material-code-braces: ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConfigsRequestListConfigsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigsRequestListConfigsPaginateTypeDef](./type_defs.md#listconfigsrequestlistconfigspaginatetypedef) 
## ListContactsPaginator

Type annotations and code completion for `#!python session.client("groundstation").get_paginator("list_contacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_groundstation.paginator import ListContactsPaginator

session = Session()

session = get_session()
async with session.client("groundstation") as client:  # (1)
    paginator: ListContactsPaginator = client.get_paginator("list_contacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListContactsPaginator](./paginators.md#listcontactspaginator)
3. item: [:material-code-braces: ListContactsResponseTypeDef](./type_defs.md#listcontactsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListContactsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    endTime: Union[datetime, str],
    startTime: Union[datetime, str],
    statusList: Sequence[ContactStatusType],  # (1)
    groundStation: str = ...,
    missionProfileArn: str = ...,
    satelliteArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListContactsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContactStatusType](./literals.md#contactstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListContactsResponseTypeDef](./type_defs.md#listcontactsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListContactsRequestListContactsPaginateTypeDef = {  # (1)
    "endTime": ...,
    "startTime": ...,
    "statusList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactsRequestListContactsPaginateTypeDef](./type_defs.md#listcontactsrequestlistcontactspaginatetypedef) 
## ListDataflowEndpointGroupsPaginator

Type annotations and code completion for `#!python session.client("groundstation").get_paginator("list_dataflow_endpoint_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_groundstation.paginator import ListDataflowEndpointGroupsPaginator

session = Session()

session = get_session()
async with session.client("groundstation") as client:  # (1)
    paginator: ListDataflowEndpointGroupsPaginator = client.get_paginator("list_dataflow_endpoint_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataflowEndpointGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListDataflowEndpointGroupsPaginator](./paginators.md#listdataflowendpointgroupspaginator)
3. item: [:material-code-braces: ListDataflowEndpointGroupsResponseTypeDef](./type_defs.md#listdataflowendpointgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataflowEndpointGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataflowEndpointGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataflowEndpointGroupsResponseTypeDef](./type_defs.md#listdataflowendpointgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef](./type_defs.md#listdataflowendpointgroupsrequestlistdataflowendpointgroupspaginatetypedef) 
## ListGroundStationsPaginator

Type annotations and code completion for `#!python session.client("groundstation").get_paginator("list_ground_stations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_groundstation.paginator import ListGroundStationsPaginator

session = Session()

session = get_session()
async with session.client("groundstation") as client:  # (1)
    paginator: ListGroundStationsPaginator = client.get_paginator("list_ground_stations")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroundStationsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListGroundStationsPaginator](./paginators.md#listgroundstationspaginator)
3. item: [:material-code-braces: ListGroundStationsResponseTypeDef](./type_defs.md#listgroundstationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroundStationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    satelliteId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGroundStationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroundStationsResponseTypeDef](./type_defs.md#listgroundstationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroundStationsRequestListGroundStationsPaginateTypeDef = {  # (1)
    "satelliteId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroundStationsRequestListGroundStationsPaginateTypeDef](./type_defs.md#listgroundstationsrequestlistgroundstationspaginatetypedef) 
## ListMissionProfilesPaginator

Type annotations and code completion for `#!python session.client("groundstation").get_paginator("list_mission_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_groundstation.paginator import ListMissionProfilesPaginator

session = Session()

session = get_session()
async with session.client("groundstation") as client:  # (1)
    paginator: ListMissionProfilesPaginator = client.get_paginator("list_mission_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListMissionProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListMissionProfilesPaginator](./paginators.md#listmissionprofilespaginator)
3. item: [:material-code-braces: ListMissionProfilesResponseTypeDef](./type_defs.md#listmissionprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMissionProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMissionProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMissionProfilesResponseTypeDef](./type_defs.md#listmissionprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMissionProfilesRequestListMissionProfilesPaginateTypeDef](./type_defs.md#listmissionprofilesrequestlistmissionprofilespaginatetypedef) 
## ListSatellitesPaginator

Type annotations and code completion for `#!python session.client("groundstation").get_paginator("list_satellites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_groundstation.paginator import ListSatellitesPaginator

session = Session()

session = get_session()
async with session.client("groundstation") as client:  # (1)
    paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")  # (2)
    async for item in paginator.paginate(...):
        item: ListSatellitesResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListSatellitesPaginator](./paginators.md#listsatellitespaginator)
3. item: [:material-code-braces: ListSatellitesResponseTypeDef](./type_defs.md#listsatellitesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSatellitesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSatellitesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSatellitesResponseTypeDef](./type_defs.md#listsatellitesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSatellitesRequestListSatellitesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSatellitesRequestListSatellitesPaginateTypeDef](./type_defs.md#listsatellitesrequestlistsatellitespaginatetypedef) 
