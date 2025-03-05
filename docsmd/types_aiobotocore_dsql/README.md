# AuroraDSQL module

> [Index](../README.md) > AuroraDSQL


!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==14.1.0' mypy-boto3-builder`
1. Select `aioboto3` AWS SDK.
1. Add `AuroraDSQL` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `AuroraDSQL` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[dsql]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[dsql]'

# standalone installation
python -m pip install types-aiobotocore-dsql
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-dsql
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AuroraDSQLClient

Type annotations and code completion for  `#!python session.client("dsql")` as [AuroraDSQLClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#AuroraDSQL.Client)

```python
# AuroraDSQLClient usage example

from aioboto3.session import Session

from types_aiobotocore_dsql.client import AuroraDSQLClient


session = Session()
async with session.client("dsql") as client:
    client: AuroraDSQLClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("dsql").get_paginator("...")`.

```python
# ListClustersPaginator usage example

from types_aiobotocore_dsql.paginator import ListClustersPaginator

def get_list_clusters_paginator() -> ListClustersPaginator:
    return client.get_paginator("list_clusters"))
```

- [ListClustersPaginator](./paginators.md#listclusterspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.client("dsql").get_waiter("...")`.

```python
# ClusterActiveWaiter usage example

from types_aiobotocore_dsql.waiter import ClusterActiveWaiter

def get_cluster_active_waiter() -> ClusterActiveWaiter:
    return Session().client("dsql").get_waiter("cluster_active")
```

- [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)
- [ClusterNotExistsWaiter](./waiters.md#clusternotexistswaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ClusterActiveWaiterName usage example

from types_aiobotocore_dsql.literals import ClusterActiveWaiterName

def get_value() -> ClusterActiveWaiterName:
    return "cluster_active"
```

- [ClusterActiveWaiterName](./literals.md#clusteractivewaitername)
- [ClusterNotExistsWaiterName](./literals.md#clusternotexistswaitername)
- [ClusterStatusType](./literals.md#clusterstatustype)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [AuroraDSQLServiceName](./literals.md#auroradsqlservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef)
- [CreateClusterInputTypeDef](./type_defs.md#createclusterinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LinkedClusterPropertiesTypeDef](./type_defs.md#linkedclusterpropertiestypedef)
- [DeleteClusterInputTypeDef](./type_defs.md#deleteclusterinputtypedef)
- [DeleteMultiRegionClustersInputTypeDef](./type_defs.md#deletemultiregionclustersinputtypedef)
- [GetClusterInputTypeDef](./type_defs.md#getclusterinputtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListClustersInputTypeDef](./type_defs.md#listclustersinputtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateClusterInputTypeDef](./type_defs.md#updateclusterinputtypedef)
- [CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef)
- [CreateMultiRegionClustersOutputTypeDef](./type_defs.md#createmultiregionclustersoutputtypedef)
- [DeleteClusterOutputTypeDef](./type_defs.md#deleteclusteroutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetClusterOutputTypeDef](./type_defs.md#getclusteroutputtypedef)
- [ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [UpdateClusterOutputTypeDef](./type_defs.md#updateclusteroutputtypedef)
- [CreateMultiRegionClustersInputTypeDef](./type_defs.md#createmultiregionclustersinputtypedef)
- [GetClusterInputWaitExtraTypeDef](./type_defs.md#getclusterinputwaitextratypedef)
- [GetClusterInputWaitTypeDef](./type_defs.md#getclusterinputwaittypedef)
- [ListClustersInputPaginateTypeDef](./type_defs.md#listclustersinputpaginatetypedef)

