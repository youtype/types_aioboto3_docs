# MarketplaceMetering module

> [Index](../README.md) > MarketplaceMetering


!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `MarketplaceMetering` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `MarketplaceMetering` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[meteringmarketplace]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[meteringmarketplace]'

# standalone installation
python -m pip install types-aiobotocore-meteringmarketplace
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-meteringmarketplace
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceMeteringClient

Type annotations and code completion for  `#!python session.client("meteringmarketplace")` as [MarketplaceMeteringClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

```python
# MarketplaceMeteringClient usage example

from aioboto3.session import Session

from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient


session = Session()
async with session.client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# UsageRecordResultStatusType usage example

from types_aiobotocore_meteringmarketplace.literals import UsageRecordResultStatusType

def get_value() -> UsageRecordResultStatusType:
    return "CustomerNotSubscribed"
```

- [UsageRecordResultStatusType](./literals.md#usagerecordresultstatustype)
- [MarketplaceMeteringServiceName](./literals.md#marketplacemeteringservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RegisterUsageRequestRequestTypeDef](./type_defs.md#registerusagerequestrequesttypedef)
- [ResolveCustomerRequestRequestTypeDef](./type_defs.md#resolvecustomerrequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [MeterUsageResultTypeDef](./type_defs.md#meterusageresulttypedef)
- [RegisterUsageResultTypeDef](./type_defs.md#registerusageresulttypedef)
- [ResolveCustomerResultTypeDef](./type_defs.md#resolvecustomerresulttypedef)
- [UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef)
- [UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef)
- [UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef)
- [UsageAllocationUnionTypeDef](./type_defs.md#usageallocationuniontypedef)
- [UsageRecordResultTypeDef](./type_defs.md#usagerecordresulttypedef)
- [MeterUsageRequestRequestTypeDef](./type_defs.md#meterusagerequestrequesttypedef)
- [UsageRecordTypeDef](./type_defs.md#usagerecordtypedef)
- [BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef)
- [UsageRecordUnionTypeDef](./type_defs.md#usagerecorduniontypedef)
- [BatchMeterUsageRequestRequestTypeDef](./type_defs.md#batchmeterusagerequestrequesttypedef)
