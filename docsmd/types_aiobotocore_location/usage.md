# Examples

> [Index](../README.md) > [LocationService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[location]` package installed.

Write your `LocationService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("location") as client:  # (1)
        result = await client.batch_delete_device_position_history()  # (2)
    ```

    1. client: [LocationServiceClient](./client.md)
    2. result: [:material-code-braces: BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("location") as client:  # (1)
        paginator = client.get_paginator("get_device_position_history")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [LocationServiceClient](./client.md)
    2. paginator: [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
    3. item: [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[location]`
or a standalone `types_aiobotocore_location` package, you have to explicitly specify
`client: LocationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_location.client import LocationServiceClient
    from types_aiobotocore_location.type_defs import BatchDeleteDevicePositionHistoryResponseTypeDef
    from types_aiobotocore_location.type_defs import BatchDeleteDevicePositionHistoryRequestRequestTypeDef


    session = Session()

    client: LocationServiceClient
    async with session.client("location") as client:  # (1)
        kwargs: BatchDeleteDevicePositionHistoryRequestRequestTypeDef = {...}  # (2)
        result: BatchDeleteDevicePositionHistoryResponseTypeDef = await client.batch_delete_device_position_history(**kwargs)  # (3)
    ```

    1. client: [LocationServiceClient](./client.md)
    2. kwargs: [:material-code-braces: BatchDeleteDevicePositionHistoryRequestRequestTypeDef](./type_defs.md#batchdeletedevicepositionhistoryrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_location.client import LocationServiceClient
    from types_aiobotocore_location.paginator import GetDevicePositionHistoryPaginator
    from types_aiobotocore_location.type_defs import GetDevicePositionHistoryResponseTypeDef


    session = Session()

    client: LocationServiceClient
    async with session.client("location") as client:  # (1)
        paginator: GetDevicePositionHistoryPaginator = client.get_paginator("get_device_position_history")  # (2)
        async for item in paginator.paginate(...):
            item: GetDevicePositionHistoryResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [LocationServiceClient](./client.md)
    2. paginator: [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
    3. item: [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 




