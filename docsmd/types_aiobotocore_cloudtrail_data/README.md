# CloudTrailDataService module

> [Index](../README.md) > CloudTrailDataService


!!! note ""

    Auto-generated documentation for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice)
    type annotations stubs module [types-aiobotocore-cloudtrail-data](https://pypi.org/project/types-aiobotocore-cloudtrail-data/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `CloudTrailDataService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `CloudTrailDataService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[cloudtrail-data]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[cloudtrail-data]'

# standalone installation
python -m pip install types-aiobotocore-cloudtrail-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudtrail-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudTrailDataServiceClient

Type annotations and code completion for  `#!python session.client("cloudtrail-data")` as [CloudTrailDataServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService.Client)

```python
# CloudTrailDataServiceClient usage example

from aioboto3.session import Session

from types_aiobotocore_cloudtrail_data.client import CloudTrailDataServiceClient


session = Session()
async with session.client("cloudtrail-data") as client:
    client: CloudTrailDataServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CloudTrailDataServiceServiceName usage example

from types_aiobotocore_cloudtrail_data.literals import CloudTrailDataServiceServiceName

def get_value() -> CloudTrailDataServiceServiceName:
    return "cloudtrail-data"
```

- [CloudTrailDataServiceServiceName](./literals.md#cloudtraildataserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AuditEventResultEntryTypeDef](./type_defs.md#auditeventresultentrytypedef)
- [AuditEventTypeDef](./type_defs.md#auditeventtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ResultErrorEntryTypeDef](./type_defs.md#resulterrorentrytypedef)
- [PutAuditEventsRequestRequestTypeDef](./type_defs.md#putauditeventsrequestrequesttypedef)
- [PutAuditEventsResponseTypeDef](./type_defs.md#putauditeventsresponsetypedef)
