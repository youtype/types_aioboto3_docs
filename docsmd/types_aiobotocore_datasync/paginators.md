# Paginators

> [Index](../README.md) > [DataSync](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## DescribeStorageSystemResourceMetricsPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("describe_storage_system_resource_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/DescribeStorageSystemResourceMetrics.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics)

```python
# DescribeStorageSystemResourceMetricsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import DescribeStorageSystemResourceMetricsPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator("describe_storage_system_resource_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStorageSystemResourceMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [DescribeStorageSystemResourceMetricsPaginator](./paginators.md#describestoragesystemresourcemetricspaginator)
3. item: `AioPageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeStorageSystemResourceMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DiscoveryJobArn: str,
    ResourceType: DiscoveryResourceTypeType,  # (1)
    ResourceId: str,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DiscoveryResourceTypeType](./literals.md#discoveryresourcetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStorageSystemResourceMetricsRequestPaginateTypeDef = {  # (1)
    "DiscoveryJobArn": ...,
    "ResourceType": ...,
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStorageSystemResourceMetricsRequestPaginateTypeDef](./type_defs.md#describestoragesystemresourcemetricsrequestpaginatetypedef)
## ListAgentsPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListAgents.html#DataSync.Paginator.ListAgents)

```python
# ListAgentsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListAgentsPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListAgentsPaginator = client.get_paginator("list_agents")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListAgentsPaginator](./paginators.md#listagentspaginator)
3. item: `AioPageIterator[ListAgentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentsRequestPaginateTypeDef](./type_defs.md#listagentsrequestpaginatetypedef)
## ListDiscoveryJobsPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_discovery_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListDiscoveryJobs.html#DataSync.Paginator.ListDiscoveryJobs)

```python
# ListDiscoveryJobsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListDiscoveryJobsPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListDiscoveryJobsPaginator = client.get_paginator("list_discovery_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoveryJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListDiscoveryJobsPaginator](./paginators.md#listdiscoveryjobspaginator)
3. item: `AioPageIterator[ListDiscoveryJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDiscoveryJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StorageSystemArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDiscoveryJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDiscoveryJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDiscoveryJobsRequestPaginateTypeDef = {  # (1)
    "StorageSystemArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoveryJobsRequestPaginateTypeDef](./type_defs.md#listdiscoveryjobsrequestpaginatetypedef)
## ListLocationsPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_locations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListLocations.html#DataSync.Paginator.ListLocations)

```python
# ListLocationsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListLocationsPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListLocationsPaginator = client.get_paginator("list_locations")  # (2)
    async for item in paginator.paginate(...):
        item: ListLocationsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListLocationsPaginator](./paginators.md#listlocationspaginator)
3. item: `AioPageIterator[ListLocationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[LocationFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListLocationsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[LocationFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListLocationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLocationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLocationsRequestPaginateTypeDef](./type_defs.md#listlocationsrequestpaginatetypedef)
## ListStorageSystemsPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_storage_systems")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListStorageSystems.html#DataSync.Paginator.ListStorageSystems)

```python
# ListStorageSystemsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListStorageSystemsPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListStorageSystemsPaginator = client.get_paginator("list_storage_systems")  # (2)
    async for item in paginator.paginate(...):
        item: ListStorageSystemsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListStorageSystemsPaginator](./paginators.md#liststoragesystemspaginator)
3. item: `AioPageIterator[ListStorageSystemsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStorageSystemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStorageSystemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStorageSystemsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStorageSystemsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStorageSystemsRequestPaginateTypeDef](./type_defs.md#liststoragesystemsrequestpaginatetypedef)
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListTagsForResource.html#DataSync.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListTagsForResourcePaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: `AioPageIterator[ListTagsForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
## ListTaskExecutionsPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_task_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListTaskExecutions.html#DataSync.Paginator.ListTaskExecutions)

```python
# ListTaskExecutionsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListTaskExecutionsPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListTaskExecutionsPaginator = client.get_paginator("list_task_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaskExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListTaskExecutionsPaginator](./paginators.md#listtaskexecutionspaginator)
3. item: `AioPageIterator[ListTaskExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTaskExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TaskArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTaskExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTaskExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTaskExecutionsRequestPaginateTypeDef = {  # (1)
    "TaskArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaskExecutionsRequestPaginateTypeDef](./type_defs.md#listtaskexecutionsrequestpaginatetypedef)
## ListTasksPaginator

Type annotations and code completion for `#!python session.client("datasync").get_paginator("list_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync/paginator/ListTasks.html#DataSync.Paginator.ListTasks)

```python
# ListTasksPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_datasync.paginator import ListTasksPaginator

session = Session()

session = get_session()
async with session.client("datasync") as client:  # (1)
    paginator: ListTasksPaginator = client.get_paginator("list_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [ListTasksPaginator](./paginators.md#listtaskspaginator)
3. item: `AioPageIterator[ListTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[TaskFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListTasksResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[TaskFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTasksRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTasksRequestPaginateTypeDef](./type_defs.md#listtasksrequestpaginatetypedef)
