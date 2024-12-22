# Billing module

> [Index](../README.md) > Billing


!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Billing` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Billing` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[billing]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[billing]'

# standalone installation
python -m pip install types-aiobotocore-billing
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-billing
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BillingClient

Type annotations and code completion for  `#!python session.client("billing")` as [BillingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# BillingClient usage example

from aioboto3.session import Session

from types_aiobotocore_billing.client import BillingClient


session = Session()
async with session.client("billing") as client:
    client: BillingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("billing").get_paginator("...")`.

```python
# ListBillingViewsPaginator usage example

from types_aiobotocore_billing.paginator import ListBillingViewsPaginator

def get_list_billing_views_paginator() -> ListBillingViewsPaginator:
    return client.get_paginator("list_billing_views"))
```

- [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BillingViewTypeType usage example

from types_aiobotocore_billing.literals import BillingViewTypeType

def get_value() -> BillingViewTypeType:
    return "BILLING_GROUP"
```

- [BillingViewTypeType](./literals.md#billingviewtypetype)
- [ListBillingViewsPaginatorName](./literals.md#listbillingviewspaginatorname)
- [BillingServiceName](./literals.md#billingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [BillingViewListElementTypeDef](./type_defs.md#billingviewlistelementtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef)
- [ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef)
- [ListBillingViewsRequestPaginateTypeDef](./type_defs.md#listbillingviewsrequestpaginatetypedef)
- [ListBillingViewsRequestRequestTypeDef](./type_defs.md#listbillingviewsrequestrequesttypedef)

