# PinpointSMSVoice module

> [Index](../README.md) > PinpointSMSVoice


!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
    type annotations stubs module [types-aiobotocore-sms-voice](https://pypi.org/project/types-aiobotocore-sms-voice/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `PinpointSMSVoice`.

### From PyPI with pip

Install `types-aioboto3` for `PinpointSMSVoice` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sms-voice]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sms-voice]'


# standalone installation
python -m pip install types-aiobotocore-sms-voice
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sms-voice
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PinpointSMSVoiceClient

Type annotations and code completion for  `#!python session.client("sms-voice")` as [PinpointSMSVoiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sms_voice.client import PinpointSMSVoiceClient


session = Session()
async with session.client("sms-voice") as client:
    client: PinpointSMSVoiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sms_voice.literals import EventTypeType

def get_value() -> EventTypeType:
    return "ANSWERED"
```

- [EventTypeType](./literals.md#eventtypetype)
- [PinpointSMSVoiceServiceName](./literals.md#pinpointsmsvoiceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sms_voice.type_defs import CallInstructionsMessageTypeTypeDef

def get_value() -> CallInstructionsMessageTypeTypeDef:
    return {
        "Text": ...,
    }
```

- [CallInstructionsMessageTypeTypeDef](./type_defs.md#callinstructionsmessagetypetypedef)
- [CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef)
- [CreateConfigurationSetRequestRequestTypeDef](./type_defs.md#createconfigurationsetrequestrequesttypedef)
- [DeleteConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequestrequesttypedef)
- [DeleteConfigurationSetRequestRequestTypeDef](./type_defs.md#deleteconfigurationsetrequestrequesttypedef)
- [KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef)
- [SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef)
- [GetConfigurationSetEventDestinationsRequestRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ListConfigurationSetsRequestRequestTypeDef](./type_defs.md#listconfigurationsetsrequestrequesttypedef)
- [PlainTextMessageTypeTypeDef](./type_defs.md#plaintextmessagetypetypedef)
- [SSMLMessageTypeTypeDef](./type_defs.md#ssmlmessagetypetypedef)
- [EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef)
- [EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef)
- [ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef)
- [SendVoiceMessageResponseTypeDef](./type_defs.md#sendvoicemessageresponsetypedef)
- [VoiceMessageContentTypeDef](./type_defs.md#voicemessagecontenttypedef)
- [CreateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequestrequesttypedef)
- [UpdateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequestrequesttypedef)
- [GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef)
- [SendVoiceMessageRequestRequestTypeDef](./type_defs.md#sendvoicemessagerequestrequesttypedef)

