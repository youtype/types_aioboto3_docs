# Pricing module

> [Index](../README.md) > Pricing


!!! note ""

    Auto-generated documentation for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#pricing)
    type annotations stubs module [types-aiobotocore-pricing](https://pypi.org/project/types-aiobotocore-pricing/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Pricing` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Pricing` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[pricing]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[pricing]'

# standalone installation
python -m pip install types-aiobotocore-pricing
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pricing
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PricingClient

Type annotations and code completion for  `#!python session.client("pricing")` as [PricingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client)

```python
# PricingClient usage example

from aioboto3.session import Session

from types_aiobotocore_pricing.client import PricingClient


session = Session()
async with session.client("pricing") as client:
    client: PricingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("pricing").get_paginator("...")`.

```python
# DescribeServicesPaginator usage example

from types_aiobotocore_pricing.paginator import DescribeServicesPaginator

def get_describe_services_paginator() -> DescribeServicesPaginator:
    return client.get_paginator("describe_services"))
```

- [DescribeServicesPaginator](./paginators.md#describeservicespaginator)
- [GetAttributeValuesPaginator](./paginators.md#getattributevaluespaginator)
- [GetProductsPaginator](./paginators.md#getproductspaginator)
- [ListPriceListsPaginator](./paginators.md#listpricelistspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DescribeServicesPaginatorName usage example

from types_aiobotocore_pricing.literals import DescribeServicesPaginatorName

def get_value() -> DescribeServicesPaginatorName:
    return "describe_services"
```

- [DescribeServicesPaginatorName](./literals.md#describeservicespaginatorname)
- [FilterTypeType](./literals.md#filtertypetype)
- [GetAttributeValuesPaginatorName](./literals.md#getattributevaluespaginatorname)
- [GetProductsPaginatorName](./literals.md#getproductspaginatorname)
- [ListPriceListsPaginatorName](./literals.md#listpricelistspaginatorname)
- [PricingServiceName](./literals.md#pricingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetAttributeValuesRequestRequestTypeDef](./type_defs.md#getattributevaluesrequestrequesttypedef)
- [GetPriceListFileUrlRequestRequestTypeDef](./type_defs.md#getpricelistfileurlrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PriceListTypeDef](./type_defs.md#pricelisttypedef)
- [DescribeServicesRequestPaginateTypeDef](./type_defs.md#describeservicesrequestpaginatetypedef)
- [GetAttributeValuesRequestPaginateTypeDef](./type_defs.md#getattributevaluesrequestpaginatetypedef)
- [GetAttributeValuesResponseTypeDef](./type_defs.md#getattributevaluesresponsetypedef)
- [GetPriceListFileUrlResponseTypeDef](./type_defs.md#getpricelistfileurlresponsetypedef)
- [GetProductsResponseTypeDef](./type_defs.md#getproductsresponsetypedef)
- [DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)
- [GetProductsRequestPaginateTypeDef](./type_defs.md#getproductsrequestpaginatetypedef)
- [GetProductsRequestRequestTypeDef](./type_defs.md#getproductsrequestrequesttypedef)
- [ListPriceListsRequestPaginateTypeDef](./type_defs.md#listpricelistsrequestpaginatetypedef)
- [ListPriceListsRequestRequestTypeDef](./type_defs.md#listpricelistsrequestrequesttypedef)
- [ListPriceListsResponseTypeDef](./type_defs.md#listpricelistsresponsetypedef)
