# PinpointSMSVoice module

> [Index](../README.md) > PinpointSMSVoice


!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#pinpointsmsvoice)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `PinpointSMSVoice` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `PinpointSMSVoice` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[pinpoint-sms-voice]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[pinpoint-sms-voice]'

# standalone installation
python -m pip install types-aiobotocore-pinpoint-sms-voice
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pinpoint-sms-voice
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PinpointSMSVoiceClient

Type annotations and code completion for  `#!python session.client("pinpoint-sms-voice")` as [PinpointSMSVoiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python
# PinpointSMSVoiceClient usage example

from aioboto3.session import Session

from types_aiobotocore_pinpoint_sms_voice.client import PinpointSMSVoiceClient


session = Session()
async with session.client("pinpoint-sms-voice") as client:
    client: PinpointSMSVoiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EventTypeType usage example

from types_aiobotocore_pinpoint_sms_voice.literals import EventTypeType

def get_value() -> EventTypeType:
    return "ANSWERED"
```

- [EventTypeType](./literals.md#eventtypetype)
- [PinpointSMSVoiceServiceName](./literals.md#pinpointsmsvoiceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CallInstructionsMessageTypeTypeDef](./type_defs.md#callinstructionsmessagetypetypedef)
- [CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef)
- [CreateConfigurationSetRequestTypeDef](./type_defs.md#createconfigurationsetrequesttypedef)
- [DeleteConfigurationSetEventDestinationRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequesttypedef)
- [DeleteConfigurationSetRequestTypeDef](./type_defs.md#deleteconfigurationsetrequesttypedef)
- [KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef)
- [SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef)
- [GetConfigurationSetEventDestinationsRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PlainTextMessageTypeTypeDef](./type_defs.md#plaintextmessagetypetypedef)
- [SSMLMessageTypeTypeDef](./type_defs.md#ssmlmessagetypetypedef)
- [EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef)
- [EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef)
- [SendVoiceMessageResponseTypeDef](./type_defs.md#sendvoicemessageresponsetypedef)
- [VoiceMessageContentTypeDef](./type_defs.md#voicemessagecontenttypedef)
- [CreateConfigurationSetEventDestinationRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequesttypedef)
- [UpdateConfigurationSetEventDestinationRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequesttypedef)
- [GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef)
- [SendVoiceMessageRequestTypeDef](./type_defs.md#sendvoicemessagerequesttypedef)

