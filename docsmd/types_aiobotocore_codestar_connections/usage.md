# Examples

> [Index](../README.md) > [CodeStarconnections](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeStarconnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
    type annotations stubs module [types-aiobotocore-codestar-connections](https://pypi.org/project/types-aiobotocore-codestar-connections/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codestar-connections]` package installed.

Write your `CodeStarconnections` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codestar-connections") as client:  # (1)
        result = await client.create_connection()  # (2)
    ```

    1. client: [CodeStarconnectionsClient](./client.md)
    2. result: [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef) 






### Explicit type annotations

With `types-aioboto3-lite[codestar-connections]`
or a standalone `types_aiobotocore_codestar_connections` package, you have to explicitly specify
`client: CodeStarconnectionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codestar_connections.client import CodeStarconnectionsClient
    from types_aiobotocore_codestar_connections.type_defs import CreateConnectionOutputTypeDef
    from types_aiobotocore_codestar_connections.type_defs import CreateConnectionInputRequestTypeDef


    session = Session()

    client: CodeStarconnectionsClient
    async with session.client("codestar-connections") as client:  # (1)
        kwargs: CreateConnectionInputRequestTypeDef = {...}  # (2)
        result: CreateConnectionOutputTypeDef = await client.create_connection(**kwargs)  # (3)
    ```

    1. client: [CodeStarconnectionsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateConnectionInputRequestTypeDef](./type_defs.md#createconnectioninputrequesttypedef) 
    3. result: [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef) 






