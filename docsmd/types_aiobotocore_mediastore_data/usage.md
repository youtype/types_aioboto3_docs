# Examples

> [Index](../README.md) > [MediaStoreData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
    type annotations stubs module [types-aiobotocore-mediastore-data](https://pypi.org/project/types-aiobotocore-mediastore-data/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mediastore-data]` package installed.

Write your `MediaStoreData` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediastore-data") as client:  # (1)
        result = await client.describe_object()  # (2)
    ```

    1. client: [MediaStoreDataClient](./client.md)
    2. result: [:material-code-braces: DescribeObjectResponseTypeDef](./type_defs.md#describeobjectresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediastore-data") as client:  # (1)
        paginator = client.get_paginator("list_items")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MediaStoreDataClient](./client.md)
    2. paginator: [ListItemsPaginator](./paginators.md#listitemspaginator)
    3. item: [:material-code-braces: ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mediastore-data]`
or a standalone `types_aiobotocore_mediastore_data` package, you have to explicitly specify
`client: MediaStoreDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediastore_data.client import MediaStoreDataClient
    from types_aiobotocore_mediastore_data.type_defs import DescribeObjectResponseTypeDef
    from types_aiobotocore_mediastore_data.type_defs import DescribeObjectRequestRequestTypeDef


    session = Session()

    client: MediaStoreDataClient
    async with session.client("mediastore-data") as client:  # (1)
        kwargs: DescribeObjectRequestRequestTypeDef = {...}  # (2)
        result: DescribeObjectResponseTypeDef = await client.describe_object(**kwargs)  # (3)
    ```

    1. client: [MediaStoreDataClient](./client.md)
    2. kwargs: [:material-code-braces: DescribeObjectRequestRequestTypeDef](./type_defs.md#describeobjectrequestrequesttypedef) 
    3. result: [:material-code-braces: DescribeObjectResponseTypeDef](./type_defs.md#describeobjectresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediastore_data.client import MediaStoreDataClient
    from types_aiobotocore_mediastore_data.paginator import ListItemsPaginator
    from types_aiobotocore_mediastore_data.type_defs import ListItemsResponseTypeDef


    session = Session()

    client: MediaStoreDataClient
    async with session.client("mediastore-data") as client:  # (1)
        paginator: ListItemsPaginator = client.get_paginator("list_items")  # (2)
        async for item in paginator.paginate(...):
            item: ListItemsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MediaStoreDataClient](./client.md)
    2. paginator: [ListItemsPaginator](./paginators.md#listitemspaginator)
    3. item: [:material-code-braces: ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef) 




