# Type definitions

> [Index](../README.md) > [MediaStore](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#mediastore)
    type annotations stubs module [types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

## CorsRuleUnionTypeDef

```python
# CorsRuleUnionTypeDef definition

CorsRuleUnionTypeDef = Union[
    CorsRuleTypeDef,  # (1)
    CorsRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CorsRuleTypeDef](./type_defs.md#corsruletypedef) 
2. See [:material-code-braces: CorsRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef) 



## ContainerTypeDef

```python
# ContainerTypeDef definition

class ContainerTypeDef(TypedDict):
    Endpoint: NotRequired[str],
    CreationTime: NotRequired[datetime],
    ARN: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ContainerStatusType],  # (1)
    AccessLoggingEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: ContainerStatusType](./literals.md#containerstatustype) 
## CorsRuleOutputTypeDef

```python
# CorsRuleOutputTypeDef definition

class CorsRuleOutputTypeDef(TypedDict):
    AllowedOrigins: list[str],
    AllowedHeaders: list[str],
    AllowedMethods: NotRequired[list[MethodNameType]],  # (1)
    MaxAgeSeconds: NotRequired[int],
    ExposeHeaders: NotRequired[list[str]],
```

1. See [:material-code-brackets: MethodNameType](./literals.md#methodnametype) 
## CorsRuleTypeDef

```python
# CorsRuleTypeDef definition

class CorsRuleTypeDef(TypedDict):
    AllowedOrigins: Sequence[str],
    AllowedHeaders: Sequence[str],
    AllowedMethods: NotRequired[Sequence[MethodNameType]],  # (1)
    MaxAgeSeconds: NotRequired[int],
    ExposeHeaders: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: MethodNameType](./literals.md#methodnametype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
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

## DeleteContainerInputRequestTypeDef

```python
# DeleteContainerInputRequestTypeDef definition

class DeleteContainerInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## DeleteContainerPolicyInputRequestTypeDef

```python
# DeleteContainerPolicyInputRequestTypeDef definition

class DeleteContainerPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## DeleteCorsPolicyInputRequestTypeDef

```python
# DeleteCorsPolicyInputRequestTypeDef definition

class DeleteCorsPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## DeleteLifecyclePolicyInputRequestTypeDef

```python
# DeleteLifecyclePolicyInputRequestTypeDef definition

class DeleteLifecyclePolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## DeleteMetricPolicyInputRequestTypeDef

```python
# DeleteMetricPolicyInputRequestTypeDef definition

class DeleteMetricPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## DescribeContainerInputRequestTypeDef

```python
# DescribeContainerInputRequestTypeDef definition

class DescribeContainerInputRequestTypeDef(TypedDict):
    ContainerName: NotRequired[str],
```

## GetContainerPolicyInputRequestTypeDef

```python
# GetContainerPolicyInputRequestTypeDef definition

class GetContainerPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## GetCorsPolicyInputRequestTypeDef

```python
# GetCorsPolicyInputRequestTypeDef definition

class GetCorsPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## GetLifecyclePolicyInputRequestTypeDef

```python
# GetLifecyclePolicyInputRequestTypeDef definition

class GetLifecyclePolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## GetMetricPolicyInputRequestTypeDef

```python
# GetMetricPolicyInputRequestTypeDef definition

class GetMetricPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListContainersInputRequestTypeDef

```python
# ListContainersInputRequestTypeDef definition

class ListContainersInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    Resource: str,
```

## MetricPolicyRuleTypeDef

```python
# MetricPolicyRuleTypeDef definition

class MetricPolicyRuleTypeDef(TypedDict):
    ObjectGroup: str,
    ObjectGroupName: str,
```

## PutContainerPolicyInputRequestTypeDef

```python
# PutContainerPolicyInputRequestTypeDef definition

class PutContainerPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
    Policy: str,
```

## PutLifecyclePolicyInputRequestTypeDef

```python
# PutLifecyclePolicyInputRequestTypeDef definition

class PutLifecyclePolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
    LifecyclePolicy: str,
```

## StartAccessLoggingInputRequestTypeDef

```python
# StartAccessLoggingInputRequestTypeDef definition

class StartAccessLoggingInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## StopAccessLoggingInputRequestTypeDef

```python
# StopAccessLoggingInputRequestTypeDef definition

class StopAccessLoggingInputRequestTypeDef(TypedDict):
    ContainerName: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    Resource: str,
    TagKeys: Sequence[str],
```

## CreateContainerInputRequestTypeDef

```python
# CreateContainerInputRequestTypeDef definition

class CreateContainerInputRequestTypeDef(TypedDict):
    ContainerName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    Resource: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateContainerOutputTypeDef

```python
# CreateContainerOutputTypeDef definition

class CreateContainerOutputTypeDef(TypedDict):
    Container: ContainerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContainerOutputTypeDef

```python
# DescribeContainerOutputTypeDef definition

class DescribeContainerOutputTypeDef(TypedDict):
    Container: ContainerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContainerPolicyOutputTypeDef

```python
# GetContainerPolicyOutputTypeDef definition

class GetContainerPolicyOutputTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCorsPolicyOutputTypeDef

```python
# GetCorsPolicyOutputTypeDef definition

class GetCorsPolicyOutputTypeDef(TypedDict):
    CorsPolicy: list[CorsRuleOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CorsRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLifecyclePolicyOutputTypeDef

```python
# GetLifecyclePolicyOutputTypeDef definition

class GetLifecyclePolicyOutputTypeDef(TypedDict):
    LifecyclePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContainersOutputTypeDef

```python
# ListContainersOutputTypeDef definition

class ListContainersOutputTypeDef(TypedDict):
    Containers: list[ContainerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: list[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContainersInputPaginateTypeDef

```python
# ListContainersInputPaginateTypeDef definition

class ListContainersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MetricPolicyOutputTypeDef

```python
# MetricPolicyOutputTypeDef definition

class MetricPolicyOutputTypeDef(TypedDict):
    ContainerLevelMetrics: ContainerLevelMetricsType,  # (1)
    MetricPolicyRules: NotRequired[list[MetricPolicyRuleTypeDef]],  # (2)
```

1. See [:material-code-brackets: ContainerLevelMetricsType](./literals.md#containerlevelmetricstype) 
2. See [:material-code-braces: MetricPolicyRuleTypeDef](./type_defs.md#metricpolicyruletypedef) 
## MetricPolicyTypeDef

```python
# MetricPolicyTypeDef definition

class MetricPolicyTypeDef(TypedDict):
    ContainerLevelMetrics: ContainerLevelMetricsType,  # (1)
    MetricPolicyRules: NotRequired[Sequence[MetricPolicyRuleTypeDef]],  # (2)
```

1. See [:material-code-brackets: ContainerLevelMetricsType](./literals.md#containerlevelmetricstype) 
2. See [:material-code-braces: MetricPolicyRuleTypeDef](./type_defs.md#metricpolicyruletypedef) 
## PutCorsPolicyInputRequestTypeDef

```python
# PutCorsPolicyInputRequestTypeDef definition

class PutCorsPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
    CorsPolicy: Sequence[CorsRuleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CorsRuleTypeDef](./type_defs.md#corsruletypedef) [:material-code-braces: CorsRuleOutputTypeDef](./type_defs.md#corsruleoutputtypedef) 
## GetMetricPolicyOutputTypeDef

```python
# GetMetricPolicyOutputTypeDef definition

class GetMetricPolicyOutputTypeDef(TypedDict):
    MetricPolicy: MetricPolicyOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricPolicyOutputTypeDef](./type_defs.md#metricpolicyoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMetricPolicyInputRequestTypeDef

```python
# PutMetricPolicyInputRequestTypeDef definition

class PutMetricPolicyInputRequestTypeDef(TypedDict):
    ContainerName: str,
    MetricPolicy: MetricPolicyTypeDef,  # (1)
```

1. See [:material-code-braces: MetricPolicyTypeDef](./type_defs.md#metricpolicytypedef) 