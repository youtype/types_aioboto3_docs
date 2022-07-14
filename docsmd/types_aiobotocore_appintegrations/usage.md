# Examples

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appintegrations]` package installed.

Write your `AppIntegrationsService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appintegrations") as client:  # (1)
        result = await client.create_data_integration()  # (2)
    ```

    1. client: [AppIntegrationsServiceClient](./client.md)
    2. result: [:material-code-braces: CreateDataIntegrationResponseTypeDef](./type_defs.md#createdataintegrationresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[appintegrations]`
or a standalone `types_aiobotocore_appintegrations` package, you have to explicitly specify
`client: AppIntegrationsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
    from types_aiobotocore_appintegrations.type_defs import CreateDataIntegrationResponseTypeDef
    from types_aiobotocore_appintegrations.type_defs import CreateDataIntegrationRequestRequestTypeDef


    session = Session()

    client: AppIntegrationsServiceClient
    async with session.client("appintegrations") as client:  # (1)
        kwargs: CreateDataIntegrationRequestRequestTypeDef = {...}  # (2)
        result: CreateDataIntegrationResponseTypeDef = await client.create_data_integration(**kwargs)  # (3)
    ```

    1. client: [AppIntegrationsServiceClient](./client.md)
    2. kwargs: [:material-code-braces: CreateDataIntegrationRequestRequestTypeDef](./type_defs.md#createdataintegrationrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateDataIntegrationResponseTypeDef](./type_defs.md#createdataintegrationresponsetypedef) 






