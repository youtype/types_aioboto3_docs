# Examples

> [Index](../README.md) > [KinesisVideoWebRTCStorage](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideoWebRTCStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#kinesisvideowebrtcstorage)
    type annotations stubs module [types-aiobotocore-kinesis-video-webrtc-storage](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kinesis-video-webrtc-storage]` package installed.

Write your `KinesisVideoWebRTCStorage` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisVideoWebRTCStorageClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("kinesis-video-webrtc-storage") as client:  # (1)
    result = await client.join_storage_session()  # (2)
```

1. client: [KinesisVideoWebRTCStorageClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aioboto3-lite[kinesis-video-webrtc-storage]`
or a standalone `types_aiobotocore_kinesis_video_webrtc_storage` package, you have to explicitly specify
`client: KinesisVideoWebRTCStorageClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisVideoWebRTCStorageClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_kinesis_video_webrtc_storage.client import KinesisVideoWebRTCStorageClient
from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import JoinStorageSessionInputRequestTypeDef


session = Session()

client: KinesisVideoWebRTCStorageClient
async with session.client("kinesis-video-webrtc-storage") as client:  # (1)
    kwargs: JoinStorageSessionInputRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.join_storage_session(**kwargs)  # (3)
```

1. client: [KinesisVideoWebRTCStorageClient](./client.md)
2. kwargs: [:material-code-braces: JoinStorageSessionInputRequestTypeDef](./type_defs.md#joinstoragesessioninputrequesttypedef) 
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 





