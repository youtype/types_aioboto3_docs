# Examples

> [Index](../README.md) > [MigrationHubConfig](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[migrationhub-config]` package installed.

Write your `MigrationHubConfig` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("migrationhub-config") as client:  # (1)
        result = await client.create_home_region_control()  # (2)
    ```

    1. client: [MigrationHubConfigClient](./client.md)
    2. result: [:material-code-braces: CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef) 






### Explicit type annotations

With `types-aioboto3-lite[migrationhub-config]`
or a standalone `types_aiobotocore_migrationhub_config` package, you have to explicitly specify
`client: MigrationHubConfigClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient
    from types_aiobotocore_migrationhub_config.type_defs import CreateHomeRegionControlResultTypeDef
    from types_aiobotocore_migrationhub_config.type_defs import CreateHomeRegionControlRequestRequestTypeDef


    session = Session()

    client: MigrationHubConfigClient
    async with session.client("migrationhub-config") as client:  # (1)
        kwargs: CreateHomeRegionControlRequestRequestTypeDef = {...}  # (2)
        result: CreateHomeRegionControlResultTypeDef = await client.create_home_region_control(**kwargs)  # (3)
    ```

    1. client: [MigrationHubConfigClient](./client.md)
    2. kwargs: [:material-code-braces: CreateHomeRegionControlRequestRequestTypeDef](./type_defs.md#createhomeregioncontrolrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef) 





