# IoT1ClickProjects module

> [Index](../README.md) > IoT1ClickProjects


!!! note ""

    Auto-generated documentation for [IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#iot1clickprojects)
    type annotations stubs module [types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `IoT1ClickProjects` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `IoT1ClickProjects` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[iot1click-projects]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[iot1click-projects]'

# standalone installation
python -m pip install types-aiobotocore-iot1click-projects
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iot1click-projects
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoT1ClickProjectsClient

Type annotations and code completion for  `#!python session.client("iot1click-projects")` as [IoT1ClickProjectsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client)

```python
# IoT1ClickProjectsClient usage example

from aioboto3.session import Session

from types_aiobotocore_iot1click_projects.client import IoT1ClickProjectsClient


session = Session()
async with session.client("iot1click-projects") as client:
    client: IoT1ClickProjectsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("iot1click-projects").get_paginator("...")`.

```python
# ListPlacementsPaginator usage example

from types_aiobotocore_iot1click_projects.paginator import ListPlacementsPaginator

def get_list_placements_paginator() -> ListPlacementsPaginator:
    return client.get_paginator("list_placements"))
```

- [ListPlacementsPaginator](./paginators.md#listplacementspaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListPlacementsPaginatorName usage example

from types_aiobotocore_iot1click_projects.literals import ListPlacementsPaginatorName

def get_value() -> ListPlacementsPaginatorName:
    return "list_placements"
```

- [ListPlacementsPaginatorName](./literals.md#listplacementspaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [IoT1ClickProjectsServiceName](./literals.md#iot1clickprojectsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateDeviceWithPlacementRequestRequestTypeDef](./type_defs.md#associatedevicewithplacementrequestrequesttypedef)
- [CreatePlacementRequestRequestTypeDef](./type_defs.md#createplacementrequestrequesttypedef)
- [DeletePlacementRequestRequestTypeDef](./type_defs.md#deleteplacementrequestrequesttypedef)
- [DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef)
- [DescribePlacementRequestRequestTypeDef](./type_defs.md#describeplacementrequestrequesttypedef)
- [PlacementDescriptionTypeDef](./type_defs.md#placementdescriptiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef)
- [DeviceTemplateOutputTypeDef](./type_defs.md#devicetemplateoutputtypedef)
- [DeviceTemplateTypeDef](./type_defs.md#devicetemplatetypedef)
- [DisassociateDeviceFromPlacementRequestRequestTypeDef](./type_defs.md#disassociatedevicefromplacementrequestrequesttypedef)
- [GetDevicesInPlacementRequestRequestTypeDef](./type_defs.md#getdevicesinplacementrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListPlacementsRequestRequestTypeDef](./type_defs.md#listplacementsrequestrequesttypedef)
- [PlacementSummaryTypeDef](./type_defs.md#placementsummarytypedef)
- [ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePlacementRequestRequestTypeDef](./type_defs.md#updateplacementrequestrequesttypedef)
- [DescribePlacementResponseTypeDef](./type_defs.md#describeplacementresponsetypedef)
- [GetDevicesInPlacementResponseTypeDef](./type_defs.md#getdevicesinplacementresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PlacementTemplateOutputTypeDef](./type_defs.md#placementtemplateoutputtypedef)
- [DeviceTemplateUnionTypeDef](./type_defs.md#devicetemplateuniontypedef)
- [ListPlacementsRequestPaginateTypeDef](./type_defs.md#listplacementsrequestpaginatetypedef)
- [ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef)
- [ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef)
- [ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)
- [ProjectDescriptionTypeDef](./type_defs.md#projectdescriptiontypedef)
- [PlacementTemplateTypeDef](./type_defs.md#placementtemplatetypedef)
- [DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef)
- [CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef)
- [UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef)
