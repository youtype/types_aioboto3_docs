# Examples

> [Index](../README.md) > [CloudTrail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#cloudtrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudtrail]` package installed.

Write your `CloudTrail` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudTrailClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudtrail") as client:  # (1)
    result = await client.cancel_query()  # (2)
```

1. client: [CloudTrailClient](./client.md)
2. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef)



#### Paginator usage example

```python
# ListImportFailuresPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudtrail") as client:  # (1)
    paginator = client.get_paginator("list_import_failures")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListImportFailuresPaginator](./paginators.md#listimportfailurespaginator)
3. item: [:material-code-braces: ListImportFailuresResponseTypeDef](./type_defs.md#listimportfailuresresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[cloudtrail]`
or a standalone `types_aiobotocore_cloudtrail` package, you have to explicitly specify
`client: CloudTrailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudTrailClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudtrail.client import CloudTrailClient
from types_aiobotocore_cloudtrail.type_defs import CancelQueryResponseTypeDef
from types_aiobotocore_cloudtrail.type_defs import CancelQueryRequestTypeDef


session = Session()

client: CloudTrailClient
async with session.client("cloudtrail") as client:  # (1)
    kwargs: CancelQueryRequestTypeDef = {...}  # (2)
    result: CancelQueryResponseTypeDef = await client.cancel_query(**kwargs)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. kwargs: [:material-code-braces: CancelQueryRequestTypeDef](./type_defs.md#cancelqueryrequesttypedef)
3. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef)



#### Paginator usage example

```python
# ListImportFailuresPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudtrail.client import CloudTrailClient
from types_aiobotocore_cloudtrail.paginator import ListImportFailuresPaginator
from types_aiobotocore_cloudtrail.type_defs import ListImportFailuresResponseTypeDef


session = Session()

client: CloudTrailClient
async with session.client("cloudtrail") as client:  # (1)
    paginator: ListImportFailuresPaginator = client.get_paginator("list_import_failures")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportFailuresResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudTrailClient](./client.md)
2. paginator: [ListImportFailuresPaginator](./paginators.md#listimportfailurespaginator)
3. item: [:material-code-braces: ListImportFailuresResponseTypeDef](./type_defs.md#listimportfailuresresponsetypedef)




