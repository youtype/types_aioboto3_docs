# CloudWatchObservabilityAccessManager module

> [Index](../README.md) > CloudWatchObservabilityAccessManager


!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAccessManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#cloudwatchobservabilityaccessmanager)
    type annotations stubs module [types-aiobotocore-oam](https://pypi.org/project/types-aiobotocore-oam/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `CloudWatchObservabilityAccessManager` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `CloudWatchObservabilityAccessManager` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[oam]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[oam]'

# standalone installation
python -m pip install types-aiobotocore-oam
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-oam
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchObservabilityAccessManagerClient

Type annotations and code completion for  `#!python session.client("oam")` as [CloudWatchObservabilityAccessManagerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Client)

```python
# CloudWatchObservabilityAccessManagerClient usage example

from aioboto3.session import Session

from types_aiobotocore_oam.client import CloudWatchObservabilityAccessManagerClient


session = Session()
async with session.client("oam") as client:
    client: CloudWatchObservabilityAccessManagerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("oam").get_paginator("...")`.

```python
# ListAttachedLinksPaginator usage example

from types_aiobotocore_oam.paginator import ListAttachedLinksPaginator

def get_list_attached_links_paginator() -> ListAttachedLinksPaginator:
    return client.get_paginator("list_attached_links"))
```

- [ListAttachedLinksPaginator](./paginators.md#listattachedlinkspaginator)
- [ListLinksPaginator](./paginators.md#listlinkspaginator)
- [ListSinksPaginator](./paginators.md#listsinkspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListAttachedLinksPaginatorName usage example

from types_aiobotocore_oam.literals import ListAttachedLinksPaginatorName

def get_value() -> ListAttachedLinksPaginatorName:
    return "list_attached_links"
```

- [ListAttachedLinksPaginatorName](./literals.md#listattachedlinkspaginatorname)
- [ListLinksPaginatorName](./literals.md#listlinkspaginatorname)
- [ListSinksPaginatorName](./literals.md#listsinkspaginatorname)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [CloudWatchObservabilityAccessManagerServiceName](./literals.md#cloudwatchobservabilityaccessmanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateSinkInputRequestTypeDef](./type_defs.md#createsinkinputrequesttypedef)
- [DeleteLinkInputRequestTypeDef](./type_defs.md#deletelinkinputrequesttypedef)
- [DeleteSinkInputRequestTypeDef](./type_defs.md#deletesinkinputrequesttypedef)
- [GetLinkInputRequestTypeDef](./type_defs.md#getlinkinputrequesttypedef)
- [GetSinkInputRequestTypeDef](./type_defs.md#getsinkinputrequesttypedef)
- [GetSinkPolicyInputRequestTypeDef](./type_defs.md#getsinkpolicyinputrequesttypedef)
- [LogGroupConfigurationTypeDef](./type_defs.md#loggroupconfigurationtypedef)
- [MetricConfigurationTypeDef](./type_defs.md#metricconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAttachedLinksInputRequestTypeDef](./type_defs.md#listattachedlinksinputrequesttypedef)
- [ListAttachedLinksItemTypeDef](./type_defs.md#listattachedlinksitemtypedef)
- [ListLinksInputRequestTypeDef](./type_defs.md#listlinksinputrequesttypedef)
- [ListLinksItemTypeDef](./type_defs.md#listlinksitemtypedef)
- [ListSinksInputRequestTypeDef](./type_defs.md#listsinksinputrequesttypedef)
- [ListSinksItemTypeDef](./type_defs.md#listsinksitemtypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [PutSinkPolicyInputRequestTypeDef](./type_defs.md#putsinkpolicyinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [CreateSinkOutputTypeDef](./type_defs.md#createsinkoutputtypedef)
- [GetSinkOutputTypeDef](./type_defs.md#getsinkoutputtypedef)
- [GetSinkPolicyOutputTypeDef](./type_defs.md#getsinkpolicyoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [PutSinkPolicyOutputTypeDef](./type_defs.md#putsinkpolicyoutputtypedef)
- [LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef)
- [ListAttachedLinksInputPaginateTypeDef](./type_defs.md#listattachedlinksinputpaginatetypedef)
- [ListLinksInputPaginateTypeDef](./type_defs.md#listlinksinputpaginatetypedef)
- [ListSinksInputPaginateTypeDef](./type_defs.md#listsinksinputpaginatetypedef)
- [ListAttachedLinksOutputTypeDef](./type_defs.md#listattachedlinksoutputtypedef)
- [ListLinksOutputTypeDef](./type_defs.md#listlinksoutputtypedef)
- [ListSinksOutputTypeDef](./type_defs.md#listsinksoutputtypedef)
- [CreateLinkInputRequestTypeDef](./type_defs.md#createlinkinputrequesttypedef)
- [CreateLinkOutputTypeDef](./type_defs.md#createlinkoutputtypedef)
- [GetLinkOutputTypeDef](./type_defs.md#getlinkoutputtypedef)
- [UpdateLinkInputRequestTypeDef](./type_defs.md#updatelinkinputrequesttypedef)
- [UpdateLinkOutputTypeDef](./type_defs.md#updatelinkoutputtypedef)
