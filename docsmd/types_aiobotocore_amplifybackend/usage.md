# Examples

> [Index](../README.md) > [AmplifyBackend](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
    type annotations stubs module [types-aiobotocore-amplifybackend](https://pypi.org/project/types-aiobotocore-amplifybackend/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[amplifybackend]` package installed.

Write your `AmplifyBackend` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("amplifybackend") as client:  # (1)
        result = await client.clone_backend()  # (2)
    ```

    1. client: [AmplifyBackendClient](./client.md)
    2. result: [:material-code-braces: CloneBackendResponseTypeDef](./type_defs.md#clonebackendresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("amplifybackend") as client:  # (1)
        paginator = client.get_paginator("list_backend_jobs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AmplifyBackendClient](./client.md)
    2. paginator: [ListBackendJobsPaginator](./paginators.md#listbackendjobspaginator)
    3. item: [:material-code-braces: ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[amplifybackend]`
or a standalone `types_aiobotocore_amplifybackend` package, you have to explicitly specify
`client: AmplifyBackendClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_amplifybackend.client import AmplifyBackendClient
    from types_aiobotocore_amplifybackend.type_defs import CloneBackendResponseTypeDef
    from types_aiobotocore_amplifybackend.type_defs import CloneBackendRequestRequestTypeDef


    session = Session()

    client: AmplifyBackendClient
    async with session.client("amplifybackend") as client:  # (1)
        kwargs: CloneBackendRequestRequestTypeDef = {...}  # (2)
        result: CloneBackendResponseTypeDef = await client.clone_backend(**kwargs)  # (3)
    ```

    1. client: [AmplifyBackendClient](./client.md)
    2. kwargs: [:material-code-braces: CloneBackendRequestRequestTypeDef](./type_defs.md#clonebackendrequestrequesttypedef) 
    3. result: [:material-code-braces: CloneBackendResponseTypeDef](./type_defs.md#clonebackendresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_amplifybackend.client import AmplifyBackendClient
    from types_aiobotocore_amplifybackend.paginator import ListBackendJobsPaginator
    from types_aiobotocore_amplifybackend.type_defs import ListBackendJobsResponseTypeDef


    session = Session()

    client: AmplifyBackendClient
    async with session.client("amplifybackend") as client:  # (1)
        paginator: ListBackendJobsPaginator = client.get_paginator("list_backend_jobs")  # (2)
        async for item in paginator.paginate(...):
            item: ListBackendJobsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [AmplifyBackendClient](./client.md)
    2. paginator: [ListBackendJobsPaginator](./paginators.md#listbackendjobspaginator)
    3. item: [:material-code-braces: ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef) 




