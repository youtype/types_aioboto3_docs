# Paginators

> [Index](../README.md) > [ForecastService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
    type annotations stubs module [types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

## ListDatasetGroupsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_dataset_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
3. item: [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestlistdatasetgroupspaginatetypedef) 
## ListDatasetImportJobsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_dataset_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListDatasetImportJobsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListDatasetImportJobsPaginator = client.get_paginator("list_dataset_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
3. item: [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetImportJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDatasetImportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestlistdatasetimportjobspaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListDatasetsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListExplainabilitiesPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_explainabilities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListExplainabilitiesPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListExplainabilitiesPaginator = client.get_paginator("list_explainabilities")  # (2)
    async for item in paginator.paginate(...):
        item: ListExplainabilitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListExplainabilitiesPaginator](./paginators.md#listexplainabilitiespaginator)
3. item: [:material-code-braces: ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExplainabilitiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListExplainabilitiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef](./type_defs.md#listexplainabilitiesrequestlistexplainabilitiespaginatetypedef) 
## ListExplainabilityExportsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_explainability_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListExplainabilityExportsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListExplainabilityExportsPaginator = client.get_paginator("list_explainability_exports")  # (2)
    async for item in paginator.paginate(...):
        item: ListExplainabilityExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListExplainabilityExportsPaginator](./paginators.md#listexplainabilityexportspaginator)
3. item: [:material-code-braces: ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExplainabilityExportsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListExplainabilityExportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef](./type_defs.md#listexplainabilityexportsrequestlistexplainabilityexportspaginatetypedef) 
## ListForecastExportJobsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_forecast_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListForecastExportJobsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListForecastExportJobsPaginator = client.get_paginator("list_forecast_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListForecastExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListForecastExportJobsPaginator](./paginators.md#listforecastexportjobspaginator)
3. item: [:material-code-braces: ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListForecastExportJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListForecastExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef](./type_defs.md#listforecastexportjobsrequestlistforecastexportjobspaginatetypedef) 
## ListForecastsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_forecasts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListForecastsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListForecastsPaginator = client.get_paginator("list_forecasts")  # (2)
    async for item in paginator.paginate(...):
        item: ListForecastsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListForecastsPaginator](./paginators.md#listforecastspaginator)
3. item: [:material-code-braces: ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListForecastsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListForecastsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListForecastsRequestListForecastsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListForecastsRequestListForecastsPaginateTypeDef](./type_defs.md#listforecastsrequestlistforecastspaginatetypedef) 
## ListMonitorEvaluationsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_monitor_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListMonitorEvaluationsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListMonitorEvaluationsPaginator = client.get_paginator("list_monitor_evaluations")  # (2)
    async for item in paginator.paginate(...):
        item: ListMonitorEvaluationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListMonitorEvaluationsPaginator](./paginators.md#listmonitorevaluationspaginator)
3. item: [:material-code-braces: ListMonitorEvaluationsResponseTypeDef](./type_defs.md#listmonitorevaluationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMonitorEvaluationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    MonitorArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListMonitorEvaluationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMonitorEvaluationsResponseTypeDef](./type_defs.md#listmonitorevaluationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = {  # (1)
    "MonitorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef](./type_defs.md#listmonitorevaluationsrequestlistmonitorevaluationspaginatetypedef) 
## ListMonitorsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListMonitorsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")  # (2)
    async for item in paginator.paginate(...):
        item: ListMonitorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
3. item: [:material-code-braces: ListMonitorsResponseTypeDef](./type_defs.md#listmonitorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMonitorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListMonitorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMonitorsResponseTypeDef](./type_defs.md#listmonitorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMonitorsRequestListMonitorsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitorsRequestListMonitorsPaginateTypeDef](./type_defs.md#listmonitorsrequestlistmonitorspaginatetypedef) 
## ListPredictorBacktestExportJobsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_predictor_backtest_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListPredictorBacktestExportJobsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListPredictorBacktestExportJobsPaginator = client.get_paginator("list_predictor_backtest_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListPredictorBacktestExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListPredictorBacktestExportJobsPaginator](./paginators.md#listpredictorbacktestexportjobspaginator)
3. item: [:material-code-braces: ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPredictorBacktestExportJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPredictorBacktestExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestlistpredictorbacktestexportjobspaginatetypedef) 
## ListPredictorsPaginator

Type annotations and code completion for `#!python session.client("forecast").get_paginator("list_predictors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_forecast.paginator import ListPredictorsPaginator

session = Session()

session = get_session()
async with session.client("forecast") as client:  # (1)
    paginator: ListPredictorsPaginator = client.get_paginator("list_predictors")  # (2)
    async for item in paginator.paginate(...):
        item: ListPredictorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListPredictorsPaginator](./paginators.md#listpredictorspaginator)
3. item: [:material-code-braces: ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPredictorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPredictorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPredictorsRequestListPredictorsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPredictorsRequestListPredictorsPaginateTypeDef](./type_defs.md#listpredictorsrequestlistpredictorspaginatetypedef) 
