# Paginators

> [Index](../README.md) > [CostOptimizationHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).

## ListEnrollmentStatusesPaginator

Type annotations and code completion for `#!python session.client("cost-optimization-hub").get_paginator("list_enrollment_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListEnrollmentStatuses)

```python
# ListEnrollmentStatusesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cost_optimization_hub.paginator import ListEnrollmentStatusesPaginator

session = Session()

session = get_session()
async with session.client("cost-optimization-hub") as client:  # (1)
    paginator: ListEnrollmentStatusesPaginator = client.get_paginator("list_enrollment_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnrollmentStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListEnrollmentStatusesPaginator](./paginators.md#listenrollmentstatusespaginator)
3. item: [:material-code-braces: ListEnrollmentStatusesResponseTypeDef](./type_defs.md#listenrollmentstatusesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEnrollmentStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountId: str = ...,
    includeOrganizationInfo: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnrollmentStatusesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnrollmentStatusesResponseTypeDef](./type_defs.md#listenrollmentstatusesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef = {  # (1)
    "accountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnrollmentStatusesRequestListEnrollmentStatusesPaginateTypeDef](./type_defs.md#listenrollmentstatusesrequestlistenrollmentstatusespaginatetypedef) 
## ListRecommendationSummariesPaginator

Type annotations and code completion for `#!python session.client("cost-optimization-hub").get_paginator("list_recommendation_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListRecommendationSummaries)

```python
# ListRecommendationSummariesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cost_optimization_hub.paginator import ListRecommendationSummariesPaginator

session = Session()

session = get_session()
async with session.client("cost-optimization-hub") as client:  # (1)
    paginator: ListRecommendationSummariesPaginator = client.get_paginator("list_recommendation_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationSummariesResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListRecommendationSummariesPaginator](./paginators.md#listrecommendationsummariespaginator)
3. item: [:material-code-braces: ListRecommendationSummariesResponseTypeDef](./type_defs.md#listrecommendationsummariesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendationSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    groupBy: str,
    filter: FilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListRecommendationSummariesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRecommendationSummariesResponseTypeDef](./type_defs.md#listrecommendationsummariesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef = {  # (1)
    "groupBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationSummariesRequestListRecommendationSummariesPaginateTypeDef](./type_defs.md#listrecommendationsummariesrequestlistrecommendationsummariespaginatetypedef) 
## ListRecommendationsPaginator

Type annotations and code completion for `#!python session.client("cost-optimization-hub").get_paginator("list_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListRecommendations)

```python
# ListRecommendationsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_cost_optimization_hub.paginator import ListRecommendationsPaginator

session = Session()

session = get_session()
async with session.client("cost-optimization-hub") as client:  # (1)
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostOptimizationHubClient](./client.md)
2. paginator: [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
3. item: [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: FilterTypeDef = ...,  # (1)
    includeAllRecommendations: bool = ...,
    orderBy: OrderByTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListRecommendationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationsRequestListRecommendationsPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestListRecommendationsPaginateTypeDef](./type_defs.md#listrecommendationsrequestlistrecommendationspaginatetypedef) 
