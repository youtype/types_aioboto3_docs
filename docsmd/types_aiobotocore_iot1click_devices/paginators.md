# Paginators

> [Index](../README.md) > [IoT1ClickDevicesService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoT1ClickDevicesService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#iot1clickdevicesservice)
    type annotations stubs module [types-aiobotocore-iot1click-devices](https://pypi.org/project/types-aiobotocore-iot1click-devices/).

## ListDeviceEventsPaginator

Type annotations and code completion for `#!python session.client("iot1click-devices").get_paginator("list_device_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices/paginator/ListDeviceEvents.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents)

```python
# ListDeviceEventsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_iot1click_devices.paginator import ListDeviceEventsPaginator

session = Session()

session = get_session()
async with session.client("iot1click-devices") as client:  # (1)
    paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoT1ClickDevicesServiceClient](./client.md)
2. paginator: [ListDeviceEventsPaginator](./paginators.md#listdeviceeventspaginator)
3. item: [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DeviceId: str,
    FromTimeStamp: TimestampTypeDef,
    ToTimeStamp: TimestampTypeDef,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeviceEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeviceEventsRequestPaginateTypeDef = {  # (1)
    "DeviceId": ...,
    "FromTimeStamp": ...,
    "ToTimeStamp": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceEventsRequestPaginateTypeDef](./type_defs.md#listdeviceeventsrequestpaginatetypedef) 
## ListDevicesPaginator

Type annotations and code completion for `#!python session.client("iot1click-devices").get_paginator("list_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices/paginator/ListDevices.html#IoT1ClickDevicesService.Paginator.ListDevices)

```python
# ListDevicesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_iot1click_devices.paginator import ListDevicesPaginator

session = Session()

session = get_session()
async with session.client("iot1click-devices") as client:  # (1)
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoT1ClickDevicesServiceClient](./client.md)
2. paginator: [ListDevicesPaginator](./paginators.md#listdevicespaginator)
3. item: [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DeviceType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicesRequestPaginateTypeDef = {  # (1)
    "DeviceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestPaginateTypeDef](./type_defs.md#listdevicesrequestpaginatetypedef) 