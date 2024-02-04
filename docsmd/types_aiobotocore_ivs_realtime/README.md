# ivsrealtime module

> [Index](../README.md) > ivsrealtime


!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `ivsrealtime` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[ivs-realtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[ivs-realtime]'


# standalone installation
python -m pip install types-aiobotocore-ivs-realtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ivs-realtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ivsrealtimeClient

Type annotations and code completion for  `#!python session.client("ivs-realtime")` as [ivsrealtimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client)

```python
# ivsrealtimeClient usage example

from aioboto3.session import Session

from types_aiobotocore_ivs_realtime.client import ivsrealtimeClient


session = Session()
async with session.client("ivs-realtime") as client:
    client: ivsrealtimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CompositionStateType usage example

from types_aiobotocore_ivs_realtime.literals import CompositionStateType

def get_value() -> CompositionStateType:
    return "ACTIVE"
```

- [CompositionStateType](./literals.md#compositionstatetype)
- [DestinationStateType](./literals.md#destinationstatetype)
- [EventErrorCodeType](./literals.md#eventerrorcodetype)
- [EventNameType](./literals.md#eventnametype)
- [ParticipantStateType](./literals.md#participantstatetype)
- [ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype)
- [RecordingConfigurationFormatType](./literals.md#recordingconfigurationformattype)
- [ivsrealtimeServiceName](./literals.md#ivsrealtimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ChannelDestinationConfigurationTypeDef](./type_defs.md#channeldestinationconfigurationtypedef)
- [DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef)
- [VideoTypeDef](./type_defs.md#videotypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateParticipantTokenRequestRequestTypeDef](./type_defs.md#createparticipanttokenrequestrequesttypedef)
- [ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef)
- [ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef)
- [StageTypeDef](./type_defs.md#stagetypedef)
- [S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef)
- [DeleteEncoderConfigurationRequestRequestTypeDef](./type_defs.md#deleteencoderconfigurationrequestrequesttypedef)
- [DeleteStageRequestRequestTypeDef](./type_defs.md#deletestagerequestrequesttypedef)
- [DeleteStorageConfigurationRequestRequestTypeDef](./type_defs.md#deletestorageconfigurationrequestrequesttypedef)
- [S3DetailTypeDef](./type_defs.md#s3detailtypedef)
- [DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef)
- [EncoderConfigurationSummaryTypeDef](./type_defs.md#encoderconfigurationsummarytypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [GetCompositionRequestRequestTypeDef](./type_defs.md#getcompositionrequestrequesttypedef)
- [GetEncoderConfigurationRequestRequestTypeDef](./type_defs.md#getencoderconfigurationrequestrequesttypedef)
- [GetParticipantRequestRequestTypeDef](./type_defs.md#getparticipantrequestrequesttypedef)
- [ParticipantTypeDef](./type_defs.md#participanttypedef)
- [GetStageRequestRequestTypeDef](./type_defs.md#getstagerequestrequesttypedef)
- [GetStageSessionRequestRequestTypeDef](./type_defs.md#getstagesessionrequestrequesttypedef)
- [StageSessionTypeDef](./type_defs.md#stagesessiontypedef)
- [GetStorageConfigurationRequestRequestTypeDef](./type_defs.md#getstorageconfigurationrequestrequesttypedef)
- [GridConfigurationTypeDef](./type_defs.md#gridconfigurationtypedef)
- [ListCompositionsRequestRequestTypeDef](./type_defs.md#listcompositionsrequestrequesttypedef)
- [ListEncoderConfigurationsRequestRequestTypeDef](./type_defs.md#listencoderconfigurationsrequestrequesttypedef)
- [ListParticipantEventsRequestRequestTypeDef](./type_defs.md#listparticipanteventsrequestrequesttypedef)
- [ListParticipantsRequestRequestTypeDef](./type_defs.md#listparticipantsrequestrequesttypedef)
- [ParticipantSummaryTypeDef](./type_defs.md#participantsummarytypedef)
- [ListStageSessionsRequestRequestTypeDef](./type_defs.md#liststagesessionsrequestrequesttypedef)
- [StageSessionSummaryTypeDef](./type_defs.md#stagesessionsummarytypedef)
- [ListStagesRequestRequestTypeDef](./type_defs.md#liststagesrequestrequesttypedef)
- [StageSummaryTypeDef](./type_defs.md#stagesummarytypedef)
- [ListStorageConfigurationsRequestRequestTypeDef](./type_defs.md#liststorageconfigurationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef)
- [StopCompositionRequestRequestTypeDef](./type_defs.md#stopcompositionrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateStageRequestRequestTypeDef](./type_defs.md#updatestagerequestrequesttypedef)
- [CompositionSummaryTypeDef](./type_defs.md#compositionsummarytypedef)
- [CreateEncoderConfigurationRequestRequestTypeDef](./type_defs.md#createencoderconfigurationrequestrequesttypedef)
- [EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateParticipantTokenResponseTypeDef](./type_defs.md#createparticipanttokenresponsetypedef)
- [CreateStageRequestRequestTypeDef](./type_defs.md#createstagerequestrequesttypedef)
- [CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef)
- [GetStageResponseTypeDef](./type_defs.md#getstageresponsetypedef)
- [UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef)
- [CreateStorageConfigurationRequestRequestTypeDef](./type_defs.md#createstorageconfigurationrequestrequesttypedef)
- [StorageConfigurationSummaryTypeDef](./type_defs.md#storageconfigurationsummarytypedef)
- [StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)
- [DestinationDetailTypeDef](./type_defs.md#destinationdetailtypedef)
- [ListEncoderConfigurationsResponseTypeDef](./type_defs.md#listencoderconfigurationsresponsetypedef)
- [ListParticipantEventsResponseTypeDef](./type_defs.md#listparticipanteventsresponsetypedef)
- [GetParticipantResponseTypeDef](./type_defs.md#getparticipantresponsetypedef)
- [GetStageSessionResponseTypeDef](./type_defs.md#getstagesessionresponsetypedef)
- [LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef)
- [ListParticipantsResponseTypeDef](./type_defs.md#listparticipantsresponsetypedef)
- [ListStageSessionsResponseTypeDef](./type_defs.md#liststagesessionsresponsetypedef)
- [ListStagesResponseTypeDef](./type_defs.md#liststagesresponsetypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [ListCompositionsResponseTypeDef](./type_defs.md#listcompositionsresponsetypedef)
- [CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef)
- [GetEncoderConfigurationResponseTypeDef](./type_defs.md#getencoderconfigurationresponsetypedef)
- [ListStorageConfigurationsResponseTypeDef](./type_defs.md#liststorageconfigurationsresponsetypedef)
- [CreateStorageConfigurationResponseTypeDef](./type_defs.md#createstorageconfigurationresponsetypedef)
- [GetStorageConfigurationResponseTypeDef](./type_defs.md#getstorageconfigurationresponsetypedef)
- [DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [StartCompositionRequestRequestTypeDef](./type_defs.md#startcompositionrequestrequesttypedef)
- [CompositionTypeDef](./type_defs.md#compositiontypedef)
- [GetCompositionResponseTypeDef](./type_defs.md#getcompositionresponsetypedef)
- [StartCompositionResponseTypeDef](./type_defs.md#startcompositionresponsetypedef)

