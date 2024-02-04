# Type definitions

> [Index](../README.md) > [ivsrealtime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).



## ChannelDestinationConfigurationTypeDef

```python
# ChannelDestinationConfigurationTypeDef definition

class ChannelDestinationConfigurationTypeDef(TypedDict):
    channelArn: str,
    encoderConfigurationArn: NotRequired[str],
```

## DestinationSummaryTypeDef

```python
# DestinationSummaryTypeDef definition

class DestinationSummaryTypeDef(TypedDict):
    id: str,
    state: DestinationStateType,  # (1)
    endTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## VideoTypeDef

```python
# VideoTypeDef definition

class VideoTypeDef(TypedDict):
    bitrate: NotRequired[int],
    framerate: NotRequired[float],
    height: NotRequired[int],
    width: NotRequired[int],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CreateParticipantTokenRequestRequestTypeDef

```python
# CreateParticipantTokenRequestRequestTypeDef definition

class CreateParticipantTokenRequestRequestTypeDef(TypedDict):
    stageArn: str,
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
    duration: NotRequired[int],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## ParticipantTokenTypeDef

```python
# ParticipantTokenTypeDef definition

class ParticipantTokenTypeDef(TypedDict):
    attributes: NotRequired[Dict[str, str]],
    capabilities: NotRequired[List[ParticipantTokenCapabilityType]],  # (1)
    duration: NotRequired[int],
    expirationTime: NotRequired[datetime],
    participantId: NotRequired[str],
    token: NotRequired[str],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## ParticipantTokenConfigurationTypeDef

```python
# ParticipantTokenConfigurationTypeDef definition

class ParticipantTokenConfigurationTypeDef(TypedDict):
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ParticipantTokenCapabilityType]],  # (1)
    duration: NotRequired[int],
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
## StageTypeDef

```python
# StageTypeDef definition

class StageTypeDef(TypedDict):
    arn: str,
    activeSessionId: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## S3StorageConfigurationTypeDef

```python
# S3StorageConfigurationTypeDef definition

class S3StorageConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## DeleteEncoderConfigurationRequestRequestTypeDef

```python
# DeleteEncoderConfigurationRequestRequestTypeDef definition

class DeleteEncoderConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStageRequestRequestTypeDef

```python
# DeleteStageRequestRequestTypeDef definition

class DeleteStageRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteStorageConfigurationRequestRequestTypeDef

```python
# DeleteStorageConfigurationRequestRequestTypeDef definition

class DeleteStorageConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## S3DetailTypeDef

```python
# S3DetailTypeDef definition

class S3DetailTypeDef(TypedDict):
    recordingPrefix: str,
```

## DisconnectParticipantRequestRequestTypeDef

```python
# DisconnectParticipantRequestRequestTypeDef definition

class DisconnectParticipantRequestRequestTypeDef(TypedDict):
    participantId: str,
    stageArn: str,
    reason: NotRequired[str],
```

## EncoderConfigurationSummaryTypeDef

```python
# EncoderConfigurationSummaryTypeDef definition

class EncoderConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    errorCode: NotRequired[EventErrorCodeType],  # (1)
    eventTime: NotRequired[datetime],
    name: NotRequired[EventNameType],  # (2)
    participantId: NotRequired[str],
    remoteParticipantId: NotRequired[str],
```

