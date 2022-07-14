# Examples

> [Index](../README.md) > [Detective](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
    type annotations stubs module [types-aiobotocore-detective](https://pypi.org/project/types-aiobotocore-detective/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[detective]` package installed.

Write your `Detective` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("detective") as client:  # (1)
        result = await client.accept_invitation()  # (2)
    ```

    1. client: [DetectiveClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aioboto3-lite[detective]`
or a standalone `types_aiobotocore_detective` package, you have to explicitly specify
`client: DetectiveClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_detective.client import DetectiveClient
    from types_aiobotocore_detective.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_detective.type_defs import AcceptInvitationRequestRequestTypeDef


    session = Session()

    client: DetectiveClient
    async with session.client("detective") as client:  # (1)
        kwargs: AcceptInvitationRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.accept_invitation(**kwargs)  # (3)
    ```

    1. client: [DetectiveClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






