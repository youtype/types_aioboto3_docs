# S3Outposts module

> [Index](../README.md) > S3Outposts


!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#s3outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `S3Outposts` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `S3Outposts` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[s3outposts]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[s3outposts]'

# standalone installation
python -m pip install types-aiobotocore-s3outposts
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-s3outposts
```

## Usage

Code samples can be found in [Examples](./usage.md).

## S3OutpostsClient

Type annotations and code completion for  `#!python session.client("s3outposts")` as [S3OutpostsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Client)

```python
# S3OutpostsClient usage example

from aioboto3.session import Session

from types_aiobotocore_s3outposts.client import S3OutpostsClient


session = Session()
async with session.client("s3outposts") as client:
    client: S3OutpostsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("s3outposts").get_paginator("...")`.

```python
# ListEndpointsPaginator usage example

from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

def get_list_endpoints_paginator() -> ListEndpointsPaginator:
    return client.get_paginator("list_endpoints"))
```

- [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- [ListOutpostsWithS3Paginator](./paginators.md#listoutpostswiths3paginator)
- [ListSharedEndpointsPaginator](./paginators.md#listsharedendpointspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EndpointAccessTypeType usage example

from types_aiobotocore_s3outposts.literals import EndpointAccessTypeType

def get_value() -> EndpointAccessTypeType:
    return "CustomerOwnedIp"
```

- [EndpointAccessTypeType](./literals.md#endpointaccesstypetype)
- [EndpointStatusType](./literals.md#endpointstatustype)
- [ListEndpointsPaginatorName](./literals.md#listendpointspaginatorname)
- [ListOutpostsWithS3PaginatorName](./literals.md#listoutpostswiths3paginatorname)
- [ListSharedEndpointsPaginatorName](./literals.md#listsharedendpointspaginatorname)
- [S3OutpostsServiceName](./literals.md#s3outpostsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef)
- [FailedReasonTypeDef](./type_defs.md#failedreasontypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef)
- [ListOutpostsWithS3RequestRequestTypeDef](./type_defs.md#listoutpostswiths3requestrequesttypedef)
- [OutpostTypeDef](./type_defs.md#outposttypedef)
- [ListSharedEndpointsRequestRequestTypeDef](./type_defs.md#listsharedendpointsrequestrequesttypedef)
- [CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [ListEndpointsRequestPaginateTypeDef](./type_defs.md#listendpointsrequestpaginatetypedef)
- [ListOutpostsWithS3RequestPaginateTypeDef](./type_defs.md#listoutpostswiths3requestpaginatetypedef)
- [ListSharedEndpointsRequestPaginateTypeDef](./type_defs.md#listsharedendpointsrequestpaginatetypedef)
- [ListOutpostsWithS3ResultTypeDef](./type_defs.md#listoutpostswiths3resulttypedef)
- [ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef)
- [ListSharedEndpointsResultTypeDef](./type_defs.md#listsharedendpointsresulttypedef)
