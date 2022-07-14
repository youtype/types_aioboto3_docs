# Examples

> [Index](../README.md) > [DirectConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DirectConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
    type annotations stubs module [types-aiobotocore-directconnect](https://pypi.org/project/types-aiobotocore-directconnect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[directconnect]` package installed.

Write your `DirectConnect` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("directconnect") as client:  # (1)
        result = await client.accept_direct_connect_gateway_association_proposal()  # (2)
    ```

    1. client: [DirectConnectClient](./client.md)
    2. result: [:material-code-braces: AcceptDirectConnectGatewayAssociationProposalResultTypeDef](./type_defs.md#acceptdirectconnectgatewayassociationproposalresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("directconnect") as client:  # (1)
        paginator = client.get_paginator("describe_direct_connect_gateway_associations")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [DirectConnectClient](./client.md)
    2. paginator: [DescribeDirectConnectGatewayAssociationsPaginator](./paginators.md#describedirectconnectgatewayassociationspaginator)
    3. item: [:material-code-braces: DescribeDirectConnectGatewayAssociationsResultTypeDef](./type_defs.md#describedirectconnectgatewayassociationsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[directconnect]`
or a standalone `types_aiobotocore_directconnect` package, you have to explicitly specify
`client: DirectConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_directconnect.client import DirectConnectClient
    from types_aiobotocore_directconnect.type_defs import AcceptDirectConnectGatewayAssociationProposalResultTypeDef
    from types_aiobotocore_directconnect.type_defs import AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef


    session = Session()

    client: DirectConnectClient
    async with session.client("directconnect") as client:  # (1)
        kwargs: AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef = {...}  # (2)
        result: AcceptDirectConnectGatewayAssociationProposalResultTypeDef = await client.accept_direct_connect_gateway_association_proposal(**kwargs)  # (3)
    ```

    1. client: [DirectConnectClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef](./type_defs.md#acceptdirectconnectgatewayassociationproposalrequestrequesttypedef) 
    3. result: [:material-code-braces: AcceptDirectConnectGatewayAssociationProposalResultTypeDef](./type_defs.md#acceptdirectconnectgatewayassociationproposalresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_directconnect.client import DirectConnectClient
    from types_aiobotocore_directconnect.paginator import DescribeDirectConnectGatewayAssociationsPaginator
    from types_aiobotocore_directconnect.type_defs import DescribeDirectConnectGatewayAssociationsResultTypeDef


    session = Session()

    client: DirectConnectClient
    async with session.client("directconnect") as client:  # (1)
        paginator: DescribeDirectConnectGatewayAssociationsPaginator = client.get_paginator("describe_direct_connect_gateway_associations")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeDirectConnectGatewayAssociationsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [DirectConnectClient](./client.md)
    2. paginator: [DescribeDirectConnectGatewayAssociationsPaginator](./paginators.md#describedirectconnectgatewayassociationspaginator)
    3. item: [:material-code-braces: DescribeDirectConnectGatewayAssociationsResultTypeDef](./type_defs.md#describedirectconnectgatewayassociationsresulttypedef) 




