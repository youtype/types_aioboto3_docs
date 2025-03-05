# ControlCatalog module

> [Index](../README.md) > ControlCatalog


!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `ControlCatalog` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ControlCatalog` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[controlcatalog]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[controlcatalog]'

# standalone installation
python -m pip install types-aiobotocore-controlcatalog
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-controlcatalog
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ControlCatalogClient

Type annotations and code completion for  `#!python session.client("controlcatalog")` as [ControlCatalogClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#ControlCatalog.Client)

```python
# ControlCatalogClient usage example

from aioboto3.session import Session

from types_aiobotocore_controlcatalog.client import ControlCatalogClient


session = Session()
async with session.client("controlcatalog") as client:
    client: ControlCatalogClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("controlcatalog").get_paginator("...")`.

```python
# ListCommonControlsPaginator usage example

from types_aiobotocore_controlcatalog.paginator import ListCommonControlsPaginator

def get_list_common_controls_paginator() -> ListCommonControlsPaginator:
    return client.get_paginator("list_common_controls"))
```

- [ListCommonControlsPaginator](./paginators.md#listcommoncontrolspaginator)
- [ListControlsPaginator](./paginators.md#listcontrolspaginator)
- [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- [ListObjectivesPaginator](./paginators.md#listobjectivespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ControlBehaviorType usage example

from types_aiobotocore_controlcatalog.literals import ControlBehaviorType

def get_value() -> ControlBehaviorType:
    return "DETECTIVE"
```

- [ControlBehaviorType](./literals.md#controlbehaviortype)
- [ControlScopeType](./literals.md#controlscopetype)
- [ListCommonControlsPaginatorName](./literals.md#listcommoncontrolspaginatorname)
- [ListControlsPaginatorName](./literals.md#listcontrolspaginatorname)
- [ListDomainsPaginatorName](./literals.md#listdomainspaginatorname)
- [ListObjectivesPaginatorName](./literals.md#listobjectivespaginatorname)
- [ControlCatalogServiceName](./literals.md#controlcatalogservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociatedDomainSummaryTypeDef](./type_defs.md#associateddomainsummarytypedef)
- [AssociatedObjectiveSummaryTypeDef](./type_defs.md#associatedobjectivesummarytypedef)
- [ObjectiveResourceFilterTypeDef](./type_defs.md#objectiveresourcefiltertypedef)
- [ControlParameterTypeDef](./type_defs.md#controlparametertypedef)
- [ControlSummaryTypeDef](./type_defs.md#controlsummarytypedef)
- [DomainResourceFilterTypeDef](./type_defs.md#domainresourcefiltertypedef)
- [DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef)
- [GetControlRequestTypeDef](./type_defs.md#getcontrolrequesttypedef)
- [ImplementationDetailsTypeDef](./type_defs.md#implementationdetailstypedef)
- [RegionConfigurationTypeDef](./type_defs.md#regionconfigurationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListControlsRequestTypeDef](./type_defs.md#listcontrolsrequesttypedef)
- [ListDomainsRequestTypeDef](./type_defs.md#listdomainsrequesttypedef)
- [ObjectiveSummaryTypeDef](./type_defs.md#objectivesummarytypedef)
- [CommonControlSummaryTypeDef](./type_defs.md#commoncontrolsummarytypedef)
- [CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef)
- [ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef)
- [GetControlResponseTypeDef](./type_defs.md#getcontrolresponsetypedef)
- [ListControlsResponseTypeDef](./type_defs.md#listcontrolsresponsetypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [ListControlsRequestPaginateTypeDef](./type_defs.md#listcontrolsrequestpaginatetypedef)
- [ListDomainsRequestPaginateTypeDef](./type_defs.md#listdomainsrequestpaginatetypedef)
- [ListObjectivesResponseTypeDef](./type_defs.md#listobjectivesresponsetypedef)
- [ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef)
- [ListCommonControlsRequestPaginateTypeDef](./type_defs.md#listcommoncontrolsrequestpaginatetypedef)
- [ListCommonControlsRequestTypeDef](./type_defs.md#listcommoncontrolsrequesttypedef)
- [ListObjectivesRequestPaginateTypeDef](./type_defs.md#listobjectivesrequestpaginatetypedef)
- [ListObjectivesRequestTypeDef](./type_defs.md#listobjectivesrequesttypedef)

