# Examples

> [Index](../README.md) > [AppConfigData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
    type annotations stubs module [types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appconfigdata]` package installed.

Write your `AppConfigData` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appconfigdata") as client:  # (1)
        result = await client.get_latest_configuration()  # (2)
    ```

    1. client: [AppConfigDataClient](./client.md)
    2. result: [:material-code-braces: GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[appconfigdata]`
or a standalone `types_aiobotocore_appconfigdata` package, you have to explicitly specify
`client: AppConfigDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appconfigdata.client import AppConfigDataClient
    from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationResponseTypeDef
    from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef


    session = Session()

    client: AppConfigDataClient
    async with session.client("appconfigdata") as client:  # (1)
        kwargs: GetLatestConfigurationRequestRequestTypeDef = {...}  # (2)
        result: GetLatestConfigurationResponseTypeDef = await client.get_latest_configuration(**kwargs)  # (3)
    ```

    1. client: [AppConfigDataClient](./client.md)
    2. kwargs: [:material-code-braces: GetLatestConfigurationRequestRequestTypeDef](./type_defs.md#getlatestconfigurationrequestrequesttypedef) 
    3. result: [:material-code-braces: GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef) 






