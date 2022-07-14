# Examples

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
    type annotations stubs module [types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[globalaccelerator]` package installed.

Write your `GlobalAccelerator` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("globalaccelerator") as client:  # (1)
        result = await client.add_custom_routing_endpoints()  # (2)
    ```

    1. client: [GlobalAcceleratorClient](./client.md)
    2. result: [:material-code-braces: AddCustomRoutingEndpointsResponseTypeDef](./type_defs.md#addcustomroutingendpointsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("globalaccelerator") as client:  # (1)
        paginator = client.get_paginator("list_accelerators")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GlobalAcceleratorClient](./client.md)
    2. paginator: [ListAcceleratorsPaginator](./paginators.md#listacceleratorspaginator)
    3. item: [:material-code-braces: ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[globalaccelerator]`
or a standalone `types_aiobotocore_globalaccelerator` package, you have to explicitly specify
`client: GlobalAcceleratorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_globalaccelerator.client import GlobalAcceleratorClient
    from types_aiobotocore_globalaccelerator.type_defs import AddCustomRoutingEndpointsResponseTypeDef
    from types_aiobotocore_globalaccelerator.type_defs import AddCustomRoutingEndpointsRequestRequestTypeDef


    session = Session()

    client: GlobalAcceleratorClient
    async with session.client("globalaccelerator") as client:  # (1)
        kwargs: AddCustomRoutingEndpointsRequestRequestTypeDef = {...}  # (2)
        result: AddCustomRoutingEndpointsResponseTypeDef = await client.add_custom_routing_endpoints(**kwargs)  # (3)
    ```

    1. client: [GlobalAcceleratorClient](./client.md)
    2. kwargs: [:material-code-braces: AddCustomRoutingEndpointsRequestRequestTypeDef](./type_defs.md#addcustomroutingendpointsrequestrequesttypedef) 
    3. result: [:material-code-braces: AddCustomRoutingEndpointsResponseTypeDef](./type_defs.md#addcustomroutingendpointsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_globalaccelerator.client import GlobalAcceleratorClient
    from types_aiobotocore_globalaccelerator.paginator import ListAcceleratorsPaginator
    from types_aiobotocore_globalaccelerator.type_defs import ListAcceleratorsResponseTypeDef


    session = Session()

    client: GlobalAcceleratorClient
    async with session.client("globalaccelerator") as client:  # (1)
        paginator: ListAcceleratorsPaginator = client.get_paginator("list_accelerators")  # (2)
        async for item in paginator.paginate(...):
            item: ListAcceleratorsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [GlobalAcceleratorClient](./client.md)
    2. paginator: [ListAcceleratorsPaginator](./paginators.md#listacceleratorspaginator)
    3. item: [:material-code-braces: ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef) 




