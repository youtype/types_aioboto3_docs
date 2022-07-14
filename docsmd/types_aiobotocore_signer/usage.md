# Examples

> [Index](../README.md) > [signer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[signer]` package installed.

Write your `signer` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("signer") as client:  # (1)
        result = await client.add_profile_permission()  # (2)
    ```

    1. client: [signerClient](./client.md)
    2. result: [:material-code-braces: AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("signer") as client:  # (1)
        paginator = client.get_paginator("list_signing_jobs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [signerClient](./client.md)
    2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
    3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("signer") as client:  # (1)
        waiter = client.get_waiter("successful_signing_job")  # (2)
        await waiter.wait()
    ```

    1. client: [signerClient](./client.md)
    2. waiter: [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)


### Explicit type annotations

With `types-aioboto3-lite[signer]`
or a standalone `types_aiobotocore_signer` package, you have to explicitly specify
`client: signerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_signer.client import signerClient
    from types_aiobotocore_signer.type_defs import AddProfilePermissionResponseTypeDef
    from types_aiobotocore_signer.type_defs import AddProfilePermissionRequestRequestTypeDef


    session = Session()

    client: signerClient
    async with session.client("signer") as client:  # (1)
        kwargs: AddProfilePermissionRequestRequestTypeDef = {...}  # (2)
        result: AddProfilePermissionResponseTypeDef = await client.add_profile_permission(**kwargs)  # (3)
    ```

    1. client: [signerClient](./client.md)
    2. kwargs: [:material-code-braces: AddProfilePermissionRequestRequestTypeDef](./type_defs.md#addprofilepermissionrequestrequesttypedef) 
    3. result: [:material-code-braces: AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_signer.client import signerClient
    from types_aiobotocore_signer.paginator import ListSigningJobsPaginator
    from types_aiobotocore_signer.type_defs import ListSigningJobsResponseTypeDef


    session = Session()

    client: signerClient
    async with session.client("signer") as client:  # (1)
        paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")  # (2)
        async for item in paginator.paginate(...):
            item: ListSigningJobsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [signerClient](./client.md)
    2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
    3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_signer.client import signerClient
    from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter


    session = Session()

    async with session.client("signer") as client:  # (1)
        waiter = client.get_waiter("successful_signing_job")  # (2)
        await waiter.wait()
    ```

    1. client: [signerClient](./client.md)
    2. waiter: [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)


