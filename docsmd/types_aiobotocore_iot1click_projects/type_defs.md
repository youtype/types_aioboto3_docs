# Type definitions

> [Index](../README.md) > [IoT1ClickProjects](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#iot1clickprojects)
    type annotations stubs module [types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

## DeviceTemplateUnionTypeDef

```python
# DeviceTemplateUnionTypeDef definition

DeviceTemplateUnionTypeDef = Union[
    DeviceTemplateTypeDef,  # (1)
    DeviceTemplateOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeviceTemplateTypeDef](./type_defs.md#devicetemplatetypedef) 
2. See [:material-code-braces: DeviceTemplateOutputTypeDef](./type_defs.md#devicetemplateoutputtypedef) 



## AssociateDeviceWithPlacementRequestRequestTypeDef

```python
# AssociateDeviceWithPlacementRequestRequestTypeDef definition

class AssociateDeviceWithPlacementRequestRequestTypeDef(TypedDict):
    projectName: str,
    placementName: str,
    deviceId: str,
    deviceTemplateName: str,
```

## CreatePlacementRequestRequestTypeDef

```python
# CreatePlacementRequestRequestTypeDef definition

class CreatePlacementRequestRequestTypeDef(TypedDict):
    placementName: str,
    projectName: str,
    attributes: NotRequired[Mapping[str, str]],
```

## DeletePlacementRequestRequestTypeDef

```python
# DeletePlacementRequestRequestTypeDef definition

class DeletePlacementRequestRequestTypeDef(TypedDict):
    placementName: str,
    projectName: str,
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    projectName: str,
```

## DescribePlacementRequestRequestTypeDef

```python
# DescribePlacementRequestRequestTypeDef definition

class DescribePlacementRequestRequestTypeDef(TypedDict):
    placementName: str,
    projectName: str,
```

## PlacementDescriptionTypeDef

```python
# PlacementDescriptionTypeDef definition

class PlacementDescriptionTypeDef(TypedDict):
    projectName: str,
    placementName: str,
    attributes: dict[str, str],
    createdDate: datetime,
    updatedDate: datetime,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DescribeProjectRequestRequestTypeDef

```python
# DescribeProjectRequestRequestTypeDef definition

class DescribeProjectRequestRequestTypeDef(TypedDict):
    projectName: str,
```

## DeviceTemplateOutputTypeDef

```python
# DeviceTemplateOutputTypeDef definition

class DeviceTemplateOutputTypeDef(TypedDict):
    deviceType: NotRequired[str],
    callbackOverrides: NotRequired[dict[str, str]],
```

## DeviceTemplateTypeDef

```python
# DeviceTemplateTypeDef definition

class DeviceTemplateTypeDef(TypedDict):
    deviceType: NotRequired[str],
    callbackOverrides: NotRequired[Mapping[str, str]],
```

## DisassociateDeviceFromPlacementRequestRequestTypeDef

```python
# DisassociateDeviceFromPlacementRequestRequestTypeDef definition

class DisassociateDeviceFromPlacementRequestRequestTypeDef(TypedDict):
    projectName: str,
    placementName: str,
    deviceTemplateName: str,
```

## GetDevicesInPlacementRequestRequestTypeDef

```python
# GetDevicesInPlacementRequestRequestTypeDef definition

class GetDevicesInPlacementRequestRequestTypeDef(TypedDict):
    projectName: str,
    placementName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListPlacementsRequestRequestTypeDef

```python
# ListPlacementsRequestRequestTypeDef definition

class ListPlacementsRequestRequestTypeDef(TypedDict):
    projectName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PlacementSummaryTypeDef

```python
# PlacementSummaryTypeDef definition

class PlacementSummaryTypeDef(TypedDict):
    projectName: str,
    placementName: str,
    createdDate: datetime,
    updatedDate: datetime,
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    projectName: str,
    createdDate: datetime,
    updatedDate: datetime,
    arn: NotRequired[str],
    tags: NotRequired[dict[str, str]],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdatePlacementRequestRequestTypeDef

```python
# UpdatePlacementRequestRequestTypeDef definition

class UpdatePlacementRequestRequestTypeDef(TypedDict):
    placementName: str,
    projectName: str,
    attributes: NotRequired[Mapping[str, str]],
```

## DescribePlacementResponseTypeDef

```python
# DescribePlacementResponseTypeDef definition

class DescribePlacementResponseTypeDef(TypedDict):
    placement: PlacementDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlacementDescriptionTypeDef](./type_defs.md#placementdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevicesInPlacementResponseTypeDef

```python
# GetDevicesInPlacementResponseTypeDef definition

class GetDevicesInPlacementResponseTypeDef(TypedDict):
    devices: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PlacementTemplateOutputTypeDef

```python
# PlacementTemplateOutputTypeDef definition

class PlacementTemplateOutputTypeDef(TypedDict):
    defaultAttributes: NotRequired[dict[str, str]],
    deviceTemplates: NotRequired[dict[str, DeviceTemplateOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: DeviceTemplateOutputTypeDef](./type_defs.md#devicetemplateoutputtypedef) 
## ListPlacementsRequestPaginateTypeDef

```python
# ListPlacementsRequestPaginateTypeDef definition

class ListPlacementsRequestPaginateTypeDef(TypedDict):
    projectName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestPaginateTypeDef

```python
# ListProjectsRequestPaginateTypeDef definition

class ListProjectsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlacementsResponseTypeDef

```python
# ListPlacementsResponseTypeDef definition

class ListPlacementsResponseTypeDef(TypedDict):
    placements: list[PlacementSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PlacementSummaryTypeDef](./type_defs.md#placementsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef definition

class ListProjectsResponseTypeDef(TypedDict):
    projects: list[ProjectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectDescriptionTypeDef

```python
# ProjectDescriptionTypeDef definition

class ProjectDescriptionTypeDef(TypedDict):
    projectName: str,
    createdDate: datetime,
    updatedDate: datetime,
    arn: NotRequired[str],
    description: NotRequired[str],
    placementTemplate: NotRequired[PlacementTemplateOutputTypeDef],  # (1)
    tags: NotRequired[dict[str, str]],
```

1. See [:material-code-braces: PlacementTemplateOutputTypeDef](./type_defs.md#placementtemplateoutputtypedef) 
## PlacementTemplateTypeDef

```python
# PlacementTemplateTypeDef definition

class PlacementTemplateTypeDef(TypedDict):
    defaultAttributes: NotRequired[Mapping[str, str]],
    deviceTemplates: NotRequired[Mapping[str, DeviceTemplateUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DeviceTemplateTypeDef](./type_defs.md#devicetemplatetypedef) [:material-code-braces: DeviceTemplateOutputTypeDef](./type_defs.md#devicetemplateoutputtypedef) 
## DescribeProjectResponseTypeDef

```python
# DescribeProjectResponseTypeDef definition

class DescribeProjectResponseTypeDef(TypedDict):
    project: ProjectDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectDescriptionTypeDef](./type_defs.md#projectdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    projectName: str,
    description: NotRequired[str],
    placementTemplate: NotRequired[PlacementTemplateTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: PlacementTemplateTypeDef](./type_defs.md#placementtemplatetypedef) 
## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    projectName: str,
    description: NotRequired[str],
    placementTemplate: NotRequired[PlacementTemplateTypeDef],  # (1)
```

1. See [:material-code-braces: PlacementTemplateTypeDef](./type_defs.md#placementtemplatetypedef) 