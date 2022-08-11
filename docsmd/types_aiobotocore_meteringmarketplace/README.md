# MarketplaceMetering module

> [Index](../README.md) > MarketplaceMetering


!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## How to install



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

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient


session = Session()
async with session.client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_meteringmarketplace.literals import UsageRecordResultStatusType

def get_value() -> UsageRecordResultStatusType:
    return "CustomerNotSubscribed"
```

- [UsageRecordResultStatusType](./literals.md#usagerecordresultstatustype)
- [MarketplaceMeteringServiceName](./literals.md#marketplacemeteringservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_meteringmarketplace.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RegisterUsageRequestRequestTypeDef](./type_defs.md#registerusagerequestrequesttypedef)
- [ResolveCustomerRequestRequestTypeDef](./type_defs.md#resolvecustomerrequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [MeterUsageResultTypeDef](./type_defs.md#meterusageresulttypedef)
- [RegisterUsageResultTypeDef](./type_defs.md#registerusageresulttypedef)
- [ResolveCustomerResultTypeDef](./type_defs.md#resolvecustomerresulttypedef)
- [UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef)
- [MeterUsageRequestRequestTypeDef](./type_defs.md#meterusagerequestrequesttypedef)
- [UsageRecordTypeDef](./type_defs.md#usagerecordtypedef)
- [BatchMeterUsageRequestRequestTypeDef](./type_defs.md#batchmeterusagerequestrequesttypedef)
- [UsageRecordResultTypeDef](./type_defs.md#usagerecordresulttypedef)
- [BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef)

