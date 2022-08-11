# KinesisVideoArchivedMediaClient

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > KinesisVideoArchivedMediaClient

!!! note ""

    Auto-generated documentation for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

## KinesisVideoArchivedMediaClient

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient

session = Session()
async with session.client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("kinesis-video-archived-media").exceptions` structure.

```python title="Usage example"
async with session.client("kinesis-video-archived-media") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ClientLimitExceededException,
        client.InvalidArgumentException,
        client.InvalidCodecPrivateDataException,
        client.InvalidMediaFrameException,
        client.MissingCodecPrivateDataException,
        client.NoDataRetentionException,
        client.NotAuthorizedException,
        client.ResourceNotFoundException,
        client.UnsupportedStreamMediaTypeException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_kinesis_video_archived_media.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_clip

Downloads an MP4 file (clip) containing the archived, on-demand media from the
specified video stream over the specified time range.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").get_clip` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_clip)

```python title="Method definition"
await def get_clip(
    self,
    *,
    ClipFragmentSelector: ClipFragmentSelectorTypeDef,  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> GetClipOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ClipFragmentSelectorTypeDef](./type_defs.md#clipfragmentselectortypedef) 
2. See [:material-code-braces: GetClipOutputTypeDef](./type_defs.md#getclipoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetClipInputRequestTypeDef = {  # (1)
    "ClipFragmentSelector": ...,
}

parent.get_clip(**kwargs)
```

1. See [:material-code-braces: GetClipInputRequestTypeDef](./type_defs.md#getclipinputrequesttypedef) 

### get\_dash\_streaming\_session\_url

Retrieves an MPEG Dynamic Adaptive Streaming over HTTP (DASH) URL for the
stream.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").get_dash_streaming_session_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_dash_streaming_session_url)

```python title="Method definition"
await def get_dash_streaming_session_url(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    PlaybackMode: DASHPlaybackModeType = ...,  # (1)
    DisplayFragmentTimestamp: DASHDisplayFragmentTimestampType = ...,  # (2)
    DisplayFragmentNumber: DASHDisplayFragmentNumberType = ...,  # (3)
    DASHFragmentSelector: DASHFragmentSelectorTypeDef = ...,  # (4)
    Expires: int = ...,
    MaxManifestFragmentResults: int = ...,
) -> GetDASHStreamingSessionURLOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: DASHPlaybackModeType](./literals.md#dashplaybackmodetype) 
2. See [:material-code-brackets: DASHDisplayFragmentTimestampType](./literals.md#dashdisplayfragmenttimestamptype) 
3. See [:material-code-brackets: DASHDisplayFragmentNumberType](./literals.md#dashdisplayfragmentnumbertype) 
4. See [:material-code-braces: DASHFragmentSelectorTypeDef](./type_defs.md#dashfragmentselectortypedef) 
5. See [:material-code-braces: GetDASHStreamingSessionURLOutputTypeDef](./type_defs.md#getdashstreamingsessionurloutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetDASHStreamingSessionURLInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.get_dash_streaming_session_url(**kwargs)
```

1. See [:material-code-braces: GetDASHStreamingSessionURLInputRequestTypeDef](./type_defs.md#getdashstreamingsessionurlinputrequesttypedef) 

### get\_hls\_streaming\_session\_url

Retrieves an HTTP Live Streaming (HLS) URL for the stream.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").get_hls_streaming_session_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_hls_streaming_session_url)

```python title="Method definition"
await def get_hls_streaming_session_url(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    PlaybackMode: HLSPlaybackModeType = ...,  # (1)
    HLSFragmentSelector: HLSFragmentSelectorTypeDef = ...,  # (2)
    ContainerFormat: ContainerFormatType = ...,  # (3)
    DiscontinuityMode: HLSDiscontinuityModeType = ...,  # (4)
    DisplayFragmentTimestamp: HLSDisplayFragmentTimestampType = ...,  # (5)
    Expires: int = ...,
    MaxMediaPlaylistFragmentResults: int = ...,
) -> GetHLSStreamingSessionURLOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: HLSPlaybackModeType](./literals.md#hlsplaybackmodetype) 
2. See [:material-code-braces: HLSFragmentSelectorTypeDef](./type_defs.md#hlsfragmentselectortypedef) 
3. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
4. See [:material-code-brackets: HLSDiscontinuityModeType](./literals.md#hlsdiscontinuitymodetype) 
5. See [:material-code-brackets: HLSDisplayFragmentTimestampType](./literals.md#hlsdisplayfragmenttimestamptype) 
6. See [:material-code-braces: GetHLSStreamingSessionURLOutputTypeDef](./type_defs.md#gethlsstreamingsessionurloutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetHLSStreamingSessionURLInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.get_hls_streaming_session_url(**kwargs)
```

1. See [:material-code-braces: GetHLSStreamingSessionURLInputRequestTypeDef](./type_defs.md#gethlsstreamingsessionurlinputrequesttypedef) 

### get\_media\_for\_fragment\_list

Gets media for a list of fragments (specified by fragment number) from the
archived data in an Amazon Kinesis video stream.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").get_media_for_fragment_list` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_media_for_fragment_list)

```python title="Method definition"
await def get_media_for_fragment_list(
    self,
    *,
    Fragments: Sequence[str],
    StreamName: str = ...,
    StreamARN: str = ...,
) -> GetMediaForFragmentListOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMediaForFragmentListOutputTypeDef](./type_defs.md#getmediaforfragmentlistoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: GetMediaForFragmentListInputRequestTypeDef = {  # (1)
    "Fragments": ...,
}

parent.get_media_for_fragment_list(**kwargs)
```

1. See [:material-code-braces: GetMediaForFragmentListInputRequestTypeDef](./type_defs.md#getmediaforfragmentlistinputrequesttypedef) 

### list\_fragments

Returns a list of  Fragment objects from the specified stream and timestamp
range within the archived data.

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").list_fragments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.list_fragments)

```python title="Method definition"
await def list_fragments(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    FragmentSelector: FragmentSelectorTypeDef = ...,  # (1)
) -> ListFragmentsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef) 
2. See [:material-code-braces: ListFragmentsOutputTypeDef](./type_defs.md#listfragmentsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListFragmentsInputRequestTypeDef = {  # (1)
    "StreamName": ...,
}

parent.list_fragments(**kwargs)
```

1. See [:material-code-braces: ListFragmentsInputRequestTypeDef](./type_defs.md#listfragmentsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> KinesisVideoArchivedMediaClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("kinesis-video-archived-media").get_paginator` method with overloads.

- `client.get_paginator("list_fragments")` -> [ListFragmentsPaginator](./paginators.md#listfragmentspaginator)



