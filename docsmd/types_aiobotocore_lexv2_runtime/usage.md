# Examples

> [Index](../README.md) > [LexRuntimeV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LexRuntimeV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
    type annotations stubs module [types-aiobotocore-lexv2-runtime](https://pypi.org/project/types-aiobotocore-lexv2-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lexv2-runtime]` package installed.

Write your `LexRuntimeV2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lexv2-runtime") as client:  # (1)
        result = await client.delete_session()  # (2)
    ```

    1. client: [LexRuntimeV2Client](./client.md)
    2. result: [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[lexv2-runtime]`
or a standalone `types_aiobotocore_lexv2_runtime` package, you have to explicitly specify
`client: LexRuntimeV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client
    from types_aiobotocore_lexv2_runtime.type_defs import DeleteSessionResponseTypeDef
    from types_aiobotocore_lexv2_runtime.type_defs import DeleteSessionRequestRequestTypeDef


    session = Session()

    client: LexRuntimeV2Client
    async with session.client("lexv2-runtime") as client:  # (1)
        kwargs: DeleteSessionRequestRequestTypeDef = {...}  # (2)
        result: DeleteSessionResponseTypeDef = await client.delete_session(**kwargs)  # (3)
    ```

    1. client: [LexRuntimeV2Client](./client.md)
    2. kwargs: [:material-code-braces: DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef) 
    3. result: [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef) 






