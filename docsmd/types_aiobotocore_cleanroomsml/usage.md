# Examples

> [Index](../README.md) > [CleanRoomsML](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cleanroomsml]` package installed.

Write your `CleanRoomsML` code as usual,
type checking and code completion should work out of the box.



```python
# CleanRoomsMLClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("cleanroomsml") as client:  # (1)
    result = await client.create_audience_model()  # (2)
```

1. client: [CleanRoomsMLClient](./client.md)
2. result: [:material-code-braces: CreateAudienceModelResponseTypeDef](./type_defs.md#createaudiencemodelresponsetypedef) 



```python
# ListAudienceExportJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("cleanroomsml") as client:  # (1)
    paginator = client.get_paginator("list_audience_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListAudienceExportJobsPaginator](./paginators.md#listaudienceexportjobspaginator)
3. item: [:material-code-braces: ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cleanroomsml]`
or a standalone `types_aiobotocore_cleanroomsml` package, you have to explicitly specify
`client: CleanRoomsMLClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CleanRoomsMLClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cleanroomsml.client import CleanRoomsMLClient
from types_aiobotocore_cleanroomsml.type_defs import CreateAudienceModelResponseTypeDef
from types_aiobotocore_cleanroomsml.type_defs import CreateAudienceModelRequestRequestTypeDef


session = Session()

client: CleanRoomsMLClient
async with session.client("cleanroomsml") as client:  # (1)
    kwargs: CreateAudienceModelRequestRequestTypeDef = {...}  # (2)
    result: CreateAudienceModelResponseTypeDef = await client.create_audience_model(**kwargs)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. kwargs: [:material-code-braces: CreateAudienceModelRequestRequestTypeDef](./type_defs.md#createaudiencemodelrequestrequesttypedef) 
3. result: [:material-code-braces: CreateAudienceModelResponseTypeDef](./type_defs.md#createaudiencemodelresponsetypedef) 



```python
# ListAudienceExportJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cleanroomsml.client import CleanRoomsMLClient
from types_aiobotocore_cleanroomsml.paginator import ListAudienceExportJobsPaginator
from types_aiobotocore_cleanroomsml.type_defs import ListAudienceExportJobsResponseTypeDef


session = Session()

client: CleanRoomsMLClient
async with session.client("cleanroomsml") as client:  # (1)
    paginator: ListAudienceExportJobsPaginator = client.get_paginator("list_audience_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAudienceExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListAudienceExportJobsPaginator](./paginators.md#listaudienceexportjobspaginator)
3. item: [:material-code-braces: ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef) 




