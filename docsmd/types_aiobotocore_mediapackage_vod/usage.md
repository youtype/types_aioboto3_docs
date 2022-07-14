# Examples

> [Index](../README.md) > [MediaPackageVod](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
    type annotations stubs module [types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mediapackage-vod]` package installed.

Write your `MediaPackageVod` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediapackage-vod") as client:  # (1)
        result = await client.configure_logs()  # (2)
    ```

    1. client: [MediaPackageVodClient](./client.md)
    2. result: [:material-code-braces: ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediapackage-vod") as client:  # (1)
        paginator = client.get_paginator("list_assets")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MediaPackageVodClient](./client.md)
    2. paginator: [ListAssetsPaginator](./paginators.md#listassetspaginator)
    3. item: [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mediapackage-vod]`
or a standalone `types_aiobotocore_mediapackage_vod` package, you have to explicitly specify
`client: MediaPackageVodClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient
    from types_aiobotocore_mediapackage_vod.type_defs import ConfigureLogsResponseTypeDef
    from types_aiobotocore_mediapackage_vod.type_defs import ConfigureLogsRequestRequestTypeDef


    session = Session()

    client: MediaPackageVodClient
    async with session.client("mediapackage-vod") as client:  # (1)
        kwargs: ConfigureLogsRequestRequestTypeDef = {...}  # (2)
        result: ConfigureLogsResponseTypeDef = await client.configure_logs(**kwargs)  # (3)
    ```

    1. client: [MediaPackageVodClient](./client.md)
    2. kwargs: [:material-code-braces: ConfigureLogsRequestRequestTypeDef](./type_defs.md#configurelogsrequestrequesttypedef) 
    3. result: [:material-code-braces: ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient
    from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator
    from types_aiobotocore_mediapackage_vod.type_defs import ListAssetsResponseTypeDef


    session = Session()

    client: MediaPackageVodClient
    async with session.client("mediapackage-vod") as client:  # (1)
        paginator: ListAssetsPaginator = client.get_paginator("list_assets")  # (2)
        async for item in paginator.paginate(...):
            item: ListAssetsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MediaPackageVodClient](./client.md)
    2. paginator: [ListAssetsPaginator](./paginators.md#listassetspaginator)
    3. item: [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 




