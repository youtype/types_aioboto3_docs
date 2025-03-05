# Examples

> [Index](../README.md) > [Ivsrealtime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ivs-realtime]` package installed.

Write your `Ivsrealtime` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IvsrealtimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ivs-realtime") as client:  # (1)
    result = await client.create_encoder_configuration()  # (2)
```

1. client: [IvsrealtimeClient](./client.md)
2. result: [:material-code-braces: CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef)



#### Paginator usage example

```python
# ListIngestConfigurationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ivs-realtime") as client:  # (1)
    paginator = client.get_paginator("list_ingest_configurations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IvsrealtimeClient](./client.md)
2. paginator: [ListIngestConfigurationsPaginator](./paginators.md#listingestconfigurationspaginator)
3. item: [:material-code-braces: ListIngestConfigurationsResponseTypeDef](./type_defs.md#listingestconfigurationsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[ivs-realtime]`
or a standalone `types_aiobotocore_ivs_realtime` package, you have to explicitly specify
`client: IvsrealtimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IvsrealtimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ivs_realtime.client import IvsrealtimeClient
from types_aiobotocore_ivs_realtime.type_defs import CreateEncoderConfigurationResponseTypeDef
from types_aiobotocore_ivs_realtime.type_defs import CreateEncoderConfigurationRequestTypeDef


session = Session()

client: IvsrealtimeClient
async with session.client("ivs-realtime") as client:  # (1)
    kwargs: CreateEncoderConfigurationRequestTypeDef = {...}  # (2)
    result: CreateEncoderConfigurationResponseTypeDef = await client.create_encoder_configuration(**kwargs)  # (3)
```

1. client: [IvsrealtimeClient](./client.md)
2. kwargs: [:material-code-braces: CreateEncoderConfigurationRequestTypeDef](./type_defs.md#createencoderconfigurationrequesttypedef)
3. result: [:material-code-braces: CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef)



#### Paginator usage example

```python
# ListIngestConfigurationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ivs_realtime.client import IvsrealtimeClient
from types_aiobotocore_ivs_realtime.paginator import ListIngestConfigurationsPaginator
from types_aiobotocore_ivs_realtime.type_defs import ListIngestConfigurationsResponseTypeDef


session = Session()

client: IvsrealtimeClient
async with session.client("ivs-realtime") as client:  # (1)
    paginator: ListIngestConfigurationsPaginator = client.get_paginator("list_ingest_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListIngestConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IvsrealtimeClient](./client.md)
2. paginator: [ListIngestConfigurationsPaginator](./paginators.md#listingestconfigurationspaginator)
3. item: [:material-code-braces: ListIngestConfigurationsResponseTypeDef](./type_defs.md#listingestconfigurationsresponsetypedef)




