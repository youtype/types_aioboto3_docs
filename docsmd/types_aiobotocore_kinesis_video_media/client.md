# KinesisVideoMediaClient

> [Index](../README.md) > [KinesisVideoMedia](./README.md) > KinesisVideoMediaClient

!!! note ""

    Auto-generated documentation for [KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#kinesisvideomedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

## KinesisVideoMediaClient

Type annotations and code completion for `#!python session.client("kinesis-video-media")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# KinesisVideoMediaClient usage example

from aioboto3.session import Session
from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient

session = Session()
async with session.client("kinesis-video-media") as client:
    client: KinesisVideoMediaClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("kinesis-video-media").exceptions` structure.

```python
# KinesisVideoMediaClient.exceptions usage example

async with session.client("kinesis-video-media") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ClientLimitExceededException,
        client.exceptions.ConnectionLimitExceededException,
        client.exceptions.InvalidArgumentException,
        client.exceptions.InvalidEndpointException,
        client.exceptions.NotAuthorizedException,
        client.exceptions.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# KinesisVideoMediaClient.exceptions type checking example

from types_aiobotocore_kinesis_video_media.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("kinesis-video-media").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("kinesis-video-media").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

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


### get\_media

Use this API to retrieve media content from a Kinesis video stream.

Type annotations and code completion for `#!python session.client("kinesis-video-media").get_media` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# get_media method definition

await def get_media(
    self,
    *,
    StartSelector: StartSelectorTypeDef,  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> GetMediaOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartSelectorTypeDef](./type_defs.md#startselectortypedef) 
2. See [:material-code-braces: GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef) 


```python
# get_media method usage example with argument unpacking

kwargs: GetMediaInputRequestTypeDef = {  # (1)
    "StartSelector": ...,
}

parent.get_media(**kwargs)
```

1. See [:material-code-braces: GetMediaInputRequestTypeDef](./type_defs.md#getmediainputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("kinesis-video-media").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("kinesis-video-media").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

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




