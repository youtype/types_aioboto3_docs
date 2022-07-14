# Paginators

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## DescribeAgentsPaginator

Type annotations and code completion for `#!python session.client("discovery").get_paginator("describe_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator

session = Session()

session = get_session()
async with session.client("discovery") as client:  # (1)
    paginator: DescribeAgentsPaginator = client.get_paginator("describe_agents")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
3. item: [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAgentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    agentIds: Sequence[str] = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeAgentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAgentsRequestDescribeAgentsPaginateTypeDef = {  # (1)
    "agentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAgentsRequestDescribeAgentsPaginateTypeDef](./type_defs.md#describeagentsrequestdescribeagentspaginatetypedef) 
## DescribeContinuousExportsPaginator

Type annotations and code completion for `#!python session.client("discovery").get_paginator("describe_continuous_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_discovery.paginator import DescribeContinuousExportsPaginator

session = Session()

session = get_session()
async with session.client("discovery") as client:  # (1)
    paginator: DescribeContinuousExportsPaginator = client.get_paginator("describe_continuous_exports")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeContinuousExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeContinuousExportsPaginator](./paginators.md#describecontinuousexportspaginator)
3. item: [:material-code-braces: DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeContinuousExportsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    exportIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeContinuousExportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = {  # (1)
    "exportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef](./type_defs.md#describecontinuousexportsrequestdescribecontinuousexportspaginatetypedef) 
## DescribeExportConfigurationsPaginator

Type annotations and code completion for `#!python session.client("discovery").get_paginator("describe_export_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_discovery.paginator import DescribeExportConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("discovery") as client:  # (1)
    paginator: DescribeExportConfigurationsPaginator = client.get_paginator("describe_export_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeExportConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeExportConfigurationsPaginator](./paginators.md#describeexportconfigurationspaginator)
3. item: [:material-code-braces: DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    exportIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeExportConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = {  # (1)
    "exportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef](./type_defs.md#describeexportconfigurationsrequestdescribeexportconfigurationspaginatetypedef) 
## DescribeExportTasksPaginator

Type annotations and code completion for `#!python session.client("discovery").get_paginator("describe_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_discovery.paginator import DescribeExportTasksPaginator

session = Session()

session = get_session()
async with session.client("discovery") as client:  # (1)
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeExportTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
3. item: [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    exportIds: Sequence[str] = ...,
    filters: Sequence[ExportFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ExportFilterTypeDef](./type_defs.md#exportfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = {  # (1)
    "exportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef](./type_defs.md#describeexporttasksrequestdescribeexporttaskspaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.client("discovery").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_discovery.paginator import DescribeTagsPaginator

session = Session()

session = get_session()
async with session.client("discovery") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[TagFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTagsRequestDescribeTagsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestDescribeTagsPaginateTypeDef](./type_defs.md#describetagsrequestdescribetagspaginatetypedef) 
## ListConfigurationsPaginator

Type annotations and code completion for `#!python session.client("discovery").get_paginator("list_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_discovery.paginator import ListConfigurationsPaginator

session = Session()

session = get_session()
async with session.client("discovery") as client:  # (1)
    paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
3. item: [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    configurationType: ConfigurationItemTypeType,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    orderBy: Sequence[OrderByElementTypeDef] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListConfigurationsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ConfigurationItemTypeType](./literals.md#configurationitemtypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConfigurationsRequestListConfigurationsPaginateTypeDef = {  # (1)
    "configurationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationsRequestListConfigurationsPaginateTypeDef](./type_defs.md#listconfigurationsrequestlistconfigurationspaginatetypedef) 
