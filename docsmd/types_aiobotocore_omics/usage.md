# Examples

> [Index](../README.md) > [Omics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#omics)
    type annotations stubs module [types-aiobotocore-omics](https://pypi.org/project/types-aiobotocore-omics/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[omics]` package installed.

Write your `Omics` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# OmicsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("omics") as client:  # (1)
    result = await client.accept_share()  # (2)
```

1. client: [OmicsClient](./client.md)
2. result: [:material-code-braces: AcceptShareResponseTypeDef](./type_defs.md#acceptshareresponsetypedef)



#### Paginator usage example

```python
# ListAnnotationImportJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("omics") as client:  # (1)
    paginator = client.get_paginator("list_annotation_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OmicsClient](./client.md)
2. paginator: [ListAnnotationImportJobsPaginator](./paginators.md#listannotationimportjobspaginator)
3. item: [:material-code-braces: ListAnnotationImportJobsResponseTypeDef](./type_defs.md#listannotationimportjobsresponsetypedef)



#### Waiter usage example

```python
# AnnotationImportJobCreatedWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("omics") as client:  # (1)
    waiter = client.get_waiter("annotation_import_job_created")  # (2)
    await waiter.wait(...)
```

1. client: [OmicsClient](./client.md)
2. waiter: [AnnotationImportJobCreatedWaiter](./waiters.md#annotationimportjobcreatedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[omics]`
or a standalone `types_aiobotocore_omics` package, you have to explicitly specify
`client: OmicsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# OmicsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_omics.client import OmicsClient
from types_aiobotocore_omics.type_defs import AcceptShareResponseTypeDef
from types_aiobotocore_omics.type_defs import AcceptShareRequestTypeDef


session = Session()

client: OmicsClient
async with session.client("omics") as client:  # (1)
    kwargs: AcceptShareRequestTypeDef = {...}  # (2)
    result: AcceptShareResponseTypeDef = await client.accept_share(**kwargs)  # (3)
```

1. client: [OmicsClient](./client.md)
2. kwargs: [:material-code-braces: AcceptShareRequestTypeDef](./type_defs.md#acceptsharerequesttypedef)
3. result: [:material-code-braces: AcceptShareResponseTypeDef](./type_defs.md#acceptshareresponsetypedef)



#### Paginator usage example

```python
# ListAnnotationImportJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_omics.client import OmicsClient
from types_aiobotocore_omics.paginator import ListAnnotationImportJobsPaginator
from types_aiobotocore_omics.type_defs import ListAnnotationImportJobsResponseTypeDef


session = Session()

client: OmicsClient
async with session.client("omics") as client:  # (1)
    paginator: ListAnnotationImportJobsPaginator = client.get_paginator("list_annotation_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnnotationImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [OmicsClient](./client.md)
2. paginator: [ListAnnotationImportJobsPaginator](./paginators.md#listannotationimportjobspaginator)
3. item: [:material-code-braces: ListAnnotationImportJobsResponseTypeDef](./type_defs.md#listannotationimportjobsresponsetypedef)



#### Waiter usage example

```python
# AnnotationImportJobCreatedWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_omics.client import OmicsClient
from types_aiobotocore_omics.waiter import AnnotationImportJobCreatedWaiter


session = Session()

async with session.client("omics") as client:  # (1)
    waiter = client.get_waiter("annotation_import_job_created")  # (2)
    await waiter.wait(...)
```

1. client: [OmicsClient](./client.md)
2. waiter: [AnnotationImportJobCreatedWaiter](./waiters.md#annotationimportjobcreatedwaiter)


