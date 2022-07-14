# Examples

> [Index](../README.md) > [AppSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[appsync]` package installed.

Write your `AppSync` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appsync") as client:  # (1)
        result = await client.associate_api()  # (2)
    ```

    1. client: [AppSyncClient](./client.md)
    2. result: [:material-code-braces: AssociateApiResponseTypeDef](./type_defs.md#associateapiresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("appsync") as client:  # (1)
        paginator = client.get_paginator("list_api_keys")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AppSyncClient](./client.md)
    2. paginator: [ListApiKeysPaginator](./paginators.md#listapikeyspaginator)
    3. item: [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[appsync]`
or a standalone `types_aiobotocore_appsync` package, you have to explicitly specify
`client: AppSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appsync.client import AppSyncClient
    from types_aiobotocore_appsync.type_defs import AssociateApiResponseTypeDef
    from types_aiobotocore_appsync.type_defs import AssociateApiRequestRequestTypeDef


    session = Session()

    client: AppSyncClient
    async with session.client("appsync") as client:  # (1)
        kwargs: AssociateApiRequestRequestTypeDef = {...}  # (2)
        result: AssociateApiResponseTypeDef = await client.associate_api(**kwargs)  # (3)
    ```

    1. client: [AppSyncClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateApiRequestRequestTypeDef](./type_defs.md#associateapirequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateApiResponseTypeDef](./type_defs.md#associateapiresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_appsync.client import AppSyncClient
    from types_aiobotocore_appsync.paginator import ListApiKeysPaginator
    from types_aiobotocore_appsync.type_defs import ListApiKeysResponseTypeDef


    session = Session()

    client: AppSyncClient
    async with session.client("appsync") as client:  # (1)
        paginator: ListApiKeysPaginator = client.get_paginator("list_api_keys")  # (2)
        async for item in paginator.paginate(...):
            item: ListApiKeysResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [AppSyncClient](./client.md)
    2. paginator: [ListApiKeysPaginator](./paginators.md#listapikeyspaginator)
    3. item: [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 




