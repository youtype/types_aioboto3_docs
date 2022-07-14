# Examples

> [Index](../README.md) > [ApiGatewayManagementApi](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[apigatewaymanagementapi]` package installed.

Write your `ApiGatewayManagementApi` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("apigatewaymanagementapi") as client:  # (1)
        result = await client.delete_connection()  # (2)
    ```

    1. client: [ApiGatewayManagementApiClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aioboto3-lite[apigatewaymanagementapi]`
or a standalone `types_aiobotocore_apigatewaymanagementapi` package, you have to explicitly specify
`client: ApiGatewayManagementApiClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
    from types_aiobotocore_apigatewaymanagementapi.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef


    session = Session()

    client: ApiGatewayManagementApiClient
    async with session.client("apigatewaymanagementapi") as client:  # (1)
        kwargs: DeleteConnectionRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.delete_connection(**kwargs)  # (3)
    ```

    1. client: [ApiGatewayManagementApiClient](./client.md)
    2. kwargs: [:material-code-braces: DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






