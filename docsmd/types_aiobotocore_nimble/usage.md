# Examples

> [Index](../README.md) > [NimbleStudio](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
    type annotations stubs module [types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[nimble]` package installed.

Write your `NimbleStudio` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("nimble") as client:  # (1)
        result = await client.accept_eulas()  # (2)
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. result: [:material-code-braces: AcceptEulasResponseTypeDef](./type_defs.md#accepteulasresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("nimble") as client:  # (1)
        paginator = client.get_paginator("list_eula_acceptances")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. paginator: [ListEulaAcceptancesPaginator](./paginators.md#listeulaacceptancespaginator)
    3. item: [:material-code-braces: ListEulaAcceptancesResponseTypeDef](./type_defs.md#listeulaacceptancesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("nimble") as client:  # (1)
        waiter = client.get_waiter("launch_profile_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. waiter: [LaunchProfileDeletedWaiter](./waiters.md#launchprofiledeletedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[nimble]`
or a standalone `types_aiobotocore_nimble` package, you have to explicitly specify
`client: NimbleStudioClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_nimble.client import NimbleStudioClient
    from types_aiobotocore_nimble.type_defs import AcceptEulasResponseTypeDef
    from types_aiobotocore_nimble.type_defs import AcceptEulasRequestRequestTypeDef


    session = Session()

    client: NimbleStudioClient
    async with session.client("nimble") as client:  # (1)
        kwargs: AcceptEulasRequestRequestTypeDef = {...}  # (2)
        result: AcceptEulasResponseTypeDef = await client.accept_eulas(**kwargs)  # (3)
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptEulasRequestRequestTypeDef](./type_defs.md#accepteulasrequestrequesttypedef) 
    3. result: [:material-code-braces: AcceptEulasResponseTypeDef](./type_defs.md#accepteulasresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_nimble.client import NimbleStudioClient
    from types_aiobotocore_nimble.paginator import ListEulaAcceptancesPaginator
    from types_aiobotocore_nimble.type_defs import ListEulaAcceptancesResponseTypeDef


    session = Session()

    client: NimbleStudioClient
    async with session.client("nimble") as client:  # (1)
        paginator: ListEulaAcceptancesPaginator = client.get_paginator("list_eula_acceptances")  # (2)
        async for item in paginator.paginate(...):
            item: ListEulaAcceptancesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. paginator: [ListEulaAcceptancesPaginator](./paginators.md#listeulaacceptancespaginator)
    3. item: [:material-code-braces: ListEulaAcceptancesResponseTypeDef](./type_defs.md#listeulaacceptancesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_nimble.client import NimbleStudioClient
    from types_aiobotocore_nimble.waiter import LaunchProfileDeletedWaiter


    session = Session()

    async with session.client("nimble") as client:  # (1)
        waiter = client.get_waiter("launch_profile_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. waiter: [LaunchProfileDeletedWaiter](./waiters.md#launchprofiledeletedwaiter)


