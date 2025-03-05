# ConnectParticipant module

> [Index](../README.md) > ConnectParticipant


!!! note ""

    Auto-generated documentation for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#connectparticipant)
    type annotations stubs module [types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `ConnectParticipant` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ConnectParticipant` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[connectparticipant]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[connectparticipant]'

# standalone installation
python -m pip install types-aiobotocore-connectparticipant
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectparticipant
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectParticipantClient

Type annotations and code completion for  `#!python session.client("connectparticipant")` as [ConnectParticipantClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant.Client)

```python
# ConnectParticipantClient usage example

from aioboto3.session import Session

from types_aiobotocore_connectparticipant.client import ConnectParticipantClient


session = Session()
async with session.client("connectparticipant") as client:
    client: ConnectParticipantClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ArtifactStatusType usage example

from types_aiobotocore_connectparticipant.literals import ArtifactStatusType

def get_value() -> ArtifactStatusType:
    return "APPROVED"
```

- [ArtifactStatusType](./literals.md#artifactstatustype)
- [ChatItemTypeType](./literals.md#chatitemtypetype)
- [ConnectionTypeType](./literals.md#connectiontypetype)
- [ParticipantRoleType](./literals.md#participantroletype)
- [ScanDirectionType](./literals.md#scandirectiontype)
- [SortKeyType](./literals.md#sortkeytype)
- [ConnectParticipantServiceName](./literals.md#connectparticipantservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttachmentItemTypeDef](./type_defs.md#attachmentitemtypedef)
- [CancelParticipantAuthenticationRequestTypeDef](./type_defs.md#cancelparticipantauthenticationrequesttypedef)
- [CompleteAttachmentUploadRequestTypeDef](./type_defs.md#completeattachmentuploadrequesttypedef)
- [ConnectionCredentialsTypeDef](./type_defs.md#connectioncredentialstypedef)
- [CreateParticipantConnectionRequestTypeDef](./type_defs.md#createparticipantconnectionrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [WebsocketTypeDef](./type_defs.md#websockettypedef)
- [DescribeViewRequestTypeDef](./type_defs.md#describeviewrequesttypedef)
- [DisconnectParticipantRequestTypeDef](./type_defs.md#disconnectparticipantrequesttypedef)
- [GetAttachmentRequestTypeDef](./type_defs.md#getattachmentrequesttypedef)
- [GetAuthenticationUrlRequestTypeDef](./type_defs.md#getauthenticationurlrequesttypedef)
- [StartPositionTypeDef](./type_defs.md#startpositiontypedef)
- [ReceiptTypeDef](./type_defs.md#receipttypedef)
- [SendEventRequestTypeDef](./type_defs.md#sendeventrequesttypedef)
- [SendMessageRequestTypeDef](./type_defs.md#sendmessagerequesttypedef)
- [StartAttachmentUploadRequestTypeDef](./type_defs.md#startattachmentuploadrequesttypedef)
- [UploadMetadataTypeDef](./type_defs.md#uploadmetadatatypedef)
- [ViewContentTypeDef](./type_defs.md#viewcontenttypedef)
- [GetAttachmentResponseTypeDef](./type_defs.md#getattachmentresponsetypedef)
- [GetAuthenticationUrlResponseTypeDef](./type_defs.md#getauthenticationurlresponsetypedef)
- [SendEventResponseTypeDef](./type_defs.md#sendeventresponsetypedef)
- [SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef)
- [CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef)
- [GetTranscriptRequestTypeDef](./type_defs.md#gettranscriptrequesttypedef)
- [MessageMetadataTypeDef](./type_defs.md#messagemetadatatypedef)
- [StartAttachmentUploadResponseTypeDef](./type_defs.md#startattachmentuploadresponsetypedef)
- [ViewTypeDef](./type_defs.md#viewtypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [DescribeViewResponseTypeDef](./type_defs.md#describeviewresponsetypedef)
- [GetTranscriptResponseTypeDef](./type_defs.md#gettranscriptresponsetypedef)

