# Examples

> [Index](../README.md) > [TrustedAdvisorPublicAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[trustedadvisor]` package installed.

Write your `TrustedAdvisorPublicAPI` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# TrustedAdvisorPublicAPIClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("trustedadvisor") as client:  # (1)
    result = await client.batch_update_recommendation_resource_exclusion()  # (2)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. result: [:material-code-braces: BatchUpdateRecommendationResourceExclusionResponseTypeDef](./type_defs.md#batchupdaterecommendationresourceexclusionresponsetypedef)



#### Paginator usage example

```python
# ListChecksPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("trustedadvisor") as client:  # (1)
    paginator = client.get_paginator("list_checks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListChecksPaginator](./paginators.md#listcheckspaginator)
3. item: [:material-code-braces: ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[trustedadvisor]`
or a standalone `types_aiobotocore_trustedadvisor` package, you have to explicitly specify
`client: TrustedAdvisorPublicAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# TrustedAdvisorPublicAPIClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_trustedadvisor.client import TrustedAdvisorPublicAPIClient
from types_aiobotocore_trustedadvisor.type_defs import BatchUpdateRecommendationResourceExclusionResponseTypeDef
from types_aiobotocore_trustedadvisor.type_defs import BatchUpdateRecommendationResourceExclusionRequestTypeDef


session = Session()

client: TrustedAdvisorPublicAPIClient
async with session.client("trustedadvisor") as client:  # (1)
    kwargs: BatchUpdateRecommendationResourceExclusionRequestTypeDef = {...}  # (2)
    result: BatchUpdateRecommendationResourceExclusionResponseTypeDef = await client.batch_update_recommendation_resource_exclusion(**kwargs)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. kwargs: [:material-code-braces: BatchUpdateRecommendationResourceExclusionRequestTypeDef](./type_defs.md#batchupdaterecommendationresourceexclusionrequesttypedef)
3. result: [:material-code-braces: BatchUpdateRecommendationResourceExclusionResponseTypeDef](./type_defs.md#batchupdaterecommendationresourceexclusionresponsetypedef)



#### Paginator usage example

```python
# ListChecksPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_trustedadvisor.client import TrustedAdvisorPublicAPIClient
from types_aiobotocore_trustedadvisor.paginator import ListChecksPaginator
from types_aiobotocore_trustedadvisor.type_defs import ListChecksResponseTypeDef


session = Session()

client: TrustedAdvisorPublicAPIClient
async with session.client("trustedadvisor") as client:  # (1)
    paginator: ListChecksPaginator = client.get_paginator("list_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListChecksPaginator](./paginators.md#listcheckspaginator)
3. item: [:material-code-braces: ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef)




