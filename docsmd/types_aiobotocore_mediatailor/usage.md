# Examples

> [Index](../README.md) > [MediaTailor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#mediatailor)
    type annotations stubs module [types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mediatailor]` package installed.

Write your `MediaTailor` code as usual,
type checking and code completion should work out of the box.



```python
# MediaTailorClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("mediatailor") as client:  # (1)
    result = await client.configure_logs_for_channel()  # (2)
```

1. client: [MediaTailorClient](./client.md)
2. result: [:material-code-braces: ConfigureLogsForChannelResponseTypeDef](./type_defs.md#configurelogsforchannelresponsetypedef) 



```python
# GetChannelSchedulePaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("mediatailor") as client:  # (1)
    paginator = client.get_paginator("get_channel_schedule")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MediaTailorClient](./client.md)
2. paginator: [GetChannelSchedulePaginator](./paginators.md#getchannelschedulepaginator)
3. item: [:material-code-braces: GetChannelScheduleResponseTypeDef](./type_defs.md#getchannelscheduleresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mediatailor]`
or a standalone `types_aiobotocore_mediatailor` package, you have to explicitly specify
`client: MediaTailorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MediaTailorClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mediatailor.client import MediaTailorClient
from types_aiobotocore_mediatailor.type_defs import ConfigureLogsForChannelResponseTypeDef
from types_aiobotocore_mediatailor.type_defs import ConfigureLogsForChannelRequestRequestTypeDef


session = Session()

client: MediaTailorClient
async with session.client("mediatailor") as client:  # (1)
    kwargs: ConfigureLogsForChannelRequestRequestTypeDef = {...}  # (2)
    result: ConfigureLogsForChannelResponseTypeDef = await client.configure_logs_for_channel(**kwargs)  # (3)
```

1. client: [MediaTailorClient](./client.md)
2. kwargs: [:material-code-braces: ConfigureLogsForChannelRequestRequestTypeDef](./type_defs.md#configurelogsforchannelrequestrequesttypedef) 
3. result: [:material-code-braces: ConfigureLogsForChannelResponseTypeDef](./type_defs.md#configurelogsforchannelresponsetypedef) 



```python
# GetChannelSchedulePaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_mediatailor.client import MediaTailorClient
from types_aiobotocore_mediatailor.paginator import GetChannelSchedulePaginator
from types_aiobotocore_mediatailor.type_defs import GetChannelScheduleResponseTypeDef


session = Session()

client: MediaTailorClient
async with session.client("mediatailor") as client:  # (1)
    paginator: GetChannelSchedulePaginator = client.get_paginator("get_channel_schedule")  # (2)
    async for item in paginator.paginate(...):
        item: GetChannelScheduleResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaTailorClient](./client.md)
2. paginator: [GetChannelSchedulePaginator](./paginators.md#getchannelschedulepaginator)
3. item: [:material-code-braces: GetChannelScheduleResponseTypeDef](./type_defs.md#getchannelscheduleresponsetypedef) 



