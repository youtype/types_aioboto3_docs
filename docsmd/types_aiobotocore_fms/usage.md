# Examples

> [Index](../README.md) > [FMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[fms]` package installed.

Write your `FMS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("fms") as client:  # (1)
        result = await client.associate_admin_account()  # (2)
    ```

    1. client: [FMSClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("fms") as client:  # (1)
        paginator = client.get_paginator("list_apps_lists")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [FMSClient](./client.md)
    2. paginator: [ListAppsListsPaginator](./paginators.md#listappslistspaginator)
    3. item: [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[fms]`
or a standalone `types_aiobotocore_fms` package, you have to explicitly specify
`client: FMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_fms.client import FMSClient
    from types_aiobotocore_fms.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_fms.type_defs import AssociateAdminAccountRequestRequestTypeDef


    session = Session()

    client: FMSClient
    async with session.client("fms") as client:  # (1)
        kwargs: AssociateAdminAccountRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.associate_admin_account(**kwargs)  # (3)
    ```

    1. client: [FMSClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateAdminAccountRequestRequestTypeDef](./type_defs.md#associateadminaccountrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_fms.client import FMSClient
    from types_aiobotocore_fms.paginator import ListAppsListsPaginator
    from types_aiobotocore_fms.type_defs import ListAppsListsResponseTypeDef


    session = Session()

    client: FMSClient
    async with session.client("fms") as client:  # (1)
        paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")  # (2)
        async for item in paginator.paginate(...):
            item: ListAppsListsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [FMSClient](./client.md)
    2. paginator: [ListAppsListsPaginator](./paginators.md#listappslistspaginator)
    3. item: [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 




