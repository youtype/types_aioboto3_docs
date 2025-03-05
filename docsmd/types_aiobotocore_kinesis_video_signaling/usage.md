# Examples

> [Index](../README.md) > [KinesisVideoSignalingChannels](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#kinesisvideosignalingchannels)
    type annotations stubs module [types-aiobotocore-kinesis-video-signaling](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kinesis-video-signaling]` package installed.

Write your `KinesisVideoSignalingChannels` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# KinesisVideoSignalingChannelsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("kinesis-video-signaling") as client:  # (1)
    result = await client.get_ice_server_config()  # (2)
```

1. client: [KinesisVideoSignalingChannelsClient](./client.md)
2. result: [:material-code-braces: GetIceServerConfigResponseTypeDef](./type_defs.md#geticeserverconfigresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[kinesis-video-signaling]`
or a standalone `types_aiobotocore_kinesis_video_signaling` package, you have to explicitly specify
`client: KinesisVideoSignalingChannelsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# KinesisVideoSignalingChannelsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient
from types_aiobotocore_kinesis_video_signaling.type_defs import GetIceServerConfigResponseTypeDef
from types_aiobotocore_kinesis_video_signaling.type_defs import GetIceServerConfigRequestTypeDef


session = Session()

client: KinesisVideoSignalingChannelsClient
async with session.client("kinesis-video-signaling") as client:  # (1)
    kwargs: GetIceServerConfigRequestTypeDef = {...}  # (2)
    result: GetIceServerConfigResponseTypeDef = await client.get_ice_server_config(**kwargs)  # (3)
```

1. client: [KinesisVideoSignalingChannelsClient](./client.md)
2. kwargs: [:material-code-braces: GetIceServerConfigRequestTypeDef](./type_defs.md#geticeserverconfigrequesttypedef)
3. result: [:material-code-braces: GetIceServerConfigResponseTypeDef](./type_defs.md#geticeserverconfigresponsetypedef)






