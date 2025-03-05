# Examples

> [Index](../README.md) > [Comprehend](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[comprehend]` package installed.

Write your `Comprehend` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ComprehendClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("comprehend") as client:  # (1)
    result = await client.batch_detect_dominant_language()  # (2)
```

1. client: [ComprehendClient](./client.md)
2. result: [:material-code-braces: BatchDetectDominantLanguageResponseTypeDef](./type_defs.md#batchdetectdominantlanguageresponsetypedef)



#### Paginator usage example

```python
# ListDocumentClassificationJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("comprehend") as client:  # (1)
    paginator = client.get_paginator("list_document_classification_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
3. item: [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[comprehend]`
or a standalone `types_aiobotocore_comprehend` package, you have to explicitly specify
`client: ComprehendClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ComprehendClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_comprehend.client import ComprehendClient
from types_aiobotocore_comprehend.type_defs import BatchDetectDominantLanguageResponseTypeDef
from types_aiobotocore_comprehend.type_defs import BatchDetectDominantLanguageRequestTypeDef


session = Session()

client: ComprehendClient
async with session.client("comprehend") as client:  # (1)
    kwargs: BatchDetectDominantLanguageRequestTypeDef = {...}  # (2)
    result: BatchDetectDominantLanguageResponseTypeDef = await client.batch_detect_dominant_language(**kwargs)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. kwargs: [:material-code-braces: BatchDetectDominantLanguageRequestTypeDef](./type_defs.md#batchdetectdominantlanguagerequesttypedef)
3. result: [:material-code-braces: BatchDetectDominantLanguageResponseTypeDef](./type_defs.md#batchdetectdominantlanguageresponsetypedef)



#### Paginator usage example

```python
# ListDocumentClassificationJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_comprehend.client import ComprehendClient
from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator
from types_aiobotocore_comprehend.type_defs import ListDocumentClassificationJobsResponseTypeDef


session = Session()

client: ComprehendClient
async with session.client("comprehend") as client:  # (1)
    paginator: ListDocumentClassificationJobsPaginator = client.get_paginator("list_document_classification_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDocumentClassificationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
3. item: [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef)




