# Examples

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[evidently]` package installed.

Write your `CloudWatchEvidently` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudWatchEvidentlyClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("evidently") as client:  # (1)
    result = await client.batch_evaluate_feature()  # (2)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. result: [:material-code-braces: BatchEvaluateFeatureResponseTypeDef](./type_defs.md#batchevaluatefeatureresponsetypedef)



#### Paginator usage example

```python
# ListExperimentsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("evidently") as client:  # (1)
    paginator = client.get_paginator("list_experiments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
3. item: [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[evidently]`
or a standalone `types_aiobotocore_evidently` package, you have to explicitly specify
`client: CloudWatchEvidentlyClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudWatchEvidentlyClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient
from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureResponseTypeDef
from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureRequestTypeDef


session = Session()

client: CloudWatchEvidentlyClient
async with session.client("evidently") as client:  # (1)
    kwargs: BatchEvaluateFeatureRequestTypeDef = {...}  # (2)
    result: BatchEvaluateFeatureResponseTypeDef = await client.batch_evaluate_feature(**kwargs)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. kwargs: [:material-code-braces: BatchEvaluateFeatureRequestTypeDef](./type_defs.md#batchevaluatefeaturerequesttypedef)
3. result: [:material-code-braces: BatchEvaluateFeatureResponseTypeDef](./type_defs.md#batchevaluatefeatureresponsetypedef)



#### Paginator usage example

```python
# ListExperimentsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_evidently.client import CloudWatchEvidentlyClient
from types_aiobotocore_evidently.paginator import ListExperimentsPaginator
from types_aiobotocore_evidently.type_defs import ListExperimentsResponseTypeDef


session = Session()

client: CloudWatchEvidentlyClient
async with session.client("evidently") as client:  # (1)
    paginator: ListExperimentsPaginator = client.get_paginator("list_experiments")  # (2)
    async for item in paginator.paginate(...):
        item: ListExperimentsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
3. item: [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef)




