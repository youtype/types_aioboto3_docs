# Type definitions

> [Index](../README.md) > [ResourceExplorer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).



## AssociateDefaultViewInputRequestTypeDef

```python
# AssociateDefaultViewInputRequestTypeDef definition

class AssociateDefaultViewInputRequestTypeDef(TypedDict):
    ViewArn: str,
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

## BatchGetViewErrorTypeDef

```python
# BatchGetViewErrorTypeDef definition

class BatchGetViewErrorTypeDef(TypedDict):
    ErrorMessage: str,
    ViewArn: str,
```

## BatchGetViewInputRequestTypeDef

```python
# BatchGetViewInputRequestTypeDef definition

class BatchGetViewInputRequestTypeDef(TypedDict):
    ViewArns: NotRequired[Sequence[str]],
```

## CreateIndexInputRequestTypeDef

```python
# CreateIndexInputRequestTypeDef definition

class CreateIndexInputRequestTypeDef(TypedDict):
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## IncludedPropertyTypeDef

```python
# IncludedPropertyTypeDef definition

class IncludedPropertyTypeDef(TypedDict):
    Name: str,
```

## SearchFilterTypeDef

```python
# SearchFilterTypeDef definition

class SearchFilterTypeDef(TypedDict):
    FilterString: str,
```

## DeleteIndexInputRequestTypeDef

```python
# DeleteIndexInputRequestTypeDef definition

class DeleteIndexInputRequestTypeDef(TypedDict):
    Arn: str,
```

## DeleteViewInputRequestTypeDef

```python
# DeleteViewInputRequestTypeDef definition

class DeleteViewInputRequestTypeDef(TypedDict):
    ViewArn: str,
```

## OrgConfigurationTypeDef

```python
# OrgConfigurationTypeDef definition

class OrgConfigurationTypeDef(TypedDict):
    AWSServiceAccessStatus: AWSServiceAccessStatusType,  # (1)
    ServiceLinkedRole: NotRequired[str],
```

