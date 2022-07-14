# Examples

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rum]` package installed.

Write your `CloudWatchRUM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rum") as client:  # (1)
        result = await client.create_app_monitor()  # (2)
    ```

    1. client: [CloudWatchRUMClient](./client.md)
    2. result: [:material-code-braces: CreateAppMonitorResponseTypeDef](./type_defs.md#createappmonitorresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rum") as client:  # (1)
        paginator = client.get_paginator("get_app_monitor_data")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudWatchRUMClient](./client.md)
    2. paginator: [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
    3. item: [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[rum]`
or a standalone `types_aiobotocore_rum` package, you have to explicitly specify
`client: CloudWatchRUMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rum.client import CloudWatchRUMClient
    from types_aiobotocore_rum.type_defs import CreateAppMonitorResponseTypeDef
    from types_aiobotocore_rum.type_defs import CreateAppMonitorRequestRequestTypeDef


    session = Session()

    client: CloudWatchRUMClient
    async with session.client("rum") as client:  # (1)
        kwargs: CreateAppMonitorRequestRequestTypeDef = {...}  # (2)
        result: CreateAppMonitorResponseTypeDef = await client.create_app_monitor(**kwargs)  # (3)
    ```

    1. client: [CloudWatchRUMClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAppMonitorRequestRequestTypeDef](./type_defs.md#createappmonitorrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateAppMonitorResponseTypeDef](./type_defs.md#createappmonitorresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rum.client import CloudWatchRUMClient
    from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator
    from types_aiobotocore_rum.type_defs import GetAppMonitorDataResponseTypeDef


    session = Session()

    client: CloudWatchRUMClient
    async with session.client("rum") as client:  # (1)
        paginator: GetAppMonitorDataPaginator = client.get_paginator("get_app_monitor_data")  # (2)
        async for item in paginator.paginate(...):
            item: GetAppMonitorDataResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudWatchRUMClient](./client.md)
    2. paginator: [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
    3. item: [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 




