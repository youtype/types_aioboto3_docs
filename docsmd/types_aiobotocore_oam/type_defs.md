# Type definitions

> [Index](../README.md) > [CloudWatchObservabilityAccessManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAccessManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#cloudwatchobservabilityaccessmanager)
    type annotations stubs module [types-aiobotocore-oam](https://pypi.org/project/types-aiobotocore-oam/).



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

## CreateSinkInputRequestTypeDef

```python
# CreateSinkInputRequestTypeDef definition

class CreateSinkInputRequestTypeDef(TypedDict):
    Name: str,
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteLinkInputRequestTypeDef

```python
# DeleteLinkInputRequestTypeDef definition

class DeleteLinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## DeleteSinkInputRequestTypeDef

```python
# DeleteSinkInputRequestTypeDef definition

class DeleteSinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetLinkInputRequestTypeDef

```python
# GetLinkInputRequestTypeDef definition

class GetLinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetSinkInputRequestTypeDef

```python
# GetSinkInputRequestTypeDef definition

class GetSinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetSinkPolicyInputRequestTypeDef

```python
# GetSinkPolicyInputRequestTypeDef definition

class GetSinkPolicyInputRequestTypeDef(TypedDict):
    SinkIdentifier: str,
```

## LogGroupConfigurationTypeDef

```python
# LogGroupConfigurationTypeDef definition

class LogGroupConfigurationTypeDef(TypedDict):
    Filter: str,
```

## MetricConfigurationTypeDef

```python
# MetricConfigurationTypeDef definition

class MetricConfigurationTypeDef(TypedDict):
    Filter: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAttachedLinksInputRequestTypeDef

```python
# ListAttachedLinksInputRequestTypeDef definition

class ListAttachedLinksInputRequestTypeDef(TypedDict):
    SinkIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAttachedLinksItemTypeDef

```python
# ListAttachedLinksItemTypeDef definition

class ListAttachedLinksItemTypeDef(TypedDict):
    Label: NotRequired[str],
    LinkArn: NotRequired[str],
    ResourceTypes: NotRequired[list[str]],
```

## ListLinksInputRequestTypeDef

```python
# ListLinksInputRequestTypeDef definition

class ListLinksInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLinksItemTypeDef

```python
# ListLinksItemTypeDef definition

class ListLinksItemTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Label: NotRequired[str],
    ResourceTypes: NotRequired[list[str]],
    SinkArn: NotRequired[str],
```

## ListSinksInputRequestTypeDef

```python
# ListSinksInputRequestTypeDef definition

class ListSinksInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSinksItemTypeDef

```python
# ListSinksItemTypeDef definition

class ListSinksItemTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PutSinkPolicyInputRequestTypeDef

```python
# PutSinkPolicyInputRequestTypeDef definition

class PutSinkPolicyInputRequestTypeDef(TypedDict):
    Policy: str,
    SinkIdentifier: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CreateSinkOutputTypeDef

```python
# CreateSinkOutputTypeDef definition

class CreateSinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSinkOutputTypeDef

```python
# GetSinkOutputTypeDef definition

class GetSinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSinkPolicyOutputTypeDef

```python
# GetSinkPolicyOutputTypeDef definition

class GetSinkPolicyOutputTypeDef(TypedDict):
    Policy: str,
    SinkArn: str,
    SinkId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
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
## PutSinkPolicyOutputTypeDef

```python
# PutSinkPolicyOutputTypeDef definition

class PutSinkPolicyOutputTypeDef(TypedDict):
    Policy: str,
    SinkArn: str,
    SinkId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LinkConfigurationTypeDef

```python
# LinkConfigurationTypeDef definition

class LinkConfigurationTypeDef(TypedDict):
    LogGroupConfiguration: NotRequired[LogGroupConfigurationTypeDef],  # (1)
    MetricConfiguration: NotRequired[MetricConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: LogGroupConfigurationTypeDef](./type_defs.md#loggroupconfigurationtypedef) 
2. See [:material-code-braces: MetricConfigurationTypeDef](./type_defs.md#metricconfigurationtypedef) 
## ListAttachedLinksInputPaginateTypeDef

```python
# ListAttachedLinksInputPaginateTypeDef definition

class ListAttachedLinksInputPaginateTypeDef(TypedDict):
    SinkIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLinksInputPaginateTypeDef

```python
# ListLinksInputPaginateTypeDef definition

class ListLinksInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSinksInputPaginateTypeDef

```python
# ListSinksInputPaginateTypeDef definition

class ListSinksInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedLinksOutputTypeDef

```python
# ListAttachedLinksOutputTypeDef definition

class ListAttachedLinksOutputTypeDef(TypedDict):
    Items: list[ListAttachedLinksItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListAttachedLinksItemTypeDef](./type_defs.md#listattachedlinksitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLinksOutputTypeDef

```python
# ListLinksOutputTypeDef definition

class ListLinksOutputTypeDef(TypedDict):
    Items: list[ListLinksItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListLinksItemTypeDef](./type_defs.md#listlinksitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSinksOutputTypeDef

```python
# ListSinksOutputTypeDef definition

class ListSinksOutputTypeDef(TypedDict):
    Items: list[ListSinksItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListSinksItemTypeDef](./type_defs.md#listsinksitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLinkInputRequestTypeDef

```python
# CreateLinkInputRequestTypeDef definition

class CreateLinkInputRequestTypeDef(TypedDict):
    LabelTemplate: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
    SinkIdentifier: str,
    LinkConfiguration: NotRequired[LinkConfigurationTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef) 
## CreateLinkOutputTypeDef

```python
# CreateLinkOutputTypeDef definition

class CreateLinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Label: str,
    LabelTemplate: str,
    LinkConfiguration: LinkConfigurationTypeDef,  # (1)
    ResourceTypes: list[str],
    SinkArn: str,
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLinkOutputTypeDef

```python
# GetLinkOutputTypeDef definition

class GetLinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Label: str,
    LabelTemplate: str,
    LinkConfiguration: LinkConfigurationTypeDef,  # (1)
    ResourceTypes: list[str],
    SinkArn: str,
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLinkInputRequestTypeDef

```python
# UpdateLinkInputRequestTypeDef definition

class UpdateLinkInputRequestTypeDef(TypedDict):
    Identifier: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
    LinkConfiguration: NotRequired[LinkConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef) 
## UpdateLinkOutputTypeDef

```python
# UpdateLinkOutputTypeDef definition

class UpdateLinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Label: str,
    LabelTemplate: str,
    LinkConfiguration: LinkConfigurationTypeDef,  # (1)
    ResourceTypes: list[str],
    SinkArn: str,
    Tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LinkConfigurationTypeDef](./type_defs.md#linkconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 