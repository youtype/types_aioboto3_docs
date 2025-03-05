# Examples

> [Index](../README.md) > [ResilienceHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#resiliencehub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[resiliencehub]` package installed.

Write your `ResilienceHub` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ResilienceHubClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("resiliencehub") as client:  # (1)
    result = await client.accept_resource_grouping_recommendations()  # (2)
```

1. client: [ResilienceHubClient](./client.md)
2. result: [:material-code-braces: AcceptResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsresponsetypedef)



#### Paginator usage example

```python
# ListAppAssessmentResourceDriftsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("resiliencehub") as client:  # (1)
    paginator = client.get_paginator("list_app_assessment_resource_drifts")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResilienceHubClient](./client.md)
2. paginator: [ListAppAssessmentResourceDriftsPaginator](./paginators.md#listappassessmentresourcedriftspaginator)
3. item: [:material-code-braces: ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[resiliencehub]`
or a standalone `types_aiobotocore_resiliencehub` package, you have to explicitly specify
`client: ResilienceHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ResilienceHubClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_resiliencehub.client import ResilienceHubClient
from types_aiobotocore_resiliencehub.type_defs import AcceptResourceGroupingRecommendationsResponseTypeDef
from types_aiobotocore_resiliencehub.type_defs import AcceptResourceGroupingRecommendationsRequestTypeDef


session = Session()

client: ResilienceHubClient
async with session.client("resiliencehub") as client:  # (1)
    kwargs: AcceptResourceGroupingRecommendationsRequestTypeDef = {...}  # (2)
    result: AcceptResourceGroupingRecommendationsResponseTypeDef = await client.accept_resource_grouping_recommendations(**kwargs)  # (3)
```

1. client: [ResilienceHubClient](./client.md)
2. kwargs: [:material-code-braces: AcceptResourceGroupingRecommendationsRequestTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsrequesttypedef)
3. result: [:material-code-braces: AcceptResourceGroupingRecommendationsResponseTypeDef](./type_defs.md#acceptresourcegroupingrecommendationsresponsetypedef)



#### Paginator usage example

```python
# ListAppAssessmentResourceDriftsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_resiliencehub.client import ResilienceHubClient
from types_aiobotocore_resiliencehub.paginator import ListAppAssessmentResourceDriftsPaginator
from types_aiobotocore_resiliencehub.type_defs import ListAppAssessmentResourceDriftsResponseTypeDef


session = Session()

client: ResilienceHubClient
async with session.client("resiliencehub") as client:  # (1)
    paginator: ListAppAssessmentResourceDriftsPaginator = client.get_paginator("list_app_assessment_resource_drifts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppAssessmentResourceDriftsResponseTypeDef
        print(item)  # (3)
```

1. client: [ResilienceHubClient](./client.md)
2. paginator: [ListAppAssessmentResourceDriftsPaginator](./paginators.md#listappassessmentresourcedriftspaginator)
3. item: [:material-code-braces: ListAppAssessmentResourceDriftsResponseTypeDef](./type_defs.md#listappassessmentresourcedriftsresponsetypedef)




