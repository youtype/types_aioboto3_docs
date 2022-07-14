# Paginators

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## GetAppMonitorDataPaginator

Type annotations and code completion for `#!python session.client("rum").get_paginator("get_app_monitor_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator

session = Session()

session = get_session()
async with session.client("rum") as client:  # (1)
    paginator: GetAppMonitorDataPaginator = client.get_paginator("get_app_monitor_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetAppMonitorDataResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
3. item: [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAppMonitorDataPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Name: str,
    TimeRange: TimeRangeTypeDef,  # (1)
    Filters: Sequence[QueryFilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[GetAppMonitorDataResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef = {  # (1)
    "Name": ...,
    "TimeRange": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef](./type_defs.md#getappmonitordatarequestgetappmonitordatapaginatetypedef) 
## ListAppMonitorsPaginator

Type annotations and code completion for `#!python session.client("rum").get_paginator("list_app_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_rum.paginator import ListAppMonitorsPaginator

session = Session()

session = get_session()
async with session.client("rum") as client:  # (1)
    paginator: ListAppMonitorsPaginator = client.get_paginator("list_app_monitors")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppMonitorsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchRUMClient](./client.md)
2. paginator: [ListAppMonitorsPaginator](./paginators.md#listappmonitorspaginator)
3. item: [:material-code-braces: ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppMonitorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAppMonitorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppMonitorsRequestListAppMonitorsPaginateTypeDef](./type_defs.md#listappmonitorsrequestlistappmonitorspaginatetypedef) 
