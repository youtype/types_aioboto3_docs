# Examples

> [Index](../README.md) > [AppStream](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appstream]` package installed.

Write your `AppStream` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appstream") as client:  # (1)
        result = await client.associate_application_fleet()  # (2)
    ```

    1. client: [AppStreamClient](./client.md)
    2. result: [:material-code-braces: AssociateApplicationFleetResultTypeDef](./type_defs.md#associateapplicationfleetresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appstream") as client:  # (1)
        paginator = client.get_paginator("describe_directory_configs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AppStreamClient](./client.md)
    2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
    3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appstream") as client:  # (1)
        waiter = client.get_waiter("fleet_started")  # (2)
        await waiter.wait()
    ```

    1. client: [AppStreamClient](./client.md)
    2. waiter: [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[appstream]`
or a standalone `types_aiobotocore_appstream` package, you have to explicitly specify
`client: AppStreamClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appstream.client import AppStreamClient
    from types_aiobotocore_appstream.type_defs import AssociateApplicationFleetResultTypeDef
    from types_aiobotocore_appstream.type_defs import AssociateApplicationFleetRequestRequestTypeDef


    session = Session()

    client: AppStreamClient
    async with session.client("appstream") as client:  # (1)
        kwargs: AssociateApplicationFleetRequestRequestTypeDef = {...}  # (2)
        result: AssociateApplicationFleetResultTypeDef = await client.associate_application_fleet(**kwargs)  # (3)
    ```

    1. client: [AppStreamClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateApplicationFleetRequestRequestTypeDef](./type_defs.md#associateapplicationfleetrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateApplicationFleetResultTypeDef](./type_defs.md#associateapplicationfleetresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appstream.client import AppStreamClient
    from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator
    from types_aiobotocore_appstream.type_defs import DescribeDirectoryConfigsResultTypeDef


    session = Session()

    client: AppStreamClient
    async with session.client("appstream") as client:  # (1)
        paginator: DescribeDirectoryConfigsPaginator = client.get_paginator("describe_directory_configs")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeDirectoryConfigsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [AppStreamClient](./client.md)
    2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
    3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appstream.client import AppStreamClient
    from types_aiobotocore_appstream.waiter import FleetStartedWaiter


    session = Session()

    async with session.client("appstream") as client:  # (1)
        waiter = client.get_waiter("fleet_started")  # (2)
        await waiter.wait()
    ```

    1. client: [AppStreamClient](./client.md)
    2. waiter: [FleetStartedWaiter](./waiters.md#fleetstartedwaiter)


