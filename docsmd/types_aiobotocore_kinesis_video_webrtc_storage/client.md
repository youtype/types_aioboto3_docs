# KinesisVideoWebRTCStorageClient

> [Index](../README.md) > [KinesisVideoWebRTCStorage](./README.md) > KinesisVideoWebRTCStorageClient

!!! note ""

    Auto-generated documentation for [KinesisVideoWebRTCStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#kinesisvideowebrtcstorage)
    type annotations stubs module [types-aiobotocore-kinesis-video-webrtc-storage](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage/).

## KinesisVideoWebRTCStorageClient

Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# KinesisVideoWebRTCStorageClient usage example

from aioboto3.session import Session
from types_aiobotocore_kinesis_video_webrtc_storage.client import KinesisVideoWebRTCStorageClient

session = Session()
async with session.client("kinesis-video-webrtc-storage") as client:
    client: KinesisVideoWebRTCStorageClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("kinesis-video-webrtc-storage").exceptions` structure.

```python
# KinesisVideoWebRTCStorageClient.exceptions usage example

async with session.client("kinesis-video-webrtc-storage") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ClientLimitExceededException,
        client.exceptions.InvalidArgumentException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# KinesisVideoWebRTCStorageClient.exceptions type checking example

from types_aiobotocore_kinesis_video_webrtc_storage.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### join\_storage\_session

Before using this API, you must call the
<code>GetSignalingChannelEndpoint</code> API to request the WEBRTC endpoint.

Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage").join_storage_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# join_storage_session method definition

await def join_storage_session(
    self,
    *,
    channelArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# join_storage_session method usage example with argument unpacking

kwargs: JoinStorageSessionInputRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.join_storage_session(**kwargs)
```

1. See [:material-code-braces: JoinStorageSessionInputRequestTypeDef](./type_defs.md#joinstoragesessioninputrequesttypedef) 

### join\_storage\_session\_as\_viewer

Join the ongoing one way-video and/or multi-way audio WebRTC session as a
viewer for an input channel.

Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage").join_storage_session_as_viewer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# join_storage_session_as_viewer method definition

await def join_storage_session_as_viewer(
    self,
    *,
    channelArn: str,
    clientId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# join_storage_session_as_viewer method usage example with argument unpacking

kwargs: JoinStorageSessionAsViewerInputRequestTypeDef = {  # (1)
    "channelArn": ...,
    "clientId": ...,
}

parent.join_storage_session_as_viewer(**kwargs)
```

1. See [:material-code-braces: JoinStorageSessionAsViewerInputRequestTypeDef](./type_defs.md#joinstoragesessionasviewerinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("kinesis-video-webrtc-storage").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