1. See [:material-code-brackets: EventErrorCodeType](./literals.md#eventerrorcodetype) 
2. See [:material-code-brackets: EventNameType](./literals.md#eventnametype) 
## GetCompositionRequestRequestTypeDef

```python
# GetCompositionRequestRequestTypeDef definition

class GetCompositionRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetEncoderConfigurationRequestRequestTypeDef

```python
# GetEncoderConfigurationRequestRequestTypeDef definition

class GetEncoderConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetParticipantRequestRequestTypeDef

```python
# GetParticipantRequestRequestTypeDef definition

class GetParticipantRequestRequestTypeDef(TypedDict):
    participantId: str,
    sessionId: str,
    stageArn: str,
```

## ParticipantTypeDef

```python
# ParticipantTypeDef definition

class ParticipantTypeDef(TypedDict):
    attributes: NotRequired[Dict[str, str]],
    browserName: NotRequired[str],
    browserVersion: NotRequired[str],
    firstJoinTime: NotRequired[datetime],
    ispName: NotRequired[str],
    osName: NotRequired[str],
    osVersion: NotRequired[str],
    participantId: NotRequired[str],
    published: NotRequired[bool],
    sdkVersion: NotRequired[str],
    state: NotRequired[ParticipantStateType],  # (1)
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
## GetStageRequestRequestTypeDef

```python
# GetStageRequestRequestTypeDef definition

class GetStageRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetStageSessionRequestRequestTypeDef

```python
# GetStageSessionRequestRequestTypeDef definition

class GetStageSessionRequestRequestTypeDef(TypedDict):
    sessionId: str,
    stageArn: str,
```

## StageSessionTypeDef

```python
# StageSessionTypeDef definition

class StageSessionTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
```

## GetStorageConfigurationRequestRequestTypeDef

```python
# GetStorageConfigurationRequestRequestTypeDef definition

class GetStorageConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GridConfigurationTypeDef

```python
# GridConfigurationTypeDef definition

class GridConfigurationTypeDef(TypedDict):
    featuredParticipantAttribute: NotRequired[str],
```

## ListCompositionsRequestRequestTypeDef

```python
# ListCompositionsRequestRequestTypeDef definition

class ListCompositionsRequestRequestTypeDef(TypedDict):
    filterByEncoderConfigurationArn: NotRequired[str],
    filterByStageArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEncoderConfigurationsRequestRequestTypeDef

```python
# ListEncoderConfigurationsRequestRequestTypeDef definition

class ListEncoderConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListParticipantEventsRequestRequestTypeDef

```python
# ListParticipantEventsRequestRequestTypeDef definition

class ListParticipantEventsRequestRequestTypeDef(TypedDict):
    participantId: str,
    sessionId: str,
    stageArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListParticipantsRequestRequestTypeDef

```python
# ListParticipantsRequestRequestTypeDef definition

class ListParticipantsRequestRequestTypeDef(TypedDict):
    sessionId: str,
    stageArn: str,
    filterByPublished: NotRequired[bool],
    filterByState: NotRequired[ParticipantStateType],  # (1)
    filterByUserId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
## ParticipantSummaryTypeDef

```python
# ParticipantSummaryTypeDef definition

class ParticipantSummaryTypeDef(TypedDict):
    firstJoinTime: NotRequired[datetime],
    participantId: NotRequired[str],
    published: NotRequired[bool],
    state: NotRequired[ParticipantStateType],  # (1)
    userId: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
## ListStageSessionsRequestRequestTypeDef

```python
# ListStageSessionsRequestRequestTypeDef definition

class ListStageSessionsRequestRequestTypeDef(TypedDict):
    stageArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StageSessionSummaryTypeDef

```python
# StageSessionSummaryTypeDef definition

class StageSessionSummaryTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    sessionId: NotRequired[str],
    startTime: NotRequired[datetime],
```

## ListStagesRequestRequestTypeDef

```python
# ListStagesRequestRequestTypeDef definition

class ListStagesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StageSummaryTypeDef

```python
# StageSummaryTypeDef definition

class StageSummaryTypeDef(TypedDict):
    arn: str,
    activeSessionId: NotRequired[str],
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStorageConfigurationsRequestRequestTypeDef

```python
# ListStorageConfigurationsRequestRequestTypeDef definition

class ListStorageConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RecordingConfigurationTypeDef

```python
# RecordingConfigurationTypeDef definition

class RecordingConfigurationTypeDef(TypedDict):
    format: NotRequired[RecordingConfigurationFormatType],  # (1)
```

1. See [:material-code-brackets: RecordingConfigurationFormatType](./literals.md#recordingconfigurationformattype) 
## StopCompositionRequestRequestTypeDef

```python
# StopCompositionRequestRequestTypeDef definition

class StopCompositionRequestRequestTypeDef(TypedDict):
    arn: str,
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

## UpdateStageRequestRequestTypeDef

```python
# UpdateStageRequestRequestTypeDef definition

class UpdateStageRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
```

## CompositionSummaryTypeDef

```python
# CompositionSummaryTypeDef definition

class CompositionSummaryTypeDef(TypedDict):
    arn: str,
    destinations: List[DestinationSummaryTypeDef],  # (1)
    stageArn: str,
    state: CompositionStateType,  # (2)
    endTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef) 
2. See [:material-code-brackets: CompositionStateType](./literals.md#compositionstatetype) 
## CreateEncoderConfigurationRequestRequestTypeDef

```python
# CreateEncoderConfigurationRequestRequestTypeDef definition

class CreateEncoderConfigurationRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    video: NotRequired[VideoTypeDef],  # (1)
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
## EncoderConfigurationTypeDef

```python
# EncoderConfigurationTypeDef definition

class EncoderConfigurationTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    video: NotRequired[VideoTypeDef],  # (1)
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateParticipantTokenResponseTypeDef

```python
# CreateParticipantTokenResponseTypeDef definition

class CreateParticipantTokenResponseTypeDef(TypedDict):
    participantToken: ParticipantTokenTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStageRequestRequestTypeDef

```python
# CreateStageRequestRequestTypeDef definition

class CreateStageRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    participantTokenConfigurations: NotRequired[Sequence[ParticipantTokenConfigurationTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef) 
## CreateStageResponseTypeDef

```python
# CreateStageResponseTypeDef definition

class CreateStageResponseTypeDef(TypedDict):
    participantTokens: List[ParticipantTokenTypeDef],  # (1)
    stage: StageTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef) 
2. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageResponseTypeDef

```python
# GetStageResponseTypeDef definition

class GetStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStageResponseTypeDef

```python
# UpdateStageResponseTypeDef definition

class UpdateStageResponseTypeDef(TypedDict):
    stage: StageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageConfigurationRequestRequestTypeDef

```python
# CreateStorageConfigurationRequestRequestTypeDef definition

class CreateStorageConfigurationRequestRequestTypeDef(TypedDict):
    s3: S3StorageConfigurationTypeDef,  # (1)
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## StorageConfigurationSummaryTypeDef

```python
# StorageConfigurationSummaryTypeDef definition

class StorageConfigurationSummaryTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    s3: NotRequired[S3StorageConfigurationTypeDef],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    s3: NotRequired[S3StorageConfigurationTypeDef],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
## DestinationDetailTypeDef

```python
# DestinationDetailTypeDef definition

class DestinationDetailTypeDef(TypedDict):
    s3: NotRequired[S3DetailTypeDef],  # (1)
```

1. See [:material-code-braces: S3DetailTypeDef](./type_defs.md#s3detailtypedef) 
## ListEncoderConfigurationsResponseTypeDef

```python
# ListEncoderConfigurationsResponseTypeDef definition

class ListEncoderConfigurationsResponseTypeDef(TypedDict):
    encoderConfigurations: List[EncoderConfigurationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationSummaryTypeDef](./type_defs.md#encoderconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListParticipantEventsResponseTypeDef

```python
# ListParticipantEventsResponseTypeDef definition

class ListParticipantEventsResponseTypeDef(TypedDict):
    events: List[EventTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetParticipantResponseTypeDef

```python
# GetParticipantResponseTypeDef definition

class GetParticipantResponseTypeDef(TypedDict):
    participant: ParticipantTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTypeDef](./type_defs.md#participanttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageSessionResponseTypeDef

```python
# GetStageSessionResponseTypeDef definition

class GetStageSessionResponseTypeDef(TypedDict):
    stageSession: StageSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSessionTypeDef](./type_defs.md#stagesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LayoutConfigurationTypeDef

```python
# LayoutConfigurationTypeDef definition

class LayoutConfigurationTypeDef(TypedDict):
    grid: NotRequired[GridConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GridConfigurationTypeDef](./type_defs.md#gridconfigurationtypedef) 
## ListParticipantsResponseTypeDef

```python
# ListParticipantsResponseTypeDef definition

class ListParticipantsResponseTypeDef(TypedDict):
    nextToken: str,
    participants: List[ParticipantSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantSummaryTypeDef](./type_defs.md#participantsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStageSessionsResponseTypeDef

```python
# ListStageSessionsResponseTypeDef definition

class ListStageSessionsResponseTypeDef(TypedDict):
    nextToken: str,
    stageSessions: List[StageSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSessionSummaryTypeDef](./type_defs.md#stagesessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStagesResponseTypeDef

```python
# ListStagesResponseTypeDef definition

class ListStagesResponseTypeDef(TypedDict):
    nextToken: str,
    stages: List[StageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSummaryTypeDef](./type_defs.md#stagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    encoderConfigurationArns: List[str],
    storageConfigurationArn: str,
    recordingConfiguration: NotRequired[RecordingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef) 
## ListCompositionsResponseTypeDef

```python
# ListCompositionsResponseTypeDef definition

class ListCompositionsResponseTypeDef(TypedDict):
    compositions: List[CompositionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionSummaryTypeDef](./type_defs.md#compositionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEncoderConfigurationResponseTypeDef

```python
# CreateEncoderConfigurationResponseTypeDef definition

class CreateEncoderConfigurationResponseTypeDef(TypedDict):
    encoderConfiguration: EncoderConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEncoderConfigurationResponseTypeDef

```python
# GetEncoderConfigurationResponseTypeDef definition

class GetEncoderConfigurationResponseTypeDef(TypedDict):
    encoderConfiguration: EncoderConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStorageConfigurationsResponseTypeDef

```python
# ListStorageConfigurationsResponseTypeDef definition

class ListStorageConfigurationsResponseTypeDef(TypedDict):
    nextToken: str,
    storageConfigurations: List[StorageConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationSummaryTypeDef](./type_defs.md#storageconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageConfigurationResponseTypeDef

```python
# CreateStorageConfigurationResponseTypeDef definition

class CreateStorageConfigurationResponseTypeDef(TypedDict):
    storageConfiguration: StorageConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStorageConfigurationResponseTypeDef

```python
# GetStorageConfigurationResponseTypeDef definition

class GetStorageConfigurationResponseTypeDef(TypedDict):
    storageConfiguration: StorageConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    channel: NotRequired[ChannelDestinationConfigurationTypeDef],  # (1)
    name: NotRequired[str],
    s3: NotRequired[S3DestinationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelDestinationConfigurationTypeDef](./type_defs.md#channeldestinationconfigurationtypedef) 
2. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    configuration: DestinationConfigurationTypeDef,  # (1)
    id: str,
    state: DestinationStateType,  # (3)
    detail: NotRequired[DestinationDetailTypeDef],  # (2)
    endTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: DestinationDetailTypeDef](./type_defs.md#destinationdetailtypedef) 
3. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## StartCompositionRequestRequestTypeDef

```python
# StartCompositionRequestRequestTypeDef definition

class StartCompositionRequestRequestTypeDef(TypedDict):
    destinations: Sequence[DestinationConfigurationTypeDef],  # (1)
    stageArn: str,
    idempotencyToken: NotRequired[str],
    layout: NotRequired[LayoutConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
## CompositionTypeDef

```python
# CompositionTypeDef definition

class CompositionTypeDef(TypedDict):
    arn: str,
    destinations: List[DestinationTypeDef],  # (1)
    layout: LayoutConfigurationTypeDef,  # (2)
    stageArn: str,
    state: CompositionStateType,  # (3)
    endTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
3. See [:material-code-brackets: CompositionStateType](./literals.md#compositionstatetype) 
## GetCompositionResponseTypeDef

```python
# GetCompositionResponseTypeDef definition

class GetCompositionResponseTypeDef(TypedDict):
    composition: CompositionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionTypeDef](./type_defs.md#compositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCompositionResponseTypeDef

```python
# StartCompositionResponseTypeDef definition

class StartCompositionResponseTypeDef(TypedDict):
    composition: CompositionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompositionTypeDef](./type_defs.md#compositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
