# Examples

> [Index](../README.md) > [WorkDocs](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkDocs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#workdocs)
    type annotations stubs module [types-aiobotocore-workdocs](https://pypi.org/project/types-aiobotocore-workdocs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workdocs]` package installed.

Write your `WorkDocs` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# WorkDocsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("workdocs") as client:  # (1)
    result = await client.abort_document_version_upload()  # (2)
```

1. client: [WorkDocsClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribeActivitiesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("workdocs") as client:  # (1)
    paginator = client.get_paginator("describe_activities")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeActivitiesPaginator](./paginators.md#describeactivitiespaginator)
3. item: [:material-code-braces: DescribeActivitiesResponseTypeDef](./type_defs.md#describeactivitiesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[workdocs]`
or a standalone `types_aiobotocore_workdocs` package, you have to explicitly specify
`client: WorkDocsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# WorkDocsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workdocs.client import WorkDocsClient
from types_aiobotocore_workdocs.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_workdocs.type_defs import AbortDocumentVersionUploadRequestTypeDef


session = Session()

client: WorkDocsClient
async with session.client("workdocs") as client:  # (1)
    kwargs: AbortDocumentVersionUploadRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.abort_document_version_upload(**kwargs)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. kwargs: [:material-code-braces: AbortDocumentVersionUploadRequestTypeDef](./type_defs.md#abortdocumentversionuploadrequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribeActivitiesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_workdocs.client import WorkDocsClient
from types_aiobotocore_workdocs.paginator import DescribeActivitiesPaginator
from types_aiobotocore_workdocs.type_defs import DescribeActivitiesResponseTypeDef


session = Session()

client: WorkDocsClient
async with session.client("workdocs") as client:  # (1)
    paginator: DescribeActivitiesPaginator = client.get_paginator("describe_activities")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeActivitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkDocsClient](./client.md)
2. paginator: [DescribeActivitiesPaginator](./paginators.md#describeactivitiespaginator)
3. item: [:material-code-braces: DescribeActivitiesResponseTypeDef](./type_defs.md#describeactivitiesresponsetypedef)




