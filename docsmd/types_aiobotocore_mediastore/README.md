# MediaStore module

> [Index](../README.md) > MediaStore


!!! note ""

    Auto-generated documentation for [MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#mediastore)
    type annotations stubs module [types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `MediaStore` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `MediaStore` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[mediastore]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[mediastore]'

# standalone installation
python -m pip install types-aiobotocore-mediastore
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mediastore
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MediaStoreClient

Type annotations and code completion for  `#!python session.client("mediastore")` as [MediaStoreClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Client)

```python
# MediaStoreClient usage example

from aioboto3.session import Session

from types_aiobotocore_mediastore.client import MediaStoreClient


session = Session()
async with session.client("mediastore") as client:
    client: MediaStoreClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("mediastore").get_paginator("...")`.

```python
# ListContainersPaginator usage example

from types_aiobotocore_mediastore.paginator import ListContainersPaginator

def get_list_containers_paginator() -> ListContainersPaginator:
    return client.get_paginator("list_containers"))
```

- [ListContainersPaginator](./paginators.md#listcontainerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ContainerLevelMetricsType usage example

from types_aiobotocore_mediastore.literals import ContainerLevelMetricsType

def get_value() -> ContainerLevelMetricsType:
    return "DISABLED"
```

- [ContainerLevelMetricsType](./literals.md#containerlevelmetricstype)
- [ContainerStatusType](./literals.md#containerstatustype)
- [ListContainersPaginatorName](./literals.md#listcontainerspaginatorname)
- [MethodNameType](./literals.md#methodnametype)
- [MediaStoreServiceName](./literals.md#mediastoreservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ContainerTypeDef](./type_defs.md#containertypedef)
- [CorsRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef)
- [CorsRuleTypeDef](./type_defs.md#corsruletypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteContainerInputRequestTypeDef](./type_defs.md#deletecontainerinputrequesttypedef)
- [DeleteContainerPolicyInputRequestTypeDef](./type_defs.md#deletecontainerpolicyinputrequesttypedef)
- [DeleteCorsPolicyInputRequestTypeDef](./type_defs.md#deletecorspolicyinputrequesttypedef)
- [DeleteLifecyclePolicyInputRequestTypeDef](./type_defs.md#deletelifecyclepolicyinputrequesttypedef)
- [DeleteMetricPolicyInputRequestTypeDef](./type_defs.md#deletemetricpolicyinputrequesttypedef)
- [DescribeContainerInputRequestTypeDef](./type_defs.md#describecontainerinputrequesttypedef)
- [GetContainerPolicyInputRequestTypeDef](./type_defs.md#getcontainerpolicyinputrequesttypedef)
- [GetCorsPolicyInputRequestTypeDef](./type_defs.md#getcorspolicyinputrequesttypedef)
- [GetLifecyclePolicyInputRequestTypeDef](./type_defs.md#getlifecyclepolicyinputrequesttypedef)
- [GetMetricPolicyInputRequestTypeDef](./type_defs.md#getmetricpolicyinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListContainersInputRequestTypeDef](./type_defs.md#listcontainersinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [MetricPolicyRuleTypeDef](./type_defs.md#metricpolicyruletypedef)
- [PutContainerPolicyInputRequestTypeDef](./type_defs.md#putcontainerpolicyinputrequesttypedef)
- [PutLifecyclePolicyInputRequestTypeDef](./type_defs.md#putlifecyclepolicyinputrequesttypedef)
- [StartAccessLoggingInputRequestTypeDef](./type_defs.md#startaccesslogginginputrequesttypedef)
- [StopAccessLoggingInputRequestTypeDef](./type_defs.md#stopaccesslogginginputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [CorsRuleUnionTypeDef](./type_defs.md#corsruleuniontypedef)
- [CreateContainerInputRequestTypeDef](./type_defs.md#createcontainerinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [CreateContainerOutputTypeDef](./type_defs.md#createcontaineroutputtypedef)
- [DescribeContainerOutputTypeDef](./type_defs.md#describecontaineroutputtypedef)
- [GetContainerPolicyOutputTypeDef](./type_defs.md#getcontainerpolicyoutputtypedef)
- [GetCorsPolicyOutputTypeDef](./type_defs.md#getcorspolicyoutputtypedef)
- [GetLifecyclePolicyOutputTypeDef](./type_defs.md#getlifecyclepolicyoutputtypedef)
- [ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ListContainersInputPaginateTypeDef](./type_defs.md#listcontainersinputpaginatetypedef)
- [MetricPolicyOutputTypeDef](./type_defs.md#metricpolicyoutputtypedef)
- [MetricPolicyTypeDef](./type_defs.md#metricpolicytypedef)
- [PutCorsPolicyInputRequestTypeDef](./type_defs.md#putcorspolicyinputrequesttypedef)
- [GetMetricPolicyOutputTypeDef](./type_defs.md#getmetricpolicyoutputtypedef)
- [PutMetricPolicyInputRequestTypeDef](./type_defs.md#putmetricpolicyinputrequesttypedef)
