# Examples

> [Index](../README.md) > [finspace](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[finspace]` package installed.

Write your `finspace` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("finspace") as client:  # (1)
        result = await client.create_environment()  # (2)
    ```

    1. client: [finspaceClient](./client.md)
    2. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[finspace]`
or a standalone `types_aiobotocore_finspace` package, you have to explicitly specify
`client: finspaceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_finspace.client import finspaceClient
    from types_aiobotocore_finspace.type_defs import CreateEnvironmentResponseTypeDef
    from types_aiobotocore_finspace.type_defs import CreateEnvironmentRequestRequestTypeDef


    session = Session()

    client: finspaceClient
    async with session.client("finspace") as client:  # (1)
        kwargs: CreateEnvironmentRequestRequestTypeDef = {...}  # (2)
        result: CreateEnvironmentResponseTypeDef = await client.create_environment(**kwargs)  # (3)
    ```

    1. client: [finspaceClient](./client.md)
    2. kwargs: [:material-code-braces: CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef) 






