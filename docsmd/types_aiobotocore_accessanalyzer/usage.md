# Examples

> [Index](../README.md) > [AccessAnalyzer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#accessanalyzer)
    type annotations stubs module [types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[accessanalyzer]` package installed.

Write your `AccessAnalyzer` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AccessAnalyzerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("accessanalyzer") as client:  # (1)
    result = await client.apply_archive_rule()  # (2)
```

1. client: [AccessAnalyzerClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# GetFindingRecommendationPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("accessanalyzer") as client:  # (1)
    paginator = client.get_paginator("get_finding_recommendation")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [GetFindingRecommendationPaginator](./paginators.md#getfindingrecommendationpaginator)
3. item: [:material-code-braces: GetFindingRecommendationResponseTypeDef](./type_defs.md#getfindingrecommendationresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[accessanalyzer]`
or a standalone `types_aiobotocore_accessanalyzer` package, you have to explicitly specify
`client: AccessAnalyzerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AccessAnalyzerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient
from types_aiobotocore_accessanalyzer.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_accessanalyzer.type_defs import ApplyArchiveRuleRequestTypeDef


session = Session()

client: AccessAnalyzerClient
async with session.client("accessanalyzer") as client:  # (1)
    kwargs: ApplyArchiveRuleRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.apply_archive_rule(**kwargs)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. kwargs: [:material-code-braces: ApplyArchiveRuleRequestTypeDef](./type_defs.md#applyarchiverulerequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# GetFindingRecommendationPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient
from types_aiobotocore_accessanalyzer.paginator import GetFindingRecommendationPaginator
from types_aiobotocore_accessanalyzer.type_defs import GetFindingRecommendationResponseTypeDef


session = Session()

client: AccessAnalyzerClient
async with session.client("accessanalyzer") as client:  # (1)
    paginator: GetFindingRecommendationPaginator = client.get_paginator("get_finding_recommendation")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingRecommendationResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [GetFindingRecommendationPaginator](./paginators.md#getfindingrecommendationpaginator)
3. item: [:material-code-braces: GetFindingRecommendationResponseTypeDef](./type_defs.md#getfindingrecommendationresponsetypedef)