1. See [:material-code-brackets: AWSServiceAccessStatusType](./literals.md#awsserviceaccessstatustype) 
## GetManagedViewInputRequestTypeDef

```python
# GetManagedViewInputRequestTypeDef definition

class GetManagedViewInputRequestTypeDef(TypedDict):
    ManagedViewArn: str,
```

## GetViewInputRequestTypeDef

```python
# GetViewInputRequestTypeDef definition

class GetViewInputRequestTypeDef(TypedDict):
    ViewArn: str,
```

## IndexTypeDef

```python
# IndexTypeDef definition

class IndexTypeDef(TypedDict):
    Arn: NotRequired[str],
    Region: NotRequired[str],
    Type: NotRequired[IndexTypeType],  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIndexesForMembersInputRequestTypeDef

```python
# ListIndexesForMembersInputRequestTypeDef definition

class ListIndexesForMembersInputRequestTypeDef(TypedDict):
    AccountIdList: Sequence[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MemberIndexTypeDef

```python
# MemberIndexTypeDef definition

class MemberIndexTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Arn: NotRequired[str],
    Region: NotRequired[str],
    Type: NotRequired[IndexTypeType],  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## ListIndexesInputRequestTypeDef

```python
# ListIndexesInputRequestTypeDef definition

class ListIndexesInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Regions: NotRequired[Sequence[str]],
    Type: NotRequired[IndexTypeType],  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## ListManagedViewsInputRequestTypeDef

```python
# ListManagedViewsInputRequestTypeDef definition

class ListManagedViewsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ServicePrincipal: NotRequired[str],
```

## ListSupportedResourceTypesInputRequestTypeDef

```python
# ListSupportedResourceTypesInputRequestTypeDef definition

class ListSupportedResourceTypesInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SupportedResourceTypeTypeDef

```python
# SupportedResourceTypeTypeDef definition

class SupportedResourceTypeTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    Service: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListViewsInputRequestTypeDef

```python
# ListViewsInputRequestTypeDef definition

class ListViewsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ResourceCountTypeDef

```python
# ResourceCountTypeDef definition

class ResourceCountTypeDef(TypedDict):
    Complete: NotRequired[bool],
    TotalResources: NotRequired[int],
```

## ResourcePropertyTypeDef

```python
# ResourcePropertyTypeDef definition

class ResourcePropertyTypeDef(TypedDict):
    Data: NotRequired[dict[str, Any]],
    LastReportedAt: NotRequired[datetime],
    Name: NotRequired[str],
```

## SearchInputRequestTypeDef

```python
# SearchInputRequestTypeDef definition

class SearchInputRequestTypeDef(TypedDict):
    QueryString: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ViewArn: NotRequired[str],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateIndexTypeInputRequestTypeDef

```python
# UpdateIndexTypeInputRequestTypeDef definition

class UpdateIndexTypeInputRequestTypeDef(TypedDict):
    Arn: str,
    Type: IndexTypeType,  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## AssociateDefaultViewOutputTypeDef

```python
# AssociateDefaultViewOutputTypeDef definition

class AssociateDefaultViewOutputTypeDef(TypedDict):
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIndexOutputTypeDef

```python
# CreateIndexOutputTypeDef definition

class CreateIndexOutputTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    State: IndexStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIndexOutputTypeDef

```python
# DeleteIndexOutputTypeDef definition

class DeleteIndexOutputTypeDef(TypedDict):
    Arn: str,
    LastUpdatedAt: datetime,
    State: IndexStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteViewOutputTypeDef

```python
# DeleteViewOutputTypeDef definition

class DeleteViewOutputTypeDef(TypedDict):
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDefaultViewOutputTypeDef

```python
# GetDefaultViewOutputTypeDef definition

class GetDefaultViewOutputTypeDef(TypedDict):
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIndexOutputTypeDef

```python
# GetIndexOutputTypeDef definition

class GetIndexOutputTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    ReplicatingFrom: list[str],
    ReplicatingTo: list[str],
    State: IndexStateType,  # (1)
    Tags: dict[str, str],
    Type: IndexTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedViewsOutputTypeDef

```python
# ListManagedViewsOutputTypeDef definition

class ListManagedViewsOutputTypeDef(TypedDict):
    ManagedViews: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViewsOutputTypeDef

```python
# ListViewsOutputTypeDef definition

class ListViewsOutputTypeDef(TypedDict):
    Views: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIndexTypeOutputTypeDef

```python
# UpdateIndexTypeOutputTypeDef definition

class UpdateIndexTypeOutputTypeDef(TypedDict):
    Arn: str,
    LastUpdatedAt: datetime,
    State: IndexStateType,  # (1)
    Type: IndexTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewInputRequestTypeDef

```python
# CreateViewInputRequestTypeDef definition

class CreateViewInputRequestTypeDef(TypedDict):
    ViewName: str,
    ClientToken: NotRequired[str],
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[Sequence[IncludedPropertyTypeDef]],  # (2)
    Scope: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## ListResourcesInputRequestTypeDef

```python
# ListResourcesInputRequestTypeDef definition

class ListResourcesInputRequestTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ViewArn: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
## ManagedViewTypeDef

```python
# ManagedViewTypeDef definition

class ManagedViewTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[list[IncludedPropertyTypeDef]],  # (2)
    LastUpdatedAt: NotRequired[datetime],
    ManagedViewArn: NotRequired[str],
    ManagedViewName: NotRequired[str],
    Owner: NotRequired[str],
    ResourcePolicy: NotRequired[str],
    Scope: NotRequired[str],
    TrustedService: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## UpdateViewInputRequestTypeDef

```python
# UpdateViewInputRequestTypeDef definition

class UpdateViewInputRequestTypeDef(TypedDict):
    ViewArn: str,
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[Sequence[IncludedPropertyTypeDef]],  # (2)
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## ViewTypeDef

```python
# ViewTypeDef definition

class ViewTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[list[IncludedPropertyTypeDef]],  # (2)
    LastUpdatedAt: NotRequired[datetime],
    Owner: NotRequired[str],
    Scope: NotRequired[str],
    ViewArn: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## GetAccountLevelServiceConfigurationOutputTypeDef

```python
# GetAccountLevelServiceConfigurationOutputTypeDef definition

class GetAccountLevelServiceConfigurationOutputTypeDef(TypedDict):
    OrgConfiguration: OrgConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrgConfigurationTypeDef](./type_defs.md#orgconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndexesOutputTypeDef

```python
# ListIndexesOutputTypeDef definition

class ListIndexesOutputTypeDef(TypedDict):
    Indexes: list[IndexTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexTypeDef](./type_defs.md#indextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndexesForMembersInputPaginateTypeDef

```python
# ListIndexesForMembersInputPaginateTypeDef definition

class ListIndexesForMembersInputPaginateTypeDef(TypedDict):
    AccountIdList: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndexesInputPaginateTypeDef

```python
# ListIndexesInputPaginateTypeDef definition

class ListIndexesInputPaginateTypeDef(TypedDict):
    Regions: NotRequired[Sequence[str]],
    Type: NotRequired[IndexTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedViewsInputPaginateTypeDef

```python
# ListManagedViewsInputPaginateTypeDef definition

class ListManagedViewsInputPaginateTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesInputPaginateTypeDef

```python
# ListResourcesInputPaginateTypeDef definition

class ListResourcesInputPaginateTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    ViewArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSupportedResourceTypesInputPaginateTypeDef

```python
# ListSupportedResourceTypesInputPaginateTypeDef definition

class ListSupportedResourceTypesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViewsInputPaginateTypeDef

```python
# ListViewsInputPaginateTypeDef definition

class ListViewsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchInputPaginateTypeDef

```python
# SearchInputPaginateTypeDef definition

class SearchInputPaginateTypeDef(TypedDict):
    QueryString: str,
    ViewArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndexesForMembersOutputTypeDef

```python
# ListIndexesForMembersOutputTypeDef definition

class ListIndexesForMembersOutputTypeDef(TypedDict):
    Indexes: list[MemberIndexTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberIndexTypeDef](./type_defs.md#memberindextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSupportedResourceTypesOutputTypeDef

```python
# ListSupportedResourceTypesOutputTypeDef definition

class ListSupportedResourceTypesOutputTypeDef(TypedDict):
    ResourceTypes: list[SupportedResourceTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SupportedResourceTypeTypeDef](./type_defs.md#supportedresourcetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    Arn: NotRequired[str],
    LastReportedAt: NotRequired[datetime],
    OwningAccountId: NotRequired[str],
    Properties: NotRequired[list[ResourcePropertyTypeDef]],  # (1)
    Region: NotRequired[str],
    ResourceType: NotRequired[str],
    Service: NotRequired[str],
```

1. See [:material-code-braces: ResourcePropertyTypeDef](./type_defs.md#resourcepropertytypedef) 
## GetManagedViewOutputTypeDef

```python
# GetManagedViewOutputTypeDef definition

class GetManagedViewOutputTypeDef(TypedDict):
    ManagedView: ManagedViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedViewTypeDef](./type_defs.md#managedviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetViewOutputTypeDef

```python
# BatchGetViewOutputTypeDef definition

class BatchGetViewOutputTypeDef(TypedDict):
    Errors: list[BatchGetViewErrorTypeDef],  # (1)
    Views: list[ViewTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetViewErrorTypeDef](./type_defs.md#batchgetviewerrortypedef) 
2. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewOutputTypeDef

```python
# CreateViewOutputTypeDef definition

class CreateViewOutputTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetViewOutputTypeDef

```python
# GetViewOutputTypeDef definition

class GetViewOutputTypeDef(TypedDict):
    Tags: dict[str, str],
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateViewOutputTypeDef

```python
# UpdateViewOutputTypeDef definition

class UpdateViewOutputTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesOutputTypeDef

```python
# ListResourcesOutputTypeDef definition

class ListResourcesOutputTypeDef(TypedDict):
    Resources: list[ResourceTypeDef],  # (1)
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchOutputTypeDef

```python
# SearchOutputTypeDef definition

class SearchOutputTypeDef(TypedDict):
    Count: ResourceCountTypeDef,  # (1)
    Resources: list[ResourceTypeDef],  # (2)
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceCountTypeDef](./type_defs.md#resourcecounttypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 