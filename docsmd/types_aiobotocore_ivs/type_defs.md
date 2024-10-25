# Type definitions

> [Index](../README.md) > [IVS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
    type annotations stubs module [types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).



## AudioConfigurationTypeDef

```python
# AudioConfigurationTypeDef definition

class AudioConfigurationTypeDef(TypedDict):
    codec: NotRequired[str],
    targetBitrate: NotRequired[int],
    sampleRate: NotRequired[int],
    channels: NotRequired[int],
```

## BatchErrorTypeDef

```python
# BatchErrorTypeDef definition

class BatchErrorTypeDef(TypedDict):
    arn: NotRequired[str],
    code: NotRequired[str],
    message: NotRequired[str],
```

## BatchGetChannelRequestRequestTypeDef

```python
# BatchGetChannelRequestRequestTypeDef definition

class BatchGetChannelRequestRequestTypeDef(TypedDict):
    arns: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BatchGetStreamKeyRequestRequestTypeDef

```python
# BatchGetStreamKeyRequestRequestTypeDef definition

class BatchGetStreamKeyRequestRequestTypeDef(TypedDict):
    arns: Sequence[str],
```

## StreamKeyTypeDef

```python
# StreamKeyTypeDef definition

class StreamKeyTypeDef(TypedDict):
    arn: NotRequired[str],
    value: NotRequired[str],
    channelArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## BatchStartViewerSessionRevocationErrorTypeDef

```python
# BatchStartViewerSessionRevocationErrorTypeDef definition

class BatchStartViewerSessionRevocationErrorTypeDef(TypedDict):
    channelArn: str,
    viewerId: str,
    code: NotRequired[str],
    message: NotRequired[str],
```

## BatchStartViewerSessionRevocationViewerSessionTypeDef

```python
# BatchStartViewerSessionRevocationViewerSessionTypeDef definition

class BatchStartViewerSessionRevocationViewerSessionTypeDef(TypedDict):
    channelArn: str,
    viewerId: str,
    viewerSessionVersionsLessThanOrEqualTo: NotRequired[int],
```

## ChannelSummaryTypeDef

```python
# ChannelSummaryTypeDef definition

class ChannelSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (1)
    authorized: NotRequired[bool],
    recordingConfigurationArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    insecureIngest: NotRequired[bool],
    type: NotRequired[ChannelTypeType],  # (2)
    preset: NotRequired[TranscodePresetType],  # (3)
    playbackRestrictionPolicyArn: NotRequired[str],
```

1. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
2. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
3. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
## SrtTypeDef

```python
# SrtTypeDef definition

class SrtTypeDef(TypedDict):
    endpoint: NotRequired[str],
    passphrase: NotRequired[str],
```

## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (1)
    type: NotRequired[ChannelTypeType],  # (2)
    authorized: NotRequired[bool],
    recordingConfigurationArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    insecureIngest: NotRequired[bool],
    preset: NotRequired[TranscodePresetType],  # (3)
    playbackRestrictionPolicyArn: NotRequired[str],
```

1. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
2. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
3. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
## CreatePlaybackRestrictionPolicyRequestRequestTypeDef

```python
# CreatePlaybackRestrictionPolicyRequestRequestTypeDef definition

class CreatePlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    allowedCountries: NotRequired[Sequence[str]],
    allowedOrigins: NotRequired[Sequence[str]],
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## PlaybackRestrictionPolicyTypeDef

```python
# PlaybackRestrictionPolicyTypeDef definition

class PlaybackRestrictionPolicyTypeDef(TypedDict):
    arn: str,
    allowedCountries: List[str],
    allowedOrigins: List[str],
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## RenditionConfigurationTypeDef

```python
# RenditionConfigurationTypeDef definition

class RenditionConfigurationTypeDef(TypedDict):
    renditionSelection: NotRequired[RenditionConfigurationRenditionSelectionType],  # (1)
    renditions: NotRequired[Sequence[RenditionConfigurationRenditionType]],  # (2)
```

1. See [:material-code-brackets: RenditionConfigurationRenditionSelectionType](./literals.md#renditionconfigurationrenditionselectiontype) 
2. See [:material-code-brackets: RenditionConfigurationRenditionType](./literals.md#renditionconfigurationrenditiontype) 
## ThumbnailConfigurationTypeDef

```python
# ThumbnailConfigurationTypeDef definition

class ThumbnailConfigurationTypeDef(TypedDict):
    recordingMode: NotRequired[RecordingModeType],  # (1)
    targetIntervalSeconds: NotRequired[int],
    resolution: NotRequired[ThumbnailConfigurationResolutionType],  # (2)
    storage: NotRequired[Sequence[ThumbnailConfigurationStorageType]],  # (3)
```

1. See [:material-code-brackets: RecordingModeType](./literals.md#recordingmodetype) 
2. See [:material-code-brackets: ThumbnailConfigurationResolutionType](./literals.md#thumbnailconfigurationresolutiontype) 
3. See [:material-code-brackets: ThumbnailConfigurationStorageType](./literals.md#thumbnailconfigurationstoragetype) 
## CreateStreamKeyRequestRequestTypeDef

```python
# CreateStreamKeyRequestRequestTypeDef definition

class CreateStreamKeyRequestRequestTypeDef(TypedDict):
    channelArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeletePlaybackKeyPairRequestRequestTypeDef

```python
# DeletePlaybackKeyPairRequestRequestTypeDef definition

class DeletePlaybackKeyPairRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeletePlaybackRestrictionPolicyRequestRequestTypeDef

```python
# DeletePlaybackRestrictionPolicyRequestRequestTypeDef definition

class DeletePlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteRecordingConfigurationRequestRequestTypeDef

```python
# DeleteRecordingConfigurationRequestRequestTypeDef definition

class DeleteRecordingConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStreamKeyRequestRequestTypeDef

```python
# DeleteStreamKeyRequestRequestTypeDef definition

class DeleteStreamKeyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## GetChannelRequestRequestTypeDef

```python
# GetChannelRequestRequestTypeDef definition

class GetChannelRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetPlaybackKeyPairRequestRequestTypeDef

```python
# GetPlaybackKeyPairRequestRequestTypeDef definition

class GetPlaybackKeyPairRequestRequestTypeDef(TypedDict):
    arn: str,
```

## PlaybackKeyPairTypeDef

```python
# PlaybackKeyPairTypeDef definition

class PlaybackKeyPairTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    fingerprint: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## GetPlaybackRestrictionPolicyRequestRequestTypeDef

```python
# GetPlaybackRestrictionPolicyRequestRequestTypeDef definition

class GetPlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetRecordingConfigurationRequestRequestTypeDef

```python
# GetRecordingConfigurationRequestRequestTypeDef definition

class GetRecordingConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetStreamKeyRequestRequestTypeDef

```python
# GetStreamKeyRequestRequestTypeDef definition

class GetStreamKeyRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetStreamRequestRequestTypeDef

```python
# GetStreamRequestRequestTypeDef definition

class GetStreamRequestRequestTypeDef(TypedDict):
    channelArn: str,
```

## StreamTypeDef

```python
# StreamTypeDef definition

class StreamTypeDef(TypedDict):
    channelArn: NotRequired[str],
    streamId: NotRequired[str],
    playbackUrl: NotRequired[str],
    startTime: NotRequired[datetime],
    state: NotRequired[StreamStateType],  # (1)
    health: NotRequired[StreamHealthType],  # (2)
    viewerCount: NotRequired[int],
```

1. See [:material-code-brackets: StreamStateType](./literals.md#streamstatetype) 
2. See [:material-code-brackets: StreamHealthType](./literals.md#streamhealthtype) 
## GetStreamSessionRequestRequestTypeDef

```python
# GetStreamSessionRequestRequestTypeDef definition

class GetStreamSessionRequestRequestTypeDef(TypedDict):
    channelArn: str,
    streamId: NotRequired[str],
```

## ImportPlaybackKeyPairRequestRequestTypeDef

```python
# ImportPlaybackKeyPairRequestRequestTypeDef definition

class ImportPlaybackKeyPairRequestRequestTypeDef(TypedDict):
    publicKeyMaterial: str,
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## VideoConfigurationTypeDef

```python
# VideoConfigurationTypeDef definition

class VideoConfigurationTypeDef(TypedDict):
    avcProfile: NotRequired[str],
    avcLevel: NotRequired[str],
    codec: NotRequired[str],
    encoder: NotRequired[str],
    targetBitrate: NotRequired[int],
    targetFramerate: NotRequired[int],
    videoHeight: NotRequired[int],
    videoWidth: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    filterByName: NotRequired[str],
    filterByRecordingConfigurationArn: NotRequired[str],
    filterByPlaybackRestrictionPolicyArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPlaybackKeyPairsRequestRequestTypeDef

```python
# ListPlaybackKeyPairsRequestRequestTypeDef definition

class ListPlaybackKeyPairsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PlaybackKeyPairSummaryTypeDef

```python
# PlaybackKeyPairSummaryTypeDef definition

class PlaybackKeyPairSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListPlaybackRestrictionPoliciesRequestRequestTypeDef

```python
# ListPlaybackRestrictionPoliciesRequestRequestTypeDef definition

class ListPlaybackRestrictionPoliciesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PlaybackRestrictionPolicySummaryTypeDef

```python
# PlaybackRestrictionPolicySummaryTypeDef definition

class PlaybackRestrictionPolicySummaryTypeDef(TypedDict):
    arn: str,
    allowedCountries: List[str],
    allowedOrigins: List[str],
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListRecordingConfigurationsRequestRequestTypeDef

```python
# ListRecordingConfigurationsRequestRequestTypeDef definition

class ListRecordingConfigurationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListStreamKeysRequestRequestTypeDef

```python
# ListStreamKeysRequestRequestTypeDef definition

class ListStreamKeysRequestRequestTypeDef(TypedDict):
    channelArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StreamKeySummaryTypeDef

```python
# StreamKeySummaryTypeDef definition

class StreamKeySummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    channelArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStreamSessionsRequestRequestTypeDef

```python
# ListStreamSessionsRequestRequestTypeDef definition

class ListStreamSessionsRequestRequestTypeDef(TypedDict):
    channelArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StreamSessionSummaryTypeDef

```python
# StreamSessionSummaryTypeDef definition

class StreamSessionSummaryTypeDef(TypedDict):
    streamId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    hasErrorEvent: NotRequired[bool],
```

## StreamFiltersTypeDef

```python
# StreamFiltersTypeDef definition

class StreamFiltersTypeDef(TypedDict):
    health: NotRequired[StreamHealthType],  # (1)
```

1. See [:material-code-brackets: StreamHealthType](./literals.md#streamhealthtype) 
## StreamSummaryTypeDef

```python
# StreamSummaryTypeDef definition

class StreamSummaryTypeDef(TypedDict):
    channelArn: NotRequired[str],
    streamId: NotRequired[str],
    state: NotRequired[StreamStateType],  # (1)
    health: NotRequired[StreamHealthType],  # (2)
    viewerCount: NotRequired[int],
    startTime: NotRequired[datetime],
```

1. See [:material-code-brackets: StreamStateType](./literals.md#streamstatetype) 
2. See [:material-code-brackets: StreamHealthType](./literals.md#streamhealthtype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PutMetadataRequestRequestTypeDef

```python
# PutMetadataRequestRequestTypeDef definition

class PutMetadataRequestRequestTypeDef(TypedDict):
    channelArn: str,
    metadata: str,
```

## RenditionConfigurationOutputTypeDef

```python
# RenditionConfigurationOutputTypeDef definition

class RenditionConfigurationOutputTypeDef(TypedDict):
    renditionSelection: NotRequired[RenditionConfigurationRenditionSelectionType],  # (1)
    renditions: NotRequired[List[RenditionConfigurationRenditionType]],  # (2)
```

1. See [:material-code-brackets: RenditionConfigurationRenditionSelectionType](./literals.md#renditionconfigurationrenditionselectiontype) 
2. See [:material-code-brackets: RenditionConfigurationRenditionType](./literals.md#renditionconfigurationrenditiontype) 
## ThumbnailConfigurationOutputTypeDef

```python
# ThumbnailConfigurationOutputTypeDef definition

class ThumbnailConfigurationOutputTypeDef(TypedDict):
    recordingMode: NotRequired[RecordingModeType],  # (1)
    targetIntervalSeconds: NotRequired[int],
    resolution: NotRequired[ThumbnailConfigurationResolutionType],  # (2)
    storage: NotRequired[List[ThumbnailConfigurationStorageType]],  # (3)
```

1. See [:material-code-brackets: RecordingModeType](./literals.md#recordingmodetype) 
2. See [:material-code-brackets: ThumbnailConfigurationResolutionType](./literals.md#thumbnailconfigurationresolutiontype) 
3. See [:material-code-brackets: ThumbnailConfigurationStorageType](./literals.md#thumbnailconfigurationstoragetype) 
## StartViewerSessionRevocationRequestRequestTypeDef

```python
# StartViewerSessionRevocationRequestRequestTypeDef definition

class StartViewerSessionRevocationRequestRequestTypeDef(TypedDict):
    channelArn: str,
    viewerId: str,
    viewerSessionVersionsLessThanOrEqualTo: NotRequired[int],
```

## StopStreamRequestRequestTypeDef

```python
# StopStreamRequestRequestTypeDef definition

class StopStreamRequestRequestTypeDef(TypedDict):
    channelArn: str,
```

## StreamEventTypeDef

```python
# StreamEventTypeDef definition

class StreamEventTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    eventTime: NotRequired[datetime],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (1)
    type: NotRequired[ChannelTypeType],  # (2)
    authorized: NotRequired[bool],
    recordingConfigurationArn: NotRequired[str],
    insecureIngest: NotRequired[bool],
    preset: NotRequired[TranscodePresetType],  # (3)
    playbackRestrictionPolicyArn: NotRequired[str],
```

1. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
2. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
3. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
## UpdatePlaybackRestrictionPolicyRequestRequestTypeDef

```python
# UpdatePlaybackRestrictionPolicyRequestRequestTypeDef definition

class UpdatePlaybackRestrictionPolicyRequestRequestTypeDef(TypedDict):
    arn: str,
    allowedCountries: NotRequired[Sequence[str]],
    allowedOrigins: NotRequired[Sequence[str]],
    enableStrictOriginEnforcement: NotRequired[bool],
    name: NotRequired[str],
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetStreamKeyResponseTypeDef

```python
# BatchGetStreamKeyResponseTypeDef definition

class BatchGetStreamKeyResponseTypeDef(TypedDict):
    streamKeys: List[StreamKeyTypeDef],  # (1)
    errors: List[BatchErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
2. See [:material-code-braces: BatchErrorTypeDef](./type_defs.md#batcherrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamKeyResponseTypeDef

```python
# CreateStreamKeyResponseTypeDef definition

class CreateStreamKeyResponseTypeDef(TypedDict):
    streamKey: StreamKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamKeyResponseTypeDef

```python
# GetStreamKeyResponseTypeDef definition

class GetStreamKeyResponseTypeDef(TypedDict):
    streamKey: StreamKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStartViewerSessionRevocationResponseTypeDef

```python
# BatchStartViewerSessionRevocationResponseTypeDef definition

class BatchStartViewerSessionRevocationResponseTypeDef(TypedDict):
    errors: List[BatchStartViewerSessionRevocationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchStartViewerSessionRevocationErrorTypeDef](./type_defs.md#batchstartviewersessionrevocationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStartViewerSessionRevocationRequestRequestTypeDef

```python
# BatchStartViewerSessionRevocationRequestRequestTypeDef definition

class BatchStartViewerSessionRevocationRequestRequestTypeDef(TypedDict):
    viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],  # (1)
```

1. See [:material-code-braces: BatchStartViewerSessionRevocationViewerSessionTypeDef](./type_defs.md#batchstartviewersessionrevocationviewersessiontypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    channels: List[ChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    latencyMode: NotRequired[ChannelLatencyModeType],  # (1)
    type: NotRequired[ChannelTypeType],  # (2)
    recordingConfigurationArn: NotRequired[str],
    ingestEndpoint: NotRequired[str],
    playbackUrl: NotRequired[str],
    authorized: NotRequired[bool],
    tags: NotRequired[Dict[str, str]],
    insecureIngest: NotRequired[bool],
    preset: NotRequired[TranscodePresetType],  # (3)
    srt: NotRequired[SrtTypeDef],  # (4)
    playbackRestrictionPolicyArn: NotRequired[str],
```

1. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
2. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
3. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
4. See [:material-code-braces: SrtTypeDef](./type_defs.md#srttypedef) 
## CreatePlaybackRestrictionPolicyResponseTypeDef

```python
# CreatePlaybackRestrictionPolicyResponseTypeDef definition

class CreatePlaybackRestrictionPolicyResponseTypeDef(TypedDict):
    playbackRestrictionPolicy: PlaybackRestrictionPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackRestrictionPolicyTypeDef](./type_defs.md#playbackrestrictionpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlaybackRestrictionPolicyResponseTypeDef

```python
# GetPlaybackRestrictionPolicyResponseTypeDef definition

class GetPlaybackRestrictionPolicyResponseTypeDef(TypedDict):
    playbackRestrictionPolicy: PlaybackRestrictionPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackRestrictionPolicyTypeDef](./type_defs.md#playbackrestrictionpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePlaybackRestrictionPolicyResponseTypeDef

```python
# UpdatePlaybackRestrictionPolicyResponseTypeDef definition

class UpdatePlaybackRestrictionPolicyResponseTypeDef(TypedDict):
    playbackRestrictionPolicy: PlaybackRestrictionPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackRestrictionPolicyTypeDef](./type_defs.md#playbackrestrictionpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    s3: NotRequired[S3DestinationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## GetPlaybackKeyPairResponseTypeDef

```python
# GetPlaybackKeyPairResponseTypeDef definition

class GetPlaybackKeyPairResponseTypeDef(TypedDict):
    keyPair: PlaybackKeyPairTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackKeyPairTypeDef](./type_defs.md#playbackkeypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportPlaybackKeyPairResponseTypeDef

```python
# ImportPlaybackKeyPairResponseTypeDef definition

class ImportPlaybackKeyPairResponseTypeDef(TypedDict):
    keyPair: PlaybackKeyPairTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackKeyPairTypeDef](./type_defs.md#playbackkeypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStreamResponseTypeDef

```python
# GetStreamResponseTypeDef definition

class GetStreamResponseTypeDef(TypedDict):
    stream: StreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamTypeDef](./type_defs.md#streamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngestConfigurationTypeDef

```python
# IngestConfigurationTypeDef definition

class IngestConfigurationTypeDef(TypedDict):
    video: NotRequired[VideoConfigurationTypeDef],  # (1)
    audio: NotRequired[AudioConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: VideoConfigurationTypeDef](./type_defs.md#videoconfigurationtypedef) 
2. See [:material-code-braces: AudioConfigurationTypeDef](./type_defs.md#audioconfigurationtypedef) 
## ListChannelsRequestListChannelsPaginateTypeDef

```python
# ListChannelsRequestListChannelsPaginateTypeDef definition

class ListChannelsRequestListChannelsPaginateTypeDef(TypedDict):
    filterByName: NotRequired[str],
    filterByRecordingConfigurationArn: NotRequired[str],
    filterByPlaybackRestrictionPolicyArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef

```python
# ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef definition

class ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef

```python
# ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef definition

class ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamKeysRequestListStreamKeysPaginateTypeDef

```python
# ListStreamKeysRequestListStreamKeysPaginateTypeDef definition

class ListStreamKeysRequestListStreamKeysPaginateTypeDef(TypedDict):
    channelArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaybackKeyPairsResponseTypeDef

```python
# ListPlaybackKeyPairsResponseTypeDef definition

class ListPlaybackKeyPairsResponseTypeDef(TypedDict):
    keyPairs: List[PlaybackKeyPairSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PlaybackKeyPairSummaryTypeDef](./type_defs.md#playbackkeypairsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlaybackRestrictionPoliciesResponseTypeDef

```python
# ListPlaybackRestrictionPoliciesResponseTypeDef definition

class ListPlaybackRestrictionPoliciesResponseTypeDef(TypedDict):
    playbackRestrictionPolicies: List[PlaybackRestrictionPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PlaybackRestrictionPolicySummaryTypeDef](./type_defs.md#playbackrestrictionpolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamKeysResponseTypeDef

```python
# ListStreamKeysResponseTypeDef definition

class ListStreamKeysResponseTypeDef(TypedDict):
    streamKeys: List[StreamKeySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamKeySummaryTypeDef](./type_defs.md#streamkeysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamSessionsResponseTypeDef

```python
# ListStreamSessionsResponseTypeDef definition

class ListStreamSessionsResponseTypeDef(TypedDict):
    streamSessions: List[StreamSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamSessionSummaryTypeDef](./type_defs.md#streamsessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamsRequestListStreamsPaginateTypeDef

```python
# ListStreamsRequestListStreamsPaginateTypeDef definition

class ListStreamsRequestListStreamsPaginateTypeDef(TypedDict):
    filterBy: NotRequired[StreamFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStreamsRequestRequestTypeDef

```python
# ListStreamsRequestRequestTypeDef definition

class ListStreamsRequestRequestTypeDef(TypedDict):
    filterBy: NotRequired[StreamFiltersTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef) 
## ListStreamsResponseTypeDef

```python
# ListStreamsResponseTypeDef definition

class ListStreamsResponseTypeDef(TypedDict):
    streams: List[StreamSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StreamSummaryTypeDef](./type_defs.md#streamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetChannelResponseTypeDef

```python
# BatchGetChannelResponseTypeDef definition

class BatchGetChannelResponseTypeDef(TypedDict):
    channels: List[ChannelTypeDef],  # (1)
    errors: List[BatchErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: BatchErrorTypeDef](./type_defs.md#batcherrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    streamKey: StreamKeyTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: StreamKeyTypeDef](./type_defs.md#streamkeytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelResponseTypeDef

```python
# GetChannelResponseTypeDef definition

class GetChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecordingConfigurationRequestRequestTypeDef

```python
# CreateRecordingConfigurationRequestRequestTypeDef definition

class CreateRecordingConfigurationRequestRequestTypeDef(TypedDict):
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    thumbnailConfiguration: NotRequired[ThumbnailConfigurationTypeDef],  # (2)
    recordingReconnectWindowSeconds: NotRequired[int],
    renditionConfiguration: NotRequired[RenditionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: ThumbnailConfigurationTypeDef](./type_defs.md#thumbnailconfigurationtypedef) 
3. See [:material-code-braces: RenditionConfigurationTypeDef](./type_defs.md#renditionconfigurationtypedef) 
## RecordingConfigurationSummaryTypeDef

```python
# RecordingConfigurationSummaryTypeDef definition

class RecordingConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: RecordingConfigurationStateType,  # (2)
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: RecordingConfigurationStateType](./literals.md#recordingconfigurationstatetype) 
## RecordingConfigurationTypeDef

```python
# RecordingConfigurationTypeDef definition

class RecordingConfigurationTypeDef(TypedDict):
    arn: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: RecordingConfigurationStateType,  # (2)
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    thumbnailConfiguration: NotRequired[ThumbnailConfigurationOutputTypeDef],  # (3)
    recordingReconnectWindowSeconds: NotRequired[int],
    renditionConfiguration: NotRequired[RenditionConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: RecordingConfigurationStateType](./literals.md#recordingconfigurationstatetype) 
3. See [:material-code-braces: ThumbnailConfigurationOutputTypeDef](./type_defs.md#thumbnailconfigurationoutputtypedef) 
4. See [:material-code-braces: RenditionConfigurationOutputTypeDef](./type_defs.md#renditionconfigurationoutputtypedef) 
## ListRecordingConfigurationsResponseTypeDef

```python
# ListRecordingConfigurationsResponseTypeDef definition

class ListRecordingConfigurationsResponseTypeDef(TypedDict):
    recordingConfigurations: List[RecordingConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecordingConfigurationSummaryTypeDef](./type_defs.md#recordingconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecordingConfigurationResponseTypeDef

```python
# CreateRecordingConfigurationResponseTypeDef definition

class CreateRecordingConfigurationResponseTypeDef(TypedDict):
    recordingConfiguration: RecordingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecordingConfigurationResponseTypeDef

```python
# GetRecordingConfigurationResponseTypeDef definition

class GetRecordingConfigurationResponseTypeDef(TypedDict):
    recordingConfiguration: RecordingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamSessionTypeDef

```python
# StreamSessionTypeDef definition

class StreamSessionTypeDef(TypedDict):
    streamId: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    channel: NotRequired[ChannelTypeDef],  # (1)
    ingestConfiguration: NotRequired[IngestConfigurationTypeDef],  # (2)
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (3)
    truncatedEvents: NotRequired[List[StreamEventTypeDef]],  # (4)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef) 
3. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
4. See [:material-code-braces: StreamEventTypeDef](./type_defs.md#streameventtypedef) 
## GetStreamSessionResponseTypeDef

```python
# GetStreamSessionResponseTypeDef definition

class GetStreamSessionResponseTypeDef(TypedDict):
    streamSession: StreamSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamSessionTypeDef](./type_defs.md#streamsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
