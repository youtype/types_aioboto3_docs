# Examples

> [Index](../README.md) > [Lightsail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
    type annotations stubs module [types-aiobotocore-lightsail](https://pypi.org/project/types-aiobotocore-lightsail/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lightsail]` package installed.

Write your `Lightsail` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lightsail") as client:  # (1)
        result = await client.allocate_static_ip()  # (2)
    ```

    1. client: [LightsailClient](./client.md)
    2. result: [:material-code-braces: AllocateStaticIpResultTypeDef](./type_defs.md#allocatestaticipresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lightsail") as client:  # (1)
        paginator = client.get_paginator("get_active_names")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [LightsailClient](./client.md)
    2. paginator: [GetActiveNamesPaginator](./paginators.md#getactivenamespaginator)
    3. item: [:material-code-braces: GetActiveNamesResultTypeDef](./type_defs.md#getactivenamesresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[lightsail]`
or a standalone `types_aiobotocore_lightsail` package, you have to explicitly specify
`client: LightsailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lightsail.client import LightsailClient
    from types_aiobotocore_lightsail.type_defs import AllocateStaticIpResultTypeDef
    from types_aiobotocore_lightsail.type_defs import AllocateStaticIpRequestRequestTypeDef


    session = Session()

    client: LightsailClient
    async with session.client("lightsail") as client:  # (1)
        kwargs: AllocateStaticIpRequestRequestTypeDef = {...}  # (2)
        result: AllocateStaticIpResultTypeDef = await client.allocate_static_ip(**kwargs)  # (3)
    ```

    1. client: [LightsailClient](./client.md)
    2. kwargs: [:material-code-braces: AllocateStaticIpRequestRequestTypeDef](./type_defs.md#allocatestaticiprequestrequesttypedef) 
    3. result: [:material-code-braces: AllocateStaticIpResultTypeDef](./type_defs.md#allocatestaticipresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lightsail.client import LightsailClient
    from types_aiobotocore_lightsail.paginator import GetActiveNamesPaginator
    from types_aiobotocore_lightsail.type_defs import GetActiveNamesResultTypeDef


    session = Session()

    client: LightsailClient
    async with session.client("lightsail") as client:  # (1)
        paginator: GetActiveNamesPaginator = client.get_paginator("get_active_names")  # (2)
        async for item in paginator.paginate(...):
            item: GetActiveNamesResultTypeDef
            print(item)  # (3)
    ```

    1. client: [LightsailClient](./client.md)
    2. paginator: [GetActiveNamesPaginator](./paginators.md#getactivenamespaginator)
    3. item: [:material-code-braces: GetActiveNamesResultTypeDef](./type_defs.md#getactivenamesresulttypedef) 




