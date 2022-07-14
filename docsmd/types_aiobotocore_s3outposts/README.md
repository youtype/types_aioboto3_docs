# S3Outposts module

> [Index](../README.md) > S3Outposts


!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `S3Outposts`.

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

```python title="Usage example"
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

```python title="Usage example"
from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

def get_list_endpoints_paginator() -> ListEndpointsPaginator:
    return client.get_paginator("list_endpoints"))
```

- [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- [ListSharedEndpointsPaginator](./paginators.md#listsharedendpointspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_s3outposts.literals import EndpointAccessTypeType

def get_value() -> EndpointAccessTypeType:
    return "CustomerOwnedIp"
```

- [EndpointAccessTypeType](./literals.md#endpointaccesstypetype)
- [EndpointStatusType](./literals.md#endpointstatustype)
- [ListEndpointsPaginatorName](./literals.md#listendpointspaginatorname)
- [ListSharedEndpointsPaginatorName](./literals.md#listsharedendpointspaginatorname)
- [S3OutpostsServiceName](./literals.md#s3outpostsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_s3outposts.type_defs import CreateEndpointRequestRequestTypeDef

def get_value() -> CreateEndpointRequestRequestTypeDef:
    return {
        "OutpostId": ...,
        "SubnetId": ...,
        "SecurityGroupId": ...,
    }
```

- [CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef)
- [ListSharedEndpointsRequestRequestTypeDef](./type_defs.md#listsharedendpointsrequestrequesttypedef)
- [CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [ListEndpointsRequestListEndpointsPaginateTypeDef](./type_defs.md#listendpointsrequestlistendpointspaginatetypedef)
- [ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef](./type_defs.md#listsharedendpointsrequestlistsharedendpointspaginatetypedef)
- [ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef)
- [ListSharedEndpointsResultTypeDef](./type_defs.md#listsharedendpointsresulttypedef)

