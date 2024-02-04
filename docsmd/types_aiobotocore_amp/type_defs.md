# Type definitions

> [Index](../README.md) > [PrometheusService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## AlertManagerDefinitionStatusTypeDef

```python
# AlertManagerDefinitionStatusTypeDef definition

class AlertManagerDefinitionStatusTypeDef(TypedDict):
    statusCode: AlertManagerDefinitionStatusCodeType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: AlertManagerDefinitionStatusCodeType](./literals.md#alertmanagerdefinitionstatuscodetype) 
## AmpConfigurationTypeDef

```python
# AmpConfigurationTypeDef definition

class AmpConfigurationTypeDef(TypedDict):
    workspaceArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CreateLoggingConfigurationRequestRequestTypeDef

```python
# CreateLoggingConfigurationRequestRequestTypeDef definition

class CreateLoggingConfigurationRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    logGroupArn: str,
    clientToken: NotRequired[str],
```

## LoggingConfigurationStatusTypeDef

```python
# LoggingConfigurationStatusTypeDef definition

class LoggingConfigurationStatusTypeDef(TypedDict):
    statusCode: LoggingConfigurationStatusCodeType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: LoggingConfigurationStatusCodeType](./literals.md#loggingconfigurationstatuscodetype) 
## RuleGroupsNamespaceStatusTypeDef

```python
# RuleGroupsNamespaceStatusTypeDef definition

class RuleGroupsNamespaceStatusTypeDef(TypedDict):
    statusCode: RuleGroupsNamespaceStatusCodeType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: RuleGroupsNamespaceStatusCodeType](./literals.md#rulegroupsnamespacestatuscodetype) 
## ScraperStatusTypeDef

```python
# ScraperStatusTypeDef definition

class ScraperStatusTypeDef(TypedDict):
    statusCode: ScraperStatusCodeType,  # (1)
```

1. See [:material-code-brackets: ScraperStatusCodeType](./literals.md#scraperstatuscodetype) 
## CreateWorkspaceRequestRequestTypeDef

```python
# CreateWorkspaceRequestRequestTypeDef definition

class CreateWorkspaceRequestRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
```

## WorkspaceStatusTypeDef

```python
# WorkspaceStatusTypeDef definition

class WorkspaceStatusTypeDef(TypedDict):
    statusCode: WorkspaceStatusCodeType,  # (1)
```

1. See [:material-code-brackets: WorkspaceStatusCodeType](./literals.md#workspacestatuscodetype) 
## DeleteAlertManagerDefinitionRequestRequestTypeDef

```python
# DeleteAlertManagerDefinitionRequestRequestTypeDef definition

class DeleteAlertManagerDefinitionRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DeleteLoggingConfigurationRequestRequestTypeDef

```python
# DeleteLoggingConfigurationRequestRequestTypeDef definition

class DeleteLoggingConfigurationRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DeleteRuleGroupsNamespaceRequestRequestTypeDef

```python
# DeleteRuleGroupsNamespaceRequestRequestTypeDef definition

class DeleteRuleGroupsNamespaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    name: str,
    clientToken: NotRequired[str],
```

## DeleteScraperRequestRequestTypeDef

```python
# DeleteScraperRequestRequestTypeDef definition

class DeleteScraperRequestRequestTypeDef(TypedDict):
    scraperId: str,
    clientToken: NotRequired[str],
```

## DeleteWorkspaceRequestRequestTypeDef

```python
# DeleteWorkspaceRequestRequestTypeDef definition

class DeleteWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DescribeAlertManagerDefinitionRequestRequestTypeDef

```python
# DescribeAlertManagerDefinitionRequestRequestTypeDef definition

class DescribeAlertManagerDefinitionRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeLoggingConfigurationRequestRequestTypeDef

```python
# DescribeLoggingConfigurationRequestRequestTypeDef definition

class DescribeLoggingConfigurationRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeRuleGroupsNamespaceRequestRequestTypeDef

```python
# DescribeRuleGroupsNamespaceRequestRequestTypeDef definition

class DescribeRuleGroupsNamespaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    name: str,
```

## DescribeScraperRequestRequestTypeDef

```python
# DescribeScraperRequestRequestTypeDef definition

class DescribeScraperRequestRequestTypeDef(TypedDict):
    scraperId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeWorkspaceRequestRequestTypeDef

```python
# DescribeWorkspaceRequestRequestTypeDef definition

class DescribeWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## EksConfigurationPaginatorTypeDef

```python
# EksConfigurationPaginatorTypeDef definition

class EksConfigurationPaginatorTypeDef(TypedDict):
    clusterArn: str,
    subnetIds: List[str],
    securityGroupIds: NotRequired[List[str]],
```

## EksConfigurationTypeDef

```python
# EksConfigurationTypeDef definition

class EksConfigurationTypeDef(TypedDict):
    clusterArn: str,
    subnetIds: Sequence[str],
    securityGroupIds: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRuleGroupsNamespacesRequestRequestTypeDef

```python
# ListRuleGroupsNamespacesRequestRequestTypeDef definition

class ListRuleGroupsNamespacesRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListScrapersRequestRequestTypeDef

```python
# ListScrapersRequestRequestTypeDef definition

class ListScrapersRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Mapping[str, Sequence[str]]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorkspacesRequestRequestTypeDef

```python
# ListWorkspacesRequestRequestTypeDef definition

class ListWorkspacesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    alias: NotRequired[str],
    maxResults: NotRequired[int],
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

## UpdateLoggingConfigurationRequestRequestTypeDef

```python
# UpdateLoggingConfigurationRequestRequestTypeDef definition

class UpdateLoggingConfigurationRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    logGroupArn: str,
    clientToken: NotRequired[str],
```

## UpdateWorkspaceAliasRequestRequestTypeDef

```python
# UpdateWorkspaceAliasRequestRequestTypeDef definition

class UpdateWorkspaceAliasRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    alias: NotRequired[str],
    clientToken: NotRequired[str],
```

## AlertManagerDefinitionDescriptionTypeDef

```python
# AlertManagerDefinitionDescriptionTypeDef definition

class AlertManagerDefinitionDescriptionTypeDef(TypedDict):
    status: AlertManagerDefinitionStatusTypeDef,  # (1)
    data: bytes,
    createdAt: datetime,
    modifiedAt: datetime,
```

1. See [:material-code-braces: AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    ampConfiguration: NotRequired[AmpConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AmpConfigurationTypeDef](./type_defs.md#ampconfigurationtypedef) 
## CreateAlertManagerDefinitionRequestRequestTypeDef

```python
# CreateAlertManagerDefinitionRequestRequestTypeDef definition

class CreateAlertManagerDefinitionRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    data: Union[str, bytes, IO[Any], StreamingBody],
    clientToken: NotRequired[str],
```

## CreateRuleGroupsNamespaceRequestRequestTypeDef

```python
# CreateRuleGroupsNamespaceRequestRequestTypeDef definition

class CreateRuleGroupsNamespaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    name: str,
    data: Union[str, bytes, IO[Any], StreamingBody],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## PutAlertManagerDefinitionRequestRequestTypeDef

```python
# PutAlertManagerDefinitionRequestRequestTypeDef definition

class PutAlertManagerDefinitionRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    data: Union[str, bytes, IO[Any], StreamingBody],
    clientToken: NotRequired[str],
```

## PutRuleGroupsNamespaceRequestRequestTypeDef

```python
# PutRuleGroupsNamespaceRequestRequestTypeDef definition

class PutRuleGroupsNamespaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    name: str,
    data: Union[str, bytes, IO[Any], StreamingBody],
    clientToken: NotRequired[str],
```

## ScrapeConfigurationTypeDef

```python
# ScrapeConfigurationTypeDef definition

class ScrapeConfigurationTypeDef(TypedDict):
    configurationBlob: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
```

## CreateAlertManagerDefinitionResponseTypeDef

```python
# CreateAlertManagerDefinitionResponseTypeDef definition

class CreateAlertManagerDefinitionResponseTypeDef(TypedDict):
    status: AlertManagerDefinitionStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDefaultScraperConfigurationResponseTypeDef

```python
# GetDefaultScraperConfigurationResponseTypeDef definition

class GetDefaultScraperConfigurationResponseTypeDef(TypedDict):
    configuration: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAlertManagerDefinitionResponseTypeDef

```python
# PutAlertManagerDefinitionResponseTypeDef definition

class PutAlertManagerDefinitionResponseTypeDef(TypedDict):
    status: AlertManagerDefinitionStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggingConfigurationResponseTypeDef

```python
# CreateLoggingConfigurationResponseTypeDef definition

class CreateLoggingConfigurationResponseTypeDef(TypedDict):
    status: LoggingConfigurationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingConfigurationMetadataTypeDef

```python
# LoggingConfigurationMetadataTypeDef definition

class LoggingConfigurationMetadataTypeDef(TypedDict):
    status: LoggingConfigurationStatusTypeDef,  # (1)
    workspace: str,
    logGroupArn: str,
    createdAt: datetime,
    modifiedAt: datetime,
```

1. See [:material-code-braces: LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef) 
## UpdateLoggingConfigurationResponseTypeDef

```python
# UpdateLoggingConfigurationResponseTypeDef definition

class UpdateLoggingConfigurationResponseTypeDef(TypedDict):
    status: LoggingConfigurationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleGroupsNamespaceResponseTypeDef

```python
# CreateRuleGroupsNamespaceResponseTypeDef definition

class CreateRuleGroupsNamespaceResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRuleGroupsNamespaceResponseTypeDef

```python
# PutRuleGroupsNamespaceResponseTypeDef definition

class PutRuleGroupsNamespaceResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleGroupsNamespaceDescriptionTypeDef

```python
# RuleGroupsNamespaceDescriptionTypeDef definition

class RuleGroupsNamespaceDescriptionTypeDef(TypedDict):
    arn: str,
    name: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    data: bytes,
    createdAt: datetime,
    modifiedAt: datetime,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
## RuleGroupsNamespaceSummaryTypeDef

```python
# RuleGroupsNamespaceSummaryTypeDef definition

class RuleGroupsNamespaceSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    createdAt: datetime,
    modifiedAt: datetime,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
## CreateScraperResponseTypeDef

```python
# CreateScraperResponseTypeDef definition

class CreateScraperResponseTypeDef(TypedDict):
    scraperId: str,
    arn: str,
    status: ScraperStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteScraperResponseTypeDef

```python
# DeleteScraperResponseTypeDef definition

class DeleteScraperResponseTypeDef(TypedDict):
    scraperId: str,
    status: ScraperStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceResponseTypeDef

```python
# CreateWorkspaceResponseTypeDef definition

class CreateWorkspaceResponseTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    status: WorkspaceStatusTypeDef,  # (1)
    tags: Dict[str, str],
    kmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkspaceDescriptionTypeDef

```python
# WorkspaceDescriptionTypeDef definition

class WorkspaceDescriptionTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    status: WorkspaceStatusTypeDef,  # (1)
    createdAt: datetime,
    alias: NotRequired[str],
    prometheusEndpoint: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef) 
## WorkspaceSummaryTypeDef

```python
# WorkspaceSummaryTypeDef definition

class WorkspaceSummaryTypeDef(TypedDict):
    workspaceId: str,
    arn: str,
    status: WorkspaceStatusTypeDef,  # (1)
    createdAt: datetime,
    alias: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef) 
## DescribeScraperRequestScraperActiveWaitTypeDef

```python
# DescribeScraperRequestScraperActiveWaitTypeDef definition

class DescribeScraperRequestScraperActiveWaitTypeDef(TypedDict):
    scraperId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeScraperRequestScraperDeletedWaitTypeDef

```python
# DescribeScraperRequestScraperDeletedWaitTypeDef definition

class DescribeScraperRequestScraperDeletedWaitTypeDef(TypedDict):
    scraperId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef

```python
# DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef definition

class DescribeWorkspaceRequestWorkspaceActiveWaitTypeDef(TypedDict):
    workspaceId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef

```python
# DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef definition

class DescribeWorkspaceRequestWorkspaceDeletedWaitTypeDef(TypedDict):
    workspaceId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## SourcePaginatorTypeDef

```python
# SourcePaginatorTypeDef definition

class SourcePaginatorTypeDef(TypedDict):
    eksConfiguration: NotRequired[EksConfigurationPaginatorTypeDef],  # (1)
```

1. See [:material-code-braces: EksConfigurationPaginatorTypeDef](./type_defs.md#eksconfigurationpaginatortypedef) 
## SourceTypeDef

```python
# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    eksConfiguration: NotRequired[EksConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef) 
## ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef

```python
# ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef definition

class ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef(TypedDict):
    workspaceId: str,
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScrapersRequestListScrapersPaginateTypeDef

```python
# ListScrapersRequestListScrapersPaginateTypeDef definition

class ListScrapersRequestListScrapersPaginateTypeDef(TypedDict):
    filters: NotRequired[Mapping[str, Sequence[str]]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspacesRequestListWorkspacesPaginateTypeDef

```python
# ListWorkspacesRequestListWorkspacesPaginateTypeDef definition

class ListWorkspacesRequestListWorkspacesPaginateTypeDef(TypedDict):
    alias: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAlertManagerDefinitionResponseTypeDef

```python
# DescribeAlertManagerDefinitionResponseTypeDef definition

class DescribeAlertManagerDefinitionResponseTypeDef(TypedDict):
    alertManagerDefinition: AlertManagerDefinitionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertManagerDefinitionDescriptionTypeDef](./type_defs.md#alertmanagerdefinitiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoggingConfigurationResponseTypeDef

```python
# DescribeLoggingConfigurationResponseTypeDef definition

class DescribeLoggingConfigurationResponseTypeDef(TypedDict):
    loggingConfiguration: LoggingConfigurationMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationMetadataTypeDef](./type_defs.md#loggingconfigurationmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRuleGroupsNamespaceResponseTypeDef

```python
# DescribeRuleGroupsNamespaceResponseTypeDef definition

class DescribeRuleGroupsNamespaceResponseTypeDef(TypedDict):
    ruleGroupsNamespace: RuleGroupsNamespaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceDescriptionTypeDef](./type_defs.md#rulegroupsnamespacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleGroupsNamespacesResponseTypeDef

```python
# ListRuleGroupsNamespacesResponseTypeDef definition

class ListRuleGroupsNamespacesResponseTypeDef(TypedDict):
    ruleGroupsNamespaces: List[RuleGroupsNamespaceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceSummaryTypeDef](./type_defs.md#rulegroupsnamespacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceResponseTypeDef

```python
# DescribeWorkspaceResponseTypeDef definition

class DescribeWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkspacesResponseTypeDef

```python
# ListWorkspacesResponseTypeDef definition

class ListWorkspacesResponseTypeDef(TypedDict):
    workspaces: List[WorkspaceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScraperSummaryPaginatorTypeDef

```python
# ScraperSummaryPaginatorTypeDef definition

class ScraperSummaryPaginatorTypeDef(TypedDict):
    scraperId: str,
    arn: str,
    roleArn: str,
    status: ScraperStatusTypeDef,  # (1)
    createdAt: datetime,
    lastModifiedAt: datetime,
    source: SourcePaginatorTypeDef,  # (2)
    destination: DestinationTypeDef,  # (3)
    alias: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: SourcePaginatorTypeDef](./type_defs.md#sourcepaginatortypedef) 
3. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## CreateScraperRequestRequestTypeDef

```python
# CreateScraperRequestRequestTypeDef definition

class CreateScraperRequestRequestTypeDef(TypedDict):
    scrapeConfiguration: ScrapeConfigurationTypeDef,  # (1)
    source: SourceTypeDef,  # (2)
    destination: DestinationTypeDef,  # (3)
    alias: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
3. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## ScraperDescriptionTypeDef

```python
# ScraperDescriptionTypeDef definition

class ScraperDescriptionTypeDef(TypedDict):
    scraperId: str,
    arn: str,
    roleArn: str,
    status: ScraperStatusTypeDef,  # (1)
    createdAt: datetime,
    lastModifiedAt: datetime,
    scrapeConfiguration: ScrapeConfigurationTypeDef,  # (2)
    source: SourceTypeDef,  # (3)
    destination: DestinationTypeDef,  # (4)
    alias: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## ScraperSummaryTypeDef

```python
# ScraperSummaryTypeDef definition

class ScraperSummaryTypeDef(TypedDict):
    scraperId: str,
    arn: str,
    roleArn: str,
    status: ScraperStatusTypeDef,  # (1)
    createdAt: datetime,
    lastModifiedAt: datetime,
    source: SourceTypeDef,  # (2)
    destination: DestinationTypeDef,  # (3)
    alias: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
3. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## ListScrapersResponsePaginatorTypeDef

```python
# ListScrapersResponsePaginatorTypeDef definition

class ListScrapersResponsePaginatorTypeDef(TypedDict):
    scrapers: List[ScraperSummaryPaginatorTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperSummaryPaginatorTypeDef](./type_defs.md#scrapersummarypaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScraperResponseTypeDef

```python
# DescribeScraperResponseTypeDef definition

class DescribeScraperResponseTypeDef(TypedDict):
    scraper: ScraperDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperDescriptionTypeDef](./type_defs.md#scraperdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScrapersResponseTypeDef

```python
# ListScrapersResponseTypeDef definition

class ListScrapersResponseTypeDef(TypedDict):
    scrapers: List[ScraperSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperSummaryTypeDef](./type_defs.md#scrapersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
