# CognitoSync module

> [Index](../README.md) > CognitoSync


!!! note ""

    Auto-generated documentation for [CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#cognitosync)
    type annotations stubs module [types-aiobotocore-cognito-sync](https://pypi.org/project/types-aiobotocore-cognito-sync/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `CognitoSync` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `CognitoSync` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[cognito-sync]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[cognito-sync]'

# standalone installation
python -m pip install types-aiobotocore-cognito-sync
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cognito-sync
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CognitoSyncClient

Type annotations and code completion for  `#!python session.client("cognito-sync")` as [CognitoSyncClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client)

```python
# CognitoSyncClient usage example

from aioboto3.session import Session

from types_aiobotocore_cognito_sync.client import CognitoSyncClient


session = Session()
async with session.client("cognito-sync") as client:
    client: CognitoSyncClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BulkPublishStatusType usage example

from types_aiobotocore_cognito_sync.literals import BulkPublishStatusType

def get_value() -> BulkPublishStatusType:
    return "FAILED"
```

- [BulkPublishStatusType](./literals.md#bulkpublishstatustype)
- [OperationType](./literals.md#operationtype)
- [PlatformType](./literals.md#platformtype)
- [StreamingStatusType](./literals.md#streamingstatustype)
- [CognitoSyncServiceName](./literals.md#cognitosyncservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BulkPublishRequestRequestTypeDef](./type_defs.md#bulkpublishrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef)
- [DatasetTypeDef](./type_defs.md#datasettypedef)
- [DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef)
- [DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef)
- [DescribeIdentityPoolUsageRequestRequestTypeDef](./type_defs.md#describeidentitypoolusagerequestrequesttypedef)
- [IdentityPoolUsageTypeDef](./type_defs.md#identitypoolusagetypedef)
- [DescribeIdentityUsageRequestRequestTypeDef](./type_defs.md#describeidentityusagerequestrequesttypedef)
- [IdentityUsageTypeDef](./type_defs.md#identityusagetypedef)
- [GetBulkPublishDetailsRequestRequestTypeDef](./type_defs.md#getbulkpublishdetailsrequestrequesttypedef)
- [GetCognitoEventsRequestRequestTypeDef](./type_defs.md#getcognitoeventsrequestrequesttypedef)
- [GetIdentityPoolConfigurationRequestRequestTypeDef](./type_defs.md#getidentitypoolconfigurationrequestrequesttypedef)
- [PushSyncOutputTypeDef](./type_defs.md#pushsyncoutputtypedef)
- [ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef)
- [ListIdentityPoolUsageRequestRequestTypeDef](./type_defs.md#listidentitypoolusagerequestrequesttypedef)
- [ListRecordsRequestRequestTypeDef](./type_defs.md#listrecordsrequestrequesttypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [PushSyncTypeDef](./type_defs.md#pushsynctypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RegisterDeviceRequestRequestTypeDef](./type_defs.md#registerdevicerequestrequesttypedef)
- [SetCognitoEventsRequestRequestTypeDef](./type_defs.md#setcognitoeventsrequestrequesttypedef)
- [SubscribeToDatasetRequestRequestTypeDef](./type_defs.md#subscribetodatasetrequestrequesttypedef)
- [UnsubscribeFromDatasetRequestRequestTypeDef](./type_defs.md#unsubscribefromdatasetrequestrequesttypedef)
- [BulkPublishResponseTypeDef](./type_defs.md#bulkpublishresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetBulkPublishDetailsResponseTypeDef](./type_defs.md#getbulkpublishdetailsresponsetypedef)
- [GetCognitoEventsResponseTypeDef](./type_defs.md#getcognitoeventsresponsetypedef)
- [RegisterDeviceResponseTypeDef](./type_defs.md#registerdeviceresponsetypedef)
- [DeleteDatasetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef)
- [DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)
- [ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)
- [DescribeIdentityPoolUsageResponseTypeDef](./type_defs.md#describeidentitypoolusageresponsetypedef)
- [ListIdentityPoolUsageResponseTypeDef](./type_defs.md#listidentitypoolusageresponsetypedef)
- [DescribeIdentityUsageResponseTypeDef](./type_defs.md#describeidentityusageresponsetypedef)
- [GetIdentityPoolConfigurationResponseTypeDef](./type_defs.md#getidentitypoolconfigurationresponsetypedef)
- [SetIdentityPoolConfigurationResponseTypeDef](./type_defs.md#setidentitypoolconfigurationresponsetypedef)
- [ListRecordsResponseTypeDef](./type_defs.md#listrecordsresponsetypedef)
- [UpdateRecordsResponseTypeDef](./type_defs.md#updaterecordsresponsetypedef)
- [SetIdentityPoolConfigurationRequestRequestTypeDef](./type_defs.md#setidentitypoolconfigurationrequestrequesttypedef)
- [RecordPatchTypeDef](./type_defs.md#recordpatchtypedef)
- [UpdateRecordsRequestRequestTypeDef](./type_defs.md#updaterecordsrequestrequesttypedef)
