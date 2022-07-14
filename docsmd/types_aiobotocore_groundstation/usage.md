# Examples

> [Index](../README.md) > [GroundStation](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[groundstation]` package installed.

Write your `GroundStation` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("groundstation") as client:  # (1)
        result = await client.cancel_contact()  # (2)
    ```

    1. client: [GroundStationClient](./client.md)
    2. result: [:material-code-braces: ContactIdResponseTypeDef](./type_defs.md#contactidresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("groundstation") as client:  # (1)
        paginator = client.get_paginator("list_configs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GroundStationClient](./client.md)
    2. paginator: [ListConfigsPaginator](./paginators.md#listconfigspaginator)
    3. item: [:material-code-braces: ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[groundstation]`
or a standalone `types_aiobotocore_groundstation` package, you have to explicitly specify
`client: GroundStationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_groundstation.client import GroundStationClient
    from types_aiobotocore_groundstation.type_defs import ContactIdResponseTypeDef
    from types_aiobotocore_groundstation.type_defs import CancelContactRequestRequestTypeDef


    session = Session()

    client: GroundStationClient
    async with session.client("groundstation") as client:  # (1)
        kwargs: CancelContactRequestRequestTypeDef = {...}  # (2)
        result: ContactIdResponseTypeDef = await client.cancel_contact(**kwargs)  # (3)
    ```

    1. client: [GroundStationClient](./client.md)
    2. kwargs: [:material-code-braces: CancelContactRequestRequestTypeDef](./type_defs.md#cancelcontactrequestrequesttypedef) 
    3. result: [:material-code-braces: ContactIdResponseTypeDef](./type_defs.md#contactidresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_groundstation.client import GroundStationClient
    from types_aiobotocore_groundstation.paginator import ListConfigsPaginator
    from types_aiobotocore_groundstation.type_defs import ListConfigsResponseTypeDef


    session = Session()

    client: GroundStationClient
    async with session.client("groundstation") as client:  # (1)
        paginator: ListConfigsPaginator = client.get_paginator("list_configs")  # (2)
        async for item in paginator.paginate(...):
            item: ListConfigsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [GroundStationClient](./client.md)
    2. paginator: [ListConfigsPaginator](./paginators.md#listconfigspaginator)
    3. item: [:material-code-braces: ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef) 




