# Examples

> [Index](../README.md) > [Signer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[signer]` package installed.

Write your `Signer` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SignerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("signer") as client:  # (1)
    result = await client.add_profile_permission()  # (2)
```

1. client: [SignerClient](./client.md)
2. result: [:material-code-braces: AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef)



#### Paginator usage example

```python
# ListSigningJobsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("signer") as client:  # (1)
    paginator = client.get_paginator("list_signing_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SignerClient](./client.md)
2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef)



#### Waiter usage example

```python
# SuccessfulSigningJobWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("signer") as client:  # (1)
    waiter = client.get_waiter("successful_signing_job")  # (2)
    await waiter.wait(...)
```

1. client: [SignerClient](./client.md)
2. waiter: [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)


### Explicit type annotations

With `types-aioboto3-lite[signer]`
or a standalone `types_aiobotocore_signer` package, you have to explicitly specify
`client: SignerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SignerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_signer.client import SignerClient
from types_aiobotocore_signer.type_defs import AddProfilePermissionResponseTypeDef
from types_aiobotocore_signer.type_defs import AddProfilePermissionRequestTypeDef


session = Session()

client: SignerClient
async with session.client("signer") as client:  # (1)
    kwargs: AddProfilePermissionRequestTypeDef = {...}  # (2)
    result: AddProfilePermissionResponseTypeDef = await client.add_profile_permission(**kwargs)  # (3)
```

1. client: [SignerClient](./client.md)
2. kwargs: [:material-code-braces: AddProfilePermissionRequestTypeDef](./type_defs.md#addprofilepermissionrequesttypedef)
3. result: [:material-code-braces: AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef)



#### Paginator usage example

```python
# ListSigningJobsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_signer.client import SignerClient
from types_aiobotocore_signer.paginator import ListSigningJobsPaginator
from types_aiobotocore_signer.type_defs import ListSigningJobsResponseTypeDef


session = Session()

client: SignerClient
async with session.client("signer") as client:  # (1)
    paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [SignerClient](./client.md)
2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef)



#### Waiter usage example

```python
# SuccessfulSigningJobWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_signer.client import SignerClient
from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter


session = Session()

async with session.client("signer") as client:  # (1)
    waiter = client.get_waiter("successful_signing_job")  # (2)
    await waiter.wait(...)
```

1. client: [SignerClient](./client.md)
2. waiter: [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)


