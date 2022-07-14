# Examples

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[migrationhubstrategy]` package installed.

Write your `MigrationHubStrategyRecommendations` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("migrationhubstrategy") as client:  # (1)
        result = await client.get_application_component_details()  # (2)
    ```

    1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
    2. result: [:material-code-braces: GetApplicationComponentDetailsResponseTypeDef](./type_defs.md#getapplicationcomponentdetailsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("migrationhubstrategy") as client:  # (1)
        paginator = client.get_paginator("get_server_details")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
    2. paginator: [GetServerDetailsPaginator](./paginators.md#getserverdetailspaginator)
    3. item: [:material-code-braces: GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[migrationhubstrategy]`
or a standalone `types_aiobotocore_migrationhubstrategy` package, you have to explicitly specify
`client: MigrationHubStrategyRecommendationsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
    from types_aiobotocore_migrationhubstrategy.type_defs import GetApplicationComponentDetailsResponseTypeDef
    from types_aiobotocore_migrationhubstrategy.type_defs import GetApplicationComponentDetailsRequestRequestTypeDef


    session = Session()

    client: MigrationHubStrategyRecommendationsClient
    async with session.client("migrationhubstrategy") as client:  # (1)
        kwargs: GetApplicationComponentDetailsRequestRequestTypeDef = {...}  # (2)
        result: GetApplicationComponentDetailsResponseTypeDef = await client.get_application_component_details(**kwargs)  # (3)
    ```

    1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
    2. kwargs: [:material-code-braces: GetApplicationComponentDetailsRequestRequestTypeDef](./type_defs.md#getapplicationcomponentdetailsrequestrequesttypedef) 
    3. result: [:material-code-braces: GetApplicationComponentDetailsResponseTypeDef](./type_defs.md#getapplicationcomponentdetailsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
    from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator
    from types_aiobotocore_migrationhubstrategy.type_defs import GetServerDetailsResponseTypeDef


    session = Session()

    client: MigrationHubStrategyRecommendationsClient
    async with session.client("migrationhubstrategy") as client:  # (1)
        paginator: GetServerDetailsPaginator = client.get_paginator("get_server_details")  # (2)
        async for item in paginator.paginate(...):
            item: GetServerDetailsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
    2. paginator: [GetServerDetailsPaginator](./paginators.md#getserverdetailspaginator)
    3. item: [:material-code-braces: GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef) 




