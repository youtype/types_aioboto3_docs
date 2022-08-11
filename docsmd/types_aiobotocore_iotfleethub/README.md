# IoTFleetHub module

> [Index](../README.md) > IoTFleetHub


!!! note ""

    Auto-generated documentation for [IoTFleetHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
    type annotations stubs module [types-aiobotocore-iotfleethub](https://pypi.org/project/types-aiobotocore-iotfleethub/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `IoTFleetHub` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[iotfleethub]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[iotfleethub]'


# standalone installation
python -m pip install types-aiobotocore-iotfleethub
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotfleethub
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTFleetHubClient

Type annotations and code completion for  `#!python session.client("iotfleethub")` as [IoTFleetHubClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotfleethub.client import IoTFleetHubClient


session = Session()
async with session.client("iotfleethub") as client:
    client: IoTFleetHubClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("iotfleethub").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_iotfleethub.paginator import ListApplicationsPaginator

def get_list_applications_paginator() -> ListApplicationsPaginator:
    return client.get_paginator("list_applications"))
```

- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotfleethub.literals import ApplicationStateType

def get_value() -> ApplicationStateType:
    return "ACTIVE"
```

- [ApplicationStateType](./literals.md#applicationstatetype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [IoTFleetHubServiceName](./literals.md#iotfleethubservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotfleethub.type_defs import ApplicationSummaryTypeDef

def get_value() -> ApplicationSummaryTypeDef:
    return {
        "applicationId": ...,
        "applicationName": ...,
        "applicationUrl": ...,
    }
```

- [ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [DescribeApplicationRequestRequestTypeDef](./type_defs.md#describeapplicationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [DescribeApplicationResponseTypeDef](./type_defs.md#describeapplicationresponsetypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef)

