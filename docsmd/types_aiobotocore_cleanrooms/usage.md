# Examples

> [Index](../README.md) > [CleanRoomsService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#cleanroomsservice)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cleanrooms]` package installed.

Write your `CleanRoomsService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CleanRoomsServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("cleanrooms") as client:  # (1)
    result = await client.batch_get_collaboration_analysis_template()  # (2)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. result: [:material-code-braces: BatchGetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateoutputtypedef)



#### Paginator usage example

```python
# ListAnalysisTemplatesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("cleanrooms") as client:  # (1)
    paginator = client.get_paginator("list_analysis_templates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
3. item: [:material-code-braces: ListAnalysisTemplatesOutputTypeDef](./type_defs.md#listanalysistemplatesoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[cleanrooms]`
or a standalone `types_aiobotocore_cleanrooms` package, you have to explicitly specify
`client: CleanRoomsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CleanRoomsServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient
from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateOutputTypeDef
from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateInputTypeDef


session = Session()

client: CleanRoomsServiceClient
async with session.client("cleanrooms") as client:  # (1)
    kwargs: BatchGetCollaborationAnalysisTemplateInputTypeDef = {...}  # (2)
    result: BatchGetCollaborationAnalysisTemplateOutputTypeDef = await client.batch_get_collaboration_analysis_template(**kwargs)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetCollaborationAnalysisTemplateInputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateinputtypedef)
3. result: [:material-code-braces: BatchGetCollaborationAnalysisTemplateOutputTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateoutputtypedef)



#### Paginator usage example

```python
# ListAnalysisTemplatesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient
from types_aiobotocore_cleanrooms.paginator import ListAnalysisTemplatesPaginator
from types_aiobotocore_cleanrooms.type_defs import ListAnalysisTemplatesOutputTypeDef


session = Session()

client: CleanRoomsServiceClient
async with session.client("cleanrooms") as client:  # (1)
    paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalysisTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
3. item: [:material-code-braces: ListAnalysisTemplatesOutputTypeDef](./type_defs.md#listanalysistemplatesoutputtypedef)




