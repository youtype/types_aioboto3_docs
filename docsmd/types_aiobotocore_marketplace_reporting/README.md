# MarketplaceReportingService module

> [Index](../README.md) > MarketplaceReportingService


!!! note ""

    Auto-generated documentation for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice)
    type annotations stubs module [types-aiobotocore-marketplace-reporting](https://pypi.org/project/types-aiobotocore-marketplace-reporting/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `MarketplaceReportingService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `MarketplaceReportingService` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[marketplace-reporting]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[marketplace-reporting]'

# standalone installation
python -m pip install types-aiobotocore-marketplace-reporting
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-marketplace-reporting
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceReportingServiceClient

Type annotations and code completion for  `#!python session.client("marketplace-reporting")` as [MarketplaceReportingServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#MarketplaceReportingService.Client)

```python
# MarketplaceReportingServiceClient usage example

from aioboto3.session import Session

from types_aiobotocore_marketplace_reporting.client import MarketplaceReportingServiceClient


session = Session()
async with session.client("marketplace-reporting") as client:
    client: MarketplaceReportingServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# MarketplaceReportingServiceServiceName usage example

from types_aiobotocore_marketplace_reporting.literals import MarketplaceReportingServiceServiceName

def get_value() -> MarketplaceReportingServiceServiceName:
    return "marketplace-reporting"
```

- [MarketplaceReportingServiceServiceName](./literals.md#marketplacereportingserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetBuyerDashboardInputRequestTypeDef](./type_defs.md#getbuyerdashboardinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetBuyerDashboardOutputTypeDef](./type_defs.md#getbuyerdashboardoutputtypedef)
