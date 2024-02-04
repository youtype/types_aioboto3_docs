# Examples

> [Index](../README.md) > [ivsrealtime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ivs-realtime]` package installed.

Write your `ivsrealtime` code as usual,
type checking and code completion should work out of the box.



```python
# ivsrealtimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ivs-realtime") as client:  # (1)
    result = await client.create_encoder_configuration()  # (2)
```

1. client: [ivsrealtimeClient](./client.md)
2. result: [:material-code-braces: CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[ivs-realtime]`
or a standalone `types_aiobotocore_ivs_realtime` package, you have to explicitly specify
`client: ivsrealtimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ivsrealtimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ivs_realtime.client import ivsrealtimeClient
from types_aiobotocore_ivs_realtime.type_defs import CreateEncoderConfigurationResponseTypeDef
from types_aiobotocore_ivs_realtime.type_defs import CreateEncoderConfigurationRequestRequestTypeDef


session = Session()

client: ivsrealtimeClient
async with session.client("ivs-realtime") as client:  # (1)
    kwargs: CreateEncoderConfigurationRequestRequestTypeDef = {...}  # (2)
    result: CreateEncoderConfigurationResponseTypeDef = await client.create_encoder_configuration(**kwargs)  # (3)
```

1. client: [ivsrealtimeClient](./client.md)
2. kwargs: [:material-code-braces: CreateEncoderConfigurationRequestRequestTypeDef](./type_defs.md#createencoderconfigurationrequestrequesttypedef) 
3. result: [:material-code-braces: CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef) 






