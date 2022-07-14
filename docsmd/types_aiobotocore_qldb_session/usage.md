# Examples

> [Index](../README.md) > [QLDBSession](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[qldb-session]` package installed.

Write your `QLDBSession` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("qldb-session") as client:  # (1)
        result = await client.send_command()  # (2)
    ```

    1. client: [QLDBSessionClient](./client.md)
    2. result: [:material-code-braces: SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef) 






### Explicit type annotations

With `types-aioboto3-lite[qldb-session]`
or a standalone `types_aiobotocore_qldb_session` package, you have to explicitly specify
`client: QLDBSessionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_qldb_session.client import QLDBSessionClient
    from types_aiobotocore_qldb_session.type_defs import SendCommandResultTypeDef
    from types_aiobotocore_qldb_session.type_defs import SendCommandRequestRequestTypeDef


    session = Session()

    client: QLDBSessionClient
    async with session.client("qldb-session") as client:  # (1)
        kwargs: SendCommandRequestRequestTypeDef = {...}  # (2)
        result: SendCommandResultTypeDef = await client.send_command(**kwargs)  # (3)
    ```

    1. client: [QLDBSessionClient](./client.md)
    2. kwargs: [:material-code-braces: SendCommandRequestRequestTypeDef](./type_defs.md#sendcommandrequestrequesttypedef) 
    3. result: [:material-code-braces: SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef) 






