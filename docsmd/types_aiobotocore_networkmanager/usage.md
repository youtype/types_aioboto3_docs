# Examples

> [Index](../README.md) > [NetworkManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NetworkManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
    type annotations stubs module [types-aiobotocore-networkmanager](https://pypi.org/project/types-aiobotocore-networkmanager/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[networkmanager]` package installed.

Write your `NetworkManager` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("networkmanager") as client:  # (1)
        result = await client.accept_attachment()  # (2)
    ```

    1. client: [NetworkManagerClient](./client.md)
    2. result: [:material-code-braces: AcceptAttachmentResponseTypeDef](./type_defs.md#acceptattachmentresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("networkmanager") as client:  # (1)
        paginator = client.get_paginator("describe_global_networks")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [NetworkManagerClient](./client.md)
    2. paginator: [DescribeGlobalNetworksPaginator](./paginators.md#describeglobalnetworkspaginator)
    3. item: [:material-code-braces: DescribeGlobalNetworksResponseTypeDef](./type_defs.md#describeglobalnetworksresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[networkmanager]`
or a standalone `types_aiobotocore_networkmanager` package, you have to explicitly specify
`client: NetworkManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_networkmanager.client import NetworkManagerClient
    from types_aiobotocore_networkmanager.type_defs import AcceptAttachmentResponseTypeDef
    from types_aiobotocore_networkmanager.type_defs import AcceptAttachmentRequestRequestTypeDef


    session = Session()

    client: NetworkManagerClient
    async with session.client("networkmanager") as client:  # (1)
        kwargs: AcceptAttachmentRequestRequestTypeDef = {...}  # (2)
        result: AcceptAttachmentResponseTypeDef = await client.accept_attachment(**kwargs)  # (3)
    ```

    1. client: [NetworkManagerClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptAttachmentRequestRequestTypeDef](./type_defs.md#acceptattachmentrequestrequesttypedef) 
    3. result: [:material-code-braces: AcceptAttachmentResponseTypeDef](./type_defs.md#acceptattachmentresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_networkmanager.client import NetworkManagerClient
    from types_aiobotocore_networkmanager.paginator import DescribeGlobalNetworksPaginator
    from types_aiobotocore_networkmanager.type_defs import DescribeGlobalNetworksResponseTypeDef


    session = Session()

    client: NetworkManagerClient
    async with session.client("networkmanager") as client:  # (1)
        paginator: DescribeGlobalNetworksPaginator = client.get_paginator("describe_global_networks")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeGlobalNetworksResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [NetworkManagerClient](./client.md)
    2. paginator: [DescribeGlobalNetworksPaginator](./paginators.md#describeglobalnetworkspaginator)
    3. item: [:material-code-braces: DescribeGlobalNetworksResponseTypeDef](./type_defs.md#describeglobalnetworksresponsetypedef) 




