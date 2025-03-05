# FreeTier module

> [Index](../README.md) > FreeTier


!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `FreeTier` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `FreeTier` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[freetier]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[freetier]'

# standalone installation
python -m pip install types-aiobotocore-freetier
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-freetier
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FreeTierClient

Type annotations and code completion for  `#!python session.client("freetier")` as [FreeTierClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#FreeTier.Client)

```python
# FreeTierClient usage example

from aioboto3.session import Session

from types_aiobotocore_freetier.client import FreeTierClient


session = Session()
async with session.client("freetier") as client:
    client: FreeTierClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("freetier").get_paginator("...")`.

```python
# GetFreeTierUsagePaginator usage example

from types_aiobotocore_freetier.paginator import GetFreeTierUsagePaginator

def get_get_free_tier_usage_paginator() -> GetFreeTierUsagePaginator:
    return client.get_paginator("get_free_tier_usage"))
```

- [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DimensionType usage example

from types_aiobotocore_freetier.literals import DimensionType

def get_value() -> DimensionType:
    return "DESCRIPTION"
```

- [DimensionType](./literals.md#dimensiontype)
- [GetFreeTierUsagePaginatorName](./literals.md#getfreetierusagepaginatorname)
- [MatchOptionType](./literals.md#matchoptiontype)
- [FreeTierServiceName](./literals.md#freetierservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DimensionValuesTypeDef](./type_defs.md#dimensionvaluestypedef)
- [FreeTierUsageTypeDef](./type_defs.md#freetierusagetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef)
- [ExpressionTypeDef](./type_defs.md#expressiontypedef)
- [GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef)
- [GetFreeTierUsageRequestPaginateTypeDef](./type_defs.md#getfreetierusagerequestpaginatetypedef)
- [GetFreeTierUsageRequestTypeDef](./type_defs.md#getfreetierusagerequesttypedef)

