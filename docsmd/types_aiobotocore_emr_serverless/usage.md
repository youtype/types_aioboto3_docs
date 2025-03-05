# Examples

> [Index](../README.md) > [EMRServerless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EMRServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#emrserverless)
    type annotations stubs module [types-aiobotocore-emr-serverless](https://pypi.org/project/types-aiobotocore-emr-serverless/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[emr-serverless]` package installed.

Write your `EMRServerless` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EMRServerlessClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("emr-serverless") as client:  # (1)
    result = await client.cancel_job_run()  # (2)
```

1. client: [EMRServerlessClient](./client.md)
2. result: [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("emr-serverless") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EMRServerlessClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[emr-serverless]`
or a standalone `types_aiobotocore_emr_serverless` package, you have to explicitly specify
`client: EMRServerlessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EMRServerlessClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_emr_serverless.client import EMRServerlessClient
from types_aiobotocore_emr_serverless.type_defs import CancelJobRunResponseTypeDef
from types_aiobotocore_emr_serverless.type_defs import CancelJobRunRequestTypeDef


session = Session()

client: EMRServerlessClient
async with session.client("emr-serverless") as client:  # (1)
    kwargs: CancelJobRunRequestTypeDef = {...}  # (2)
    result: CancelJobRunResponseTypeDef = await client.cancel_job_run(**kwargs)  # (3)
```

1. client: [EMRServerlessClient](./client.md)
2. kwargs: [:material-code-braces: CancelJobRunRequestTypeDef](./type_defs.md#canceljobrunrequesttypedef)
3. result: [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_emr_serverless.client import EMRServerlessClient
from types_aiobotocore_emr_serverless.paginator import ListApplicationsPaginator
from types_aiobotocore_emr_serverless.type_defs import ListApplicationsResponseTypeDef


session = Session()

client: EMRServerlessClient
async with session.client("emr-serverless") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [EMRServerlessClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)




