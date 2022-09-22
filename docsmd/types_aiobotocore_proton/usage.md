# Examples

> [Index](../README.md) > [Proton](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
    type annotations stubs module [types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[proton]` package installed.

Write your `Proton` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("proton") as client:  # (1)
        result = await client.accept_environment_account_connection()  # (2)
    ```

    1. client: [ProtonClient](./client.md)
    2. result: [:material-code-braces: AcceptEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#acceptenvironmentaccountconnectionoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("proton") as client:  # (1)
        paginator = client.get_paginator("list_component_outputs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ProtonClient](./client.md)
    2. paginator: [ListComponentOutputsPaginator](./paginators.md#listcomponentoutputspaginator)
    3. item: [:material-code-braces: ListComponentOutputsOutputTypeDef](./type_defs.md#listcomponentoutputsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("proton") as client:  # (1)
        waiter = client.get_waiter("component_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [ProtonClient](./client.md)
    2. waiter: [ComponentDeletedWaiter](./waiters.md#componentdeletedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[proton]`
or a standalone `types_aiobotocore_proton` package, you have to explicitly specify
`client: ProtonClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.type_defs import AcceptEnvironmentAccountConnectionOutputTypeDef
    from types_aiobotocore_proton.type_defs import AcceptEnvironmentAccountConnectionInputRequestTypeDef


    session = Session()

    client: ProtonClient
    async with session.client("proton") as client:  # (1)
        kwargs: AcceptEnvironmentAccountConnectionInputRequestTypeDef = {...}  # (2)
        result: AcceptEnvironmentAccountConnectionOutputTypeDef = await client.accept_environment_account_connection(**kwargs)  # (3)
    ```

    1. client: [ProtonClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptEnvironmentAccountConnectionInputRequestTypeDef](./type_defs.md#acceptenvironmentaccountconnectioninputrequesttypedef) 
    3. result: [:material-code-braces: AcceptEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#acceptenvironmentaccountconnectionoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.paginator import ListComponentOutputsPaginator
    from types_aiobotocore_proton.type_defs import ListComponentOutputsOutputTypeDef


    session = Session()

    client: ProtonClient
    async with session.client("proton") as client:  # (1)
        paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")  # (2)
        async for item in paginator.paginate(...):
            item: ListComponentOutputsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [ProtonClient](./client.md)
    2. paginator: [ListComponentOutputsPaginator](./paginators.md#listcomponentoutputspaginator)
    3. item: [:material-code-braces: ListComponentOutputsOutputTypeDef](./type_defs.md#listcomponentoutputsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.waiter import ComponentDeletedWaiter


    session = Session()

    async with session.client("proton") as client:  # (1)
        waiter = client.get_waiter("component_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [ProtonClient](./client.md)
    2. waiter: [ComponentDeletedWaiter](./waiters.md#componentdeletedwaiter)


