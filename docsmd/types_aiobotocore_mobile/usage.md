# Examples

> [Index](../README.md) > [Mobile](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Mobile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
    type annotations stubs module [types-aiobotocore-mobile](https://pypi.org/project/types-aiobotocore-mobile/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mobile]` package installed.

Write your `Mobile` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mobile") as client:  # (1)
        result = await client.create_project()  # (2)
    ```

    1. client: [MobileClient](./client.md)
    2. result: [:material-code-braces: CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mobile") as client:  # (1)
        paginator = client.get_paginator("list_bundles")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MobileClient](./client.md)
    2. paginator: [ListBundlesPaginator](./paginators.md#listbundlespaginator)
    3. item: [:material-code-braces: ListBundlesResultTypeDef](./type_defs.md#listbundlesresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mobile]`
or a standalone `types_aiobotocore_mobile` package, you have to explicitly specify
`client: MobileClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mobile.client import MobileClient
    from types_aiobotocore_mobile.type_defs import CreateProjectResultTypeDef
    from types_aiobotocore_mobile.type_defs import CreateProjectRequestRequestTypeDef


    session = Session()

    client: MobileClient
    async with session.client("mobile") as client:  # (1)
        kwargs: CreateProjectRequestRequestTypeDef = {...}  # (2)
        result: CreateProjectResultTypeDef = await client.create_project(**kwargs)  # (3)
    ```

    1. client: [MobileClient](./client.md)
    2. kwargs: [:material-code-braces: CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mobile.client import MobileClient
    from types_aiobotocore_mobile.paginator import ListBundlesPaginator
    from types_aiobotocore_mobile.type_defs import ListBundlesResultTypeDef


    session = Session()

    client: MobileClient
    async with session.client("mobile") as client:  # (1)
        paginator: ListBundlesPaginator = client.get_paginator("list_bundles")  # (2)
        async for item in paginator.paginate(...):
            item: ListBundlesResultTypeDef
            print(item)  # (3)
    ```

    1. client: [MobileClient](./client.md)
    2. paginator: [ListBundlesPaginator](./paginators.md#listbundlespaginator)
    3. item: [:material-code-braces: ListBundlesResultTypeDef](./type_defs.md#listbundlesresulttypedef) 




