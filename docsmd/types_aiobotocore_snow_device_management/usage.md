# Examples

> [Index](../README.md) > [SnowDeviceManagement](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SnowDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#snowdevicemanagement)
    type annotations stubs module [types-aiobotocore-snow-device-management](https://pypi.org/project/types-aiobotocore-snow-device-management/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[snow-device-management]` package installed.

Write your `SnowDeviceManagement` code as usual,
type checking and code completion should work out of the box.



```python
# SnowDeviceManagementClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("snow-device-management") as client:  # (1)
    result = await client.cancel_task()  # (2)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. result: [:material-code-braces: CancelTaskOutputTypeDef](./type_defs.md#canceltaskoutputtypedef) 



```python
# ListDeviceResourcesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("snow-device-management") as client:  # (1)
    paginator = client.get_paginator("list_device_resources")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. paginator: [ListDeviceResourcesPaginator](./paginators.md#listdeviceresourcespaginator)
3. item: [:material-code-braces: ListDeviceResourcesOutputTypeDef](./type_defs.md#listdeviceresourcesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[snow-device-management]`
or a standalone `types_aiobotocore_snow_device_management` package, you have to explicitly specify
`client: SnowDeviceManagementClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SnowDeviceManagementClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_snow_device_management.client import SnowDeviceManagementClient
from types_aiobotocore_snow_device_management.type_defs import CancelTaskOutputTypeDef
from types_aiobotocore_snow_device_management.type_defs import CancelTaskInputRequestTypeDef


session = Session()

client: SnowDeviceManagementClient
async with session.client("snow-device-management") as client:  # (1)
    kwargs: CancelTaskInputRequestTypeDef = {...}  # (2)
    result: CancelTaskOutputTypeDef = await client.cancel_task(**kwargs)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. kwargs: [:material-code-braces: CancelTaskInputRequestTypeDef](./type_defs.md#canceltaskinputrequesttypedef) 
3. result: [:material-code-braces: CancelTaskOutputTypeDef](./type_defs.md#canceltaskoutputtypedef) 



```python
# ListDeviceResourcesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_snow_device_management.client import SnowDeviceManagementClient
from types_aiobotocore_snow_device_management.paginator import ListDeviceResourcesPaginator
from types_aiobotocore_snow_device_management.type_defs import ListDeviceResourcesOutputTypeDef


session = Session()

client: SnowDeviceManagementClient
async with session.client("snow-device-management") as client:  # (1)
    paginator: ListDeviceResourcesPaginator = client.get_paginator("list_device_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [SnowDeviceManagementClient](./client.md)
2. paginator: [ListDeviceResourcesPaginator](./paginators.md#listdeviceresourcespaginator)
3. item: [:material-code-braces: ListDeviceResourcesOutputTypeDef](./type_defs.md#listdeviceresourcesoutputtypedef) 



