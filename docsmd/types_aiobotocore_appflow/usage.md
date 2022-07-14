# Examples

> [Index](../README.md) > [Appflow](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Appflow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
    type annotations stubs module [types-aiobotocore-appflow](https://pypi.org/project/types-aiobotocore-appflow/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appflow]` package installed.

Write your `Appflow` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appflow") as client:  # (1)
        result = await client.create_connector_profile()  # (2)
    ```

    1. client: [AppflowClient](./client.md)
    2. result: [:material-code-braces: CreateConnectorProfileResponseTypeDef](./type_defs.md#createconnectorprofileresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[appflow]`
or a standalone `types_aiobotocore_appflow` package, you have to explicitly specify
`client: AppflowClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appflow.client import AppflowClient
    from types_aiobotocore_appflow.type_defs import CreateConnectorProfileResponseTypeDef
    from types_aiobotocore_appflow.type_defs import CreateConnectorProfileRequestRequestTypeDef


    session = Session()

    client: AppflowClient
    async with session.client("appflow") as client:  # (1)
        kwargs: CreateConnectorProfileRequestRequestTypeDef = {...}  # (2)
        result: CreateConnectorProfileResponseTypeDef = await client.create_connector_profile(**kwargs)  # (3)
    ```

    1. client: [AppflowClient](./client.md)
    2. kwargs: [:material-code-braces: CreateConnectorProfileRequestRequestTypeDef](./type_defs.md#createconnectorprofilerequestrequesttypedef) 
    3. result: [:material-code-braces: CreateConnectorProfileResponseTypeDef](./type_defs.md#createconnectorprofileresponsetypedef) 






