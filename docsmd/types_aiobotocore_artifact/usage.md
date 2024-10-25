# Examples

> [Index](../README.md) > [Artifact](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[artifact]` package installed.

Write your `Artifact` code as usual,
type checking and code completion should work out of the box.



```python
# ArtifactClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("artifact") as client:  # (1)
    result = await client.get_report()  # (2)
```

1. client: [ArtifactClient](./client.md)
2. result: [:material-code-braces: GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef) 



```python
# ListReportsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("artifact") as client:  # (1)
    paginator = client.get_paginator("list_reports")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. paginator: [ListReportsPaginator](./paginators.md#listreportspaginator)
3. item: [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[artifact]`
or a standalone `types_aiobotocore_artifact` package, you have to explicitly specify
`client: ArtifactClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ArtifactClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_artifact.client import ArtifactClient
from types_aiobotocore_artifact.type_defs import GetReportResponseTypeDef
from types_aiobotocore_artifact.type_defs import GetReportRequestRequestTypeDef


session = Session()

client: ArtifactClient
async with session.client("artifact") as client:  # (1)
    kwargs: GetReportRequestRequestTypeDef = {...}  # (2)
    result: GetReportResponseTypeDef = await client.get_report(**kwargs)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. kwargs: [:material-code-braces: GetReportRequestRequestTypeDef](./type_defs.md#getreportrequestrequesttypedef) 
3. result: [:material-code-braces: GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef) 



```python
# ListReportsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_artifact.client import ArtifactClient
from types_aiobotocore_artifact.paginator import ListReportsPaginator
from types_aiobotocore_artifact.type_defs import ListReportsResponseTypeDef


session = Session()

client: ArtifactClient
async with session.client("artifact") as client:  # (1)
    paginator: ListReportsPaginator = client.get_paginator("list_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ArtifactClient](./client.md)
2. paginator: [ListReportsPaginator](./paginators.md#listreportspaginator)
3. item: [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 




