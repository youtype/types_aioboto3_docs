# LexRuntimeService module

> [Index](../README.md) > LexRuntimeService


!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `LexRuntimeService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `LexRuntimeService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[lex-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[lex-runtime]'

# standalone installation
python -m pip install types-aiobotocore-lex-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lex-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LexRuntimeServiceClient

Type annotations and code completion for  `#!python session.client("lex-runtime")` as [LexRuntimeServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python
# LexRuntimeServiceClient usage example

from aioboto3.session import Session

from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient


session = Session()
async with session.client("lex-runtime") as client:
    client: LexRuntimeServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConfirmationStatusType usage example

from types_aiobotocore_lex_runtime.literals import ConfirmationStatusType

def get_value() -> ConfirmationStatusType:
    return "Confirmed"
```

- [ConfirmationStatusType](./literals.md#confirmationstatustype)
- [ContentTypeType](./literals.md#contenttypetype)
- [DialogActionTypeType](./literals.md#dialogactiontypetype)
- [DialogStateType](./literals.md#dialogstatetype)
- [FulfillmentStateType](./literals.md#fulfillmentstatetype)
- [MessageFormatTypeType](./literals.md#messageformattypetype)
- [LexRuntimeServiceServiceName](./literals.md#lexruntimeserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ButtonTypeDef](./type_defs.md#buttontypedef)
- [DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DialogActionOutputTypeDef](./type_defs.md#dialogactionoutputtypedef)
- [DialogActionTypeDef](./type_defs.md#dialogactiontypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [IntentSummaryOutputTypeDef](./type_defs.md#intentsummaryoutputtypedef)
- [IntentConfidenceTypeDef](./type_defs.md#intentconfidencetypedef)
- [IntentSummaryTypeDef](./type_defs.md#intentsummarytypedef)
- [SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef)
- [ActiveContextOutputTypeDef](./type_defs.md#activecontextoutputtypedef)
- [ActiveContextTypeDef](./type_defs.md#activecontexttypedef)
- [PostContentRequestRequestTypeDef](./type_defs.md#postcontentrequestrequesttypedef)
- [GenericAttachmentTypeDef](./type_defs.md#genericattachmenttypedef)
- [DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)
- [PostContentResponseTypeDef](./type_defs.md#postcontentresponsetypedef)
- [PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef)
- [PredictedIntentTypeDef](./type_defs.md#predictedintenttypedef)
- [IntentSummaryUnionTypeDef](./type_defs.md#intentsummaryuniontypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [ActiveContextUnionTypeDef](./type_defs.md#activecontextuniontypedef)
- [ResponseCardTypeDef](./type_defs.md#responsecardtypedef)
- [PutSessionRequestRequestTypeDef](./type_defs.md#putsessionrequestrequesttypedef)
- [PostTextRequestRequestTypeDef](./type_defs.md#posttextrequestrequesttypedef)
- [PostTextResponseTypeDef](./type_defs.md#posttextresponsetypedef)
