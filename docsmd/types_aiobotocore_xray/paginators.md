# Paginators

> [Index](../README.md) > [XRay](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## BatchGetTracesPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("batch_get_traces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import BatchGetTracesPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")  # (2)
    async for item in paginator.paginate(...):
        item: BatchGetTracesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
3. item: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 


### paginate

Type annotations and code completion for `#!python BatchGetTracesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TraceIds: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[BatchGetTracesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: BatchGetTracesRequestBatchGetTracesPaginateTypeDef = {  # (1)
    "TraceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: BatchGetTracesRequestBatchGetTracesPaginateTypeDef](./type_defs.md#batchgettracesrequestbatchgettracespaginatetypedef) 
## GetGroupsPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetGroupsPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetGroupsPaginator = client.get_paginator("get_groups")  # (2)
    async for item in paginator.paginate(...):
        item: GetGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetGroupsPaginator](./paginators.md#getgroupspaginator)
3. item: [:material-code-braces: GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetGroupsResultTypeDef](./type_defs.md#getgroupsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetGroupsRequestGetGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGroupsRequestGetGroupsPaginateTypeDef](./type_defs.md#getgroupsrequestgetgroupspaginatetypedef) 
## GetSamplingRulesPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_sampling_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetSamplingRulesPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetSamplingRulesPaginator = client.get_paginator("get_sampling_rules")  # (2)
    async for item in paginator.paginate(...):
        item: GetSamplingRulesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetSamplingRulesPaginator](./paginators.md#getsamplingrulespaginator)
3. item: [:material-code-braces: GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetSamplingRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSamplingRulesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSamplingRulesResultTypeDef](./type_defs.md#getsamplingrulesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef](./type_defs.md#getsamplingrulesrequestgetsamplingrulespaginatetypedef) 
## GetSamplingStatisticSummariesPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_sampling_statistic_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetSamplingStatisticSummariesPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetSamplingStatisticSummariesPaginator = client.get_paginator("get_sampling_statistic_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: GetSamplingStatisticSummariesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetSamplingStatisticSummariesPaginator](./paginators.md#getsamplingstatisticsummariespaginator)
3. item: [:material-code-braces: GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetSamplingStatisticSummariesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSamplingStatisticSummariesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSamplingStatisticSummariesResultTypeDef](./type_defs.md#getsamplingstatisticsummariesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef](./type_defs.md#getsamplingstatisticsummariesrequestgetsamplingstatisticsummariespaginatetypedef) 
## GetServiceGraphPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_service_graph")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetServiceGraphPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetServiceGraphPaginator = client.get_paginator("get_service_graph")  # (2)
    async for item in paginator.paginate(...):
        item: GetServiceGraphResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetServiceGraphPaginator](./paginators.md#getservicegraphpaginator)
3. item: [:material-code-braces: GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetServiceGraphPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    GroupName: str = ...,
    GroupARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetServiceGraphResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetServiceGraphResultTypeDef](./type_defs.md#getservicegraphresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceGraphRequestGetServiceGraphPaginateTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetServiceGraphRequestGetServiceGraphPaginateTypeDef](./type_defs.md#getservicegraphrequestgetservicegraphpaginatetypedef) 
## GetTimeSeriesServiceStatisticsPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_time_series_service_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetTimeSeriesServiceStatisticsPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")  # (2)
    async for item in paginator.paginate(...):
        item: GetTimeSeriesServiceStatisticsResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetTimeSeriesServiceStatisticsPaginator](./paginators.md#gettimeseriesservicestatisticspaginator)
3. item: [:material-code-braces: GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTimeSeriesServiceStatisticsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    GroupName: str = ...,
    GroupARN: str = ...,
    EntitySelectorExpression: str = ...,
    Period: int = ...,
    ForecastStatistics: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTimeSeriesServiceStatisticsResultTypeDef](./type_defs.md#gettimeseriesservicestatisticsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef](./type_defs.md#gettimeseriesservicestatisticsrequestgettimeseriesservicestatisticspaginatetypedef) 
## GetTraceGraphPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_trace_graph")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetTraceGraphPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")  # (2)
    async for item in paginator.paginate(...):
        item: GetTraceGraphResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetTraceGraphPaginator](./paginators.md#gettracegraphpaginator)
3. item: [:material-code-braces: GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTraceGraphPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TraceIds: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTraceGraphResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTraceGraphResultTypeDef](./type_defs.md#gettracegraphresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTraceGraphRequestGetTraceGraphPaginateTypeDef = {  # (1)
    "TraceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTraceGraphRequestGetTraceGraphPaginateTypeDef](./type_defs.md#gettracegraphrequestgettracegraphpaginatetypedef) 
## GetTraceSummariesPaginator

Type annotations and code completion for `#!python session.client("xray").get_paginator("get_trace_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_xray.paginator import GetTraceSummariesPaginator

session = Session()

session = get_session()
async with session.client("xray") as client:  # (1)
    paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: GetTraceSummariesResultTypeDef
        print(item)  # (3)
```

1. client: [XRayClient](./client.md)
2. paginator: [GetTraceSummariesPaginator](./paginators.md#gettracesummariespaginator)
3. item: [:material-code-braces: GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTraceSummariesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    TimeRangeType: TimeRangeTypeType = ...,  # (1)
    Sampling: bool = ...,
    SamplingStrategy: SamplingStrategyTypeDef = ...,  # (2)
    FilterExpression: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[GetTraceSummariesResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: TimeRangeTypeType](./literals.md#timerangetypetype) 
2. See [:material-code-braces: SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetTraceSummariesResultTypeDef](./type_defs.md#gettracesummariesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef](./type_defs.md#gettracesummariesrequestgettracesummariespaginatetypedef) 
