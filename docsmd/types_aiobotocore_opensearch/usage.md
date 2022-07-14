# Examples

> [Index](../README.md) > [OpenSearchService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[opensearch]` package installed.

Write your `OpenSearchService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("opensearch") as client:  # (1)
        result = await client.accept_inbound_connection()  # (2)
    ```

    1. client: [OpenSearchServiceClient](./client.md)
    2. result: [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[opensearch]`
or a standalone `types_aiobotocore_opensearch` package, you have to explicitly specify
`client: OpenSearchServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_opensearch.client import OpenSearchServiceClient
    from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionResponseTypeDef
    from types_aiobotocore_opensearch.type_defs import AcceptInboundConnectionRequestRequestTypeDef


    session = Session()

    client: OpenSearchServiceClient
    async with session.client("opensearch") as client:  # (1)
        kwargs: AcceptInboundConnectionRequestRequestTypeDef = {...}  # (2)
        result: AcceptInboundConnectionResponseTypeDef = await client.accept_inbound_connection(**kwargs)  # (3)
    ```

    1. client: [OpenSearchServiceClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptInboundConnectionRequestRequestTypeDef](./type_defs.md#acceptinboundconnectionrequestrequesttypedef) 
    3. result: [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef) 






