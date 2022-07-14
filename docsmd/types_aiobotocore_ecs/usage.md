# Examples

> [Index](../README.md) > [ECS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ecs]` package installed.

Write your `ECS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ecs") as client:  # (1)
        result = await client.create_capacity_provider()  # (2)
    ```

    1. client: [ECSClient](./client.md)
    2. result: [:material-code-braces: CreateCapacityProviderResponseTypeDef](./type_defs.md#createcapacityproviderresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ecs") as client:  # (1)
        paginator = client.get_paginator("list_account_settings")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ECSClient](./client.md)
    2. paginator: [ListAccountSettingsPaginator](./paginators.md#listaccountsettingspaginator)
    3. item: [:material-code-braces: ListAccountSettingsResponseTypeDef](./type_defs.md#listaccountsettingsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ecs") as client:  # (1)
        waiter = client.get_waiter("services_inactive")  # (2)
        await waiter.wait()
    ```

    1. client: [ECSClient](./client.md)
    2. waiter: [ServicesInactiveWaiter](./waiters.md#servicesinactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[ecs]`
or a standalone `types_aiobotocore_ecs` package, you have to explicitly specify
`client: ECSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ecs.client import ECSClient
    from types_aiobotocore_ecs.type_defs import CreateCapacityProviderResponseTypeDef
    from types_aiobotocore_ecs.type_defs import CreateCapacityProviderRequestRequestTypeDef


    session = Session()

    client: ECSClient
    async with session.client("ecs") as client:  # (1)
        kwargs: CreateCapacityProviderRequestRequestTypeDef = {...}  # (2)
        result: CreateCapacityProviderResponseTypeDef = await client.create_capacity_provider(**kwargs)  # (3)
    ```

    1. client: [ECSClient](./client.md)
    2. kwargs: [:material-code-braces: CreateCapacityProviderRequestRequestTypeDef](./type_defs.md#createcapacityproviderrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateCapacityProviderResponseTypeDef](./type_defs.md#createcapacityproviderresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ecs.client import ECSClient
    from types_aiobotocore_ecs.paginator import ListAccountSettingsPaginator
    from types_aiobotocore_ecs.type_defs import ListAccountSettingsResponseTypeDef


    session = Session()

    client: ECSClient
    async with session.client("ecs") as client:  # (1)
        paginator: ListAccountSettingsPaginator = client.get_paginator("list_account_settings")  # (2)
        async for item in paginator.paginate(...):
            item: ListAccountSettingsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [ECSClient](./client.md)
    2. paginator: [ListAccountSettingsPaginator](./paginators.md#listaccountsettingspaginator)
    3. item: [:material-code-braces: ListAccountSettingsResponseTypeDef](./type_defs.md#listaccountsettingsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ecs.client import ECSClient
    from types_aiobotocore_ecs.waiter import ServicesInactiveWaiter


    session = Session()

    async with session.client("ecs") as client:  # (1)
        waiter = client.get_waiter("services_inactive")  # (2)
        await waiter.wait()
    ```

    1. client: [ECSClient](./client.md)
    2. waiter: [ServicesInactiveWaiter](./waiters.md#servicesinactivewaiter)


