# CostOptimizationHubClient

> [Index](../README.md) > [CostOptimizationHub](./README.md) > CostOptimizationHubClient

!!! note ""

    Auto-generated documentation for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#costoptimizationhub)
    type annotations stubs module [types-aiobotocore-cost-optimization-hub](https://pypi.org/project/types-aiobotocore-cost-optimization-hub/).

## CostOptimizationHubClient

Type annotations and code completion for `#!python session.client("cost-optimization-hub")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# CostOptimizationHubClient usage example

from aioboto3.session import Session
from types_aiobotocore_cost_optimization_hub.client import CostOptimizationHubClient

session = Session()
async with session.client("cost-optimization-hub") as client:
    client: CostOptimizationHubClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("cost-optimization-hub").exceptions` structure.

```python
# CostOptimizationHubClient.exceptions usage example

async with session.client("cost-optimization-hub") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# CostOptimizationHubClient.exceptions type checking example

from types_aiobotocore_cost_optimization_hub.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("cost-optimization-hub").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("cost-optimization-hub").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_preferences

Returns a set of preferences for an account in order to add account-specific
preferences into the service.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").get_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# get_preferences method definition

await def get_preferences(
    self,
) -> GetPreferencesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPreferencesResponseTypeDef](./type_defs.md#getpreferencesresponsetypedef) 

### get\_recommendation

Returns both the current and recommended resource configuration and the
estimated cost impact for a recommendation.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").get_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# get_recommendation method definition

await def get_recommendation(
    self,
    *,
    recommendationId: str,
) -> GetRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef) 


```python
# get_recommendation method usage example with argument unpacking

kwargs: GetRecommendationRequestRequestTypeDef = {  # (1)
    "recommendationId": ...,
}

parent.get_recommendation(**kwargs)
```

1. See [:material-code-braces: GetRecommendationRequestRequestTypeDef](./type_defs.md#getrecommendationrequestrequesttypedef) 

### list\_enrollment\_statuses

Retrieves the enrollment status for an account.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").list_enrollment_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# list_enrollment_statuses method definition

await def list_enrollment_statuses(
    self,
    *,
    includeOrganizationInfo: bool = ...,
    accountId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEnrollmentStatusesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnrollmentStatusesResponseTypeDef](./type_defs.md#listenrollmentstatusesresponsetypedef) 


```python
# list_enrollment_statuses method usage example with argument unpacking

kwargs: ListEnrollmentStatusesRequestRequestTypeDef = {  # (1)
    "includeOrganizationInfo": ...,
}

parent.list_enrollment_statuses(**kwargs)
```

1. See [:material-code-braces: ListEnrollmentStatusesRequestRequestTypeDef](./type_defs.md#listenrollmentstatusesrequestrequesttypedef) 

### list\_recommendation\_summaries

Returns a concise representation of savings estimates for resources.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").list_recommendation_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# list_recommendation_summaries method definition

await def list_recommendation_summaries(
    self,
    *,
    groupBy: str,
    filter: FilterTypeDef = ...,  # (1)
    maxResults: int = ...,
    metrics: Sequence[SummaryMetricsType] = ...,  # (2)
    nextToken: str = ...,
) -> ListRecommendationSummariesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SummaryMetricsType](./literals.md#summarymetricstype) 
3. See [:material-code-braces: ListRecommendationSummariesResponseTypeDef](./type_defs.md#listrecommendationsummariesresponsetypedef) 


```python
# list_recommendation_summaries method usage example with argument unpacking

kwargs: ListRecommendationSummariesRequestRequestTypeDef = {  # (1)
    "groupBy": ...,
}

parent.list_recommendation_summaries(**kwargs)
```

1. See [:material-code-braces: ListRecommendationSummariesRequestRequestTypeDef](./type_defs.md#listrecommendationsummariesrequestrequesttypedef) 

### list\_recommendations

Returns a list of recommendations.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# list_recommendations method definition

await def list_recommendations(
    self,
    *,
    filter: FilterTypeDef = ...,  # (1)
    orderBy: OrderByTypeDef = ...,  # (2)
    includeAllRecommendations: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListRecommendationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: OrderByTypeDef](./type_defs.md#orderbytypedef) 
3. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python
# list_recommendations method usage example with argument unpacking

kwargs: ListRecommendationsRequestRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestRequestTypeDef](./type_defs.md#listrecommendationsrequestrequesttypedef) 

### update\_enrollment\_status

Updates the enrollment (opt in and opt out) status of an account to the Cost
Optimization Hub service.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").update_enrollment_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# update_enrollment_status method definition

await def update_enrollment_status(
    self,
    *,
    status: EnrollmentStatusType,  # (1)
    includeMemberAccounts: bool = ...,
) -> UpdateEnrollmentStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EnrollmentStatusType](./literals.md#enrollmentstatustype) 
2. See [:material-code-braces: UpdateEnrollmentStatusResponseTypeDef](./type_defs.md#updateenrollmentstatusresponsetypedef) 


```python
# update_enrollment_status method usage example with argument unpacking

kwargs: UpdateEnrollmentStatusRequestRequestTypeDef = {  # (1)
    "status": ...,
}

parent.update_enrollment_status(**kwargs)
```

1. See [:material-code-braces: UpdateEnrollmentStatusRequestRequestTypeDef](./type_defs.md#updateenrollmentstatusrequestrequesttypedef) 

### update\_preferences

Updates a set of preferences for an account in order to add account-specific
preferences into the service.

Type annotations and code completion for `#!python session.client("cost-optimization-hub").update_preferences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# update_preferences method definition

await def update_preferences(
    self,
    *,
    savingsEstimationMode: SavingsEstimationModeType = ...,  # (1)
    memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType = ...,  # (2)
) -> UpdatePreferencesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SavingsEstimationModeType](./literals.md#savingsestimationmodetype) 
2. See [:material-code-brackets: MemberAccountDiscountVisibilityType](./literals.md#memberaccountdiscountvisibilitytype) 
3. See [:material-code-braces: UpdatePreferencesResponseTypeDef](./type_defs.md#updatepreferencesresponsetypedef) 


```python
# update_preferences method usage example with argument unpacking

kwargs: UpdatePreferencesRequestRequestTypeDef = {  # (1)
    "savingsEstimationMode": ...,
}

parent.update_preferences(**kwargs)
```

1. See [:material-code-braces: UpdatePreferencesRequestRequestTypeDef](./type_defs.md#updatepreferencesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("cost-optimization-hub").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("cost-optimization-hub").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("cost-optimization-hub").get_paginator` method with overloads.

- `client.get_paginator("list_enrollment_statuses")` -> [ListEnrollmentStatusesPaginator](./paginators.md#listenrollmentstatusespaginator)
- `client.get_paginator("list_recommendation_summaries")` -> [ListRecommendationSummariesPaginator](./paginators.md#listrecommendationsummariespaginator)
- `client.get_paginator("list_recommendations")` -> [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)


