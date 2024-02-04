# Type definitions

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
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

## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## DatapointTypeDef

```python
# DatapointTypeDef definition

class DatapointTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    Value: NotRequired[float],
```

## DeleteScalingPlanRequestRequestTypeDef

```python
# DeleteScalingPlanRequestRequestTypeDef definition

class DeleteScalingPlanRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeScalingPlanResourcesRequestRequestTypeDef

```python
# DescribeScalingPlanResourcesRequestRequestTypeDef definition

class DescribeScalingPlanResourcesRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PredefinedLoadMetricSpecificationTypeDef

```python
# PredefinedLoadMetricSpecificationTypeDef definition

class PredefinedLoadMetricSpecificationTypeDef(TypedDict):
    PredefinedLoadMetricType: LoadMetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: LoadMetricTypeType](./literals.md#loadmetrictypetype) 
## PredefinedScalingMetricSpecificationTypeDef

```python
# PredefinedScalingMetricSpecificationTypeDef definition

class PredefinedScalingMetricSpecificationTypeDef(TypedDict):
    PredefinedScalingMetricType: ScalingMetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: ScalingMetricTypeType](./literals.md#scalingmetrictypetype) 
## ApplicationSourceTypeDef

```python
# ApplicationSourceTypeDef definition

class ApplicationSourceTypeDef(TypedDict):
    CloudFormationStackARN: NotRequired[str],
    TagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## CreateScalingPlanResponseTypeDef

```python
# CreateScalingPlanResponseTypeDef definition

class CreateScalingPlanResponseTypeDef(TypedDict):
    ScalingPlanVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomizedLoadMetricSpecificationPaginatorTypeDef

```python
# CustomizedLoadMetricSpecificationPaginatorTypeDef definition

class CustomizedLoadMetricSpecificationPaginatorTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## CustomizedLoadMetricSpecificationTypeDef

```python
# CustomizedLoadMetricSpecificationTypeDef definition

class CustomizedLoadMetricSpecificationTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## CustomizedScalingMetricSpecificationPaginatorTypeDef

```python
# CustomizedScalingMetricSpecificationPaginatorTypeDef definition

class CustomizedScalingMetricSpecificationPaginatorTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## CustomizedScalingMetricSpecificationTypeDef

```python
# CustomizedScalingMetricSpecificationTypeDef definition

class CustomizedScalingMetricSpecificationTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetScalingPlanResourceForecastDataResponseTypeDef

```python
# GetScalingPlanResourceForecastDataResponseTypeDef definition

class GetScalingPlanResourceForecastDataResponseTypeDef(TypedDict):
    Datapoints: List[DatapointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatapointTypeDef](./type_defs.md#datapointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef

```python
# DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef definition

class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetScalingPlanResourceForecastDataRequestRequestTypeDef

```python
# GetScalingPlanResourceForecastDataRequestRequestTypeDef definition

class GetScalingPlanResourceForecastDataRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    ForecastDataType: ForecastDataTypeType,  # (3)
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: ForecastDataTypeType](./literals.md#forecastdatatypetype) 
## DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef

```python
# DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef definition

class DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef(TypedDict):
    ScalingPlanNames: NotRequired[Sequence[str]],
    ScalingPlanVersion: NotRequired[int],
    ApplicationSources: NotRequired[Sequence[ApplicationSourceTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScalingPlansRequestRequestTypeDef

```python
# DescribeScalingPlansRequestRequestTypeDef definition

class DescribeScalingPlansRequestRequestTypeDef(TypedDict):
    ScalingPlanNames: NotRequired[Sequence[str]],
    ScalingPlanVersion: NotRequired[int],
    ApplicationSources: NotRequired[Sequence[ApplicationSourceTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
## TargetTrackingConfigurationPaginatorTypeDef

```python
# TargetTrackingConfigurationPaginatorTypeDef definition

class TargetTrackingConfigurationPaginatorTypeDef(TypedDict):
    TargetValue: float,
    PredefinedScalingMetricSpecification: NotRequired[PredefinedScalingMetricSpecificationTypeDef],  # (1)
    CustomizedScalingMetricSpecification: NotRequired[CustomizedScalingMetricSpecificationPaginatorTypeDef],  # (2)
    DisableScaleIn: NotRequired[bool],
    ScaleOutCooldown: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    EstimatedInstanceWarmup: NotRequired[int],
```

1. See [:material-code-braces: PredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predefinedscalingmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedScalingMetricSpecificationPaginatorTypeDef](./type_defs.md#customizedscalingmetricspecificationpaginatortypedef) 
## TargetTrackingConfigurationTypeDef

```python
# TargetTrackingConfigurationTypeDef definition

class TargetTrackingConfigurationTypeDef(TypedDict):
    TargetValue: float,
    PredefinedScalingMetricSpecification: NotRequired[PredefinedScalingMetricSpecificationTypeDef],  # (1)
    CustomizedScalingMetricSpecification: NotRequired[CustomizedScalingMetricSpecificationTypeDef],  # (2)
    DisableScaleIn: NotRequired[bool],
    ScaleOutCooldown: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    EstimatedInstanceWarmup: NotRequired[int],
```

1. See [:material-code-braces: PredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predefinedscalingmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedScalingMetricSpecificationTypeDef](./type_defs.md#customizedscalingmetricspecificationtypedef) 
## ScalingInstructionPaginatorTypeDef

```python
# ScalingInstructionPaginatorTypeDef definition

class ScalingInstructionPaginatorTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: int,
    MaxCapacity: int,
    TargetTrackingConfigurations: List[TargetTrackingConfigurationPaginatorTypeDef],  # (3)
    PredefinedLoadMetricSpecification: NotRequired[PredefinedLoadMetricSpecificationTypeDef],  # (4)
    CustomizedLoadMetricSpecification: NotRequired[CustomizedLoadMetricSpecificationPaginatorTypeDef],  # (5)
    ScheduledActionBufferTime: NotRequired[int],
    PredictiveScalingMaxCapacityBehavior: NotRequired[PredictiveScalingMaxCapacityBehaviorType],  # (6)
    PredictiveScalingMaxCapacityBuffer: NotRequired[int],
    PredictiveScalingMode: NotRequired[PredictiveScalingModeType],  # (7)
    ScalingPolicyUpdateBehavior: NotRequired[ScalingPolicyUpdateBehaviorType],  # (8)
    DisableDynamicScaling: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: TargetTrackingConfigurationPaginatorTypeDef](./type_defs.md#targettrackingconfigurationpaginatortypedef) 
4. See [:material-code-braces: PredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predefinedloadmetricspecificationtypedef) 
5. See [:material-code-braces: CustomizedLoadMetricSpecificationPaginatorTypeDef](./type_defs.md#customizedloadmetricspecificationpaginatortypedef) 
6. See [:material-code-brackets: PredictiveScalingMaxCapacityBehaviorType](./literals.md#predictivescalingmaxcapacitybehaviortype) 
7. See [:material-code-brackets: PredictiveScalingModeType](./literals.md#predictivescalingmodetype) 
8. See [:material-code-brackets: ScalingPolicyUpdateBehaviorType](./literals.md#scalingpolicyupdatebehaviortype) 
## ScalingPolicyPaginatorTypeDef

```python
# ScalingPolicyPaginatorTypeDef definition

class ScalingPolicyPaginatorTypeDef(TypedDict):
    PolicyName: str,
    PolicyType: PolicyTypeType,  # (1)
    TargetTrackingConfiguration: NotRequired[TargetTrackingConfigurationPaginatorTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: TargetTrackingConfigurationPaginatorTypeDef](./type_defs.md#targettrackingconfigurationpaginatortypedef) 
## ScalingInstructionTypeDef

```python
# ScalingInstructionTypeDef definition

class ScalingInstructionTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: int,
    MaxCapacity: int,
    TargetTrackingConfigurations: Sequence[TargetTrackingConfigurationTypeDef],  # (3)
    PredefinedLoadMetricSpecification: NotRequired[PredefinedLoadMetricSpecificationTypeDef],  # (4)
    CustomizedLoadMetricSpecification: NotRequired[CustomizedLoadMetricSpecificationTypeDef],  # (5)
    ScheduledActionBufferTime: NotRequired[int],
    PredictiveScalingMaxCapacityBehavior: NotRequired[PredictiveScalingMaxCapacityBehaviorType],  # (6)
    PredictiveScalingMaxCapacityBuffer: NotRequired[int],
    PredictiveScalingMode: NotRequired[PredictiveScalingModeType],  # (7)
    ScalingPolicyUpdateBehavior: NotRequired[ScalingPolicyUpdateBehaviorType],  # (8)
    DisableDynamicScaling: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) 
4. See [:material-code-braces: PredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predefinedloadmetricspecificationtypedef) 
5. See [:material-code-braces: CustomizedLoadMetricSpecificationTypeDef](./type_defs.md#customizedloadmetricspecificationtypedef) 
6. See [:material-code-brackets: PredictiveScalingMaxCapacityBehaviorType](./literals.md#predictivescalingmaxcapacitybehaviortype) 
7. See [:material-code-brackets: PredictiveScalingModeType](./literals.md#predictivescalingmodetype) 
8. See [:material-code-brackets: ScalingPolicyUpdateBehaviorType](./literals.md#scalingpolicyupdatebehaviortype) 
## ScalingPolicyTypeDef

```python
# ScalingPolicyTypeDef definition

class ScalingPolicyTypeDef(TypedDict):
    PolicyName: str,
    PolicyType: PolicyTypeType,  # (1)
    TargetTrackingConfiguration: NotRequired[TargetTrackingConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) 
## ScalingPlanPaginatorTypeDef

```python
# ScalingPlanPaginatorTypeDef definition

class ScalingPlanPaginatorTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ApplicationSource: ApplicationSourceTypeDef,  # (1)
    ScalingInstructions: List[ScalingInstructionPaginatorTypeDef],  # (2)
    StatusCode: ScalingPlanStatusCodeType,  # (3)
    StatusMessage: NotRequired[str],
    StatusStartTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionPaginatorTypeDef](./type_defs.md#scalinginstructionpaginatortypedef) 
3. See [:material-code-brackets: ScalingPlanStatusCodeType](./literals.md#scalingplanstatuscodetype) 
## ScalingPlanResourcePaginatorTypeDef

```python
# ScalingPlanResourcePaginatorTypeDef definition

class ScalingPlanResourcePaginatorTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    ScalingStatusCode: ScalingStatusCodeType,  # (4)
    ScalingPolicies: NotRequired[List[ScalingPolicyPaginatorTypeDef]],  # (3)
    ScalingStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: ScalingPolicyPaginatorTypeDef](./type_defs.md#scalingpolicypaginatortypedef) 
4. See [:material-code-brackets: ScalingStatusCodeType](./literals.md#scalingstatuscodetype) 
## CreateScalingPlanRequestRequestTypeDef

```python
# CreateScalingPlanRequestRequestTypeDef definition

class CreateScalingPlanRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ApplicationSource: ApplicationSourceTypeDef,  # (1)
    ScalingInstructions: Sequence[ScalingInstructionTypeDef],  # (2)
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) 
## ScalingPlanTypeDef

```python
# ScalingPlanTypeDef definition

class ScalingPlanTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ApplicationSource: ApplicationSourceTypeDef,  # (1)
    ScalingInstructions: List[ScalingInstructionTypeDef],  # (2)
    StatusCode: ScalingPlanStatusCodeType,  # (3)
    StatusMessage: NotRequired[str],
    StatusStartTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) 
3. See [:material-code-brackets: ScalingPlanStatusCodeType](./literals.md#scalingplanstatuscodetype) 
## UpdateScalingPlanRequestRequestTypeDef

```python
# UpdateScalingPlanRequestRequestTypeDef definition

class UpdateScalingPlanRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ApplicationSource: NotRequired[ApplicationSourceTypeDef],  # (1)
    ScalingInstructions: NotRequired[Sequence[ScalingInstructionTypeDef]],  # (2)
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) 
## ScalingPlanResourceTypeDef

```python
# ScalingPlanResourceTypeDef definition

class ScalingPlanResourceTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    ScalingStatusCode: ScalingStatusCodeType,  # (4)
    ScalingPolicies: NotRequired[List[ScalingPolicyTypeDef]],  # (3)
    ScalingStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef) 
4. See [:material-code-brackets: ScalingStatusCodeType](./literals.md#scalingstatuscodetype) 
## DescribeScalingPlansResponsePaginatorTypeDef

```python
# DescribeScalingPlansResponsePaginatorTypeDef definition

class DescribeScalingPlansResponsePaginatorTypeDef(TypedDict):
    ScalingPlans: List[ScalingPlanPaginatorTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScalingPlanPaginatorTypeDef](./type_defs.md#scalingplanpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPlanResourcesResponsePaginatorTypeDef

```python
# DescribeScalingPlanResourcesResponsePaginatorTypeDef definition

class DescribeScalingPlanResourcesResponsePaginatorTypeDef(TypedDict):
    ScalingPlanResources: List[ScalingPlanResourcePaginatorTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScalingPlanResourcePaginatorTypeDef](./type_defs.md#scalingplanresourcepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPlansResponseTypeDef

```python
# DescribeScalingPlansResponseTypeDef definition

class DescribeScalingPlansResponseTypeDef(TypedDict):
    ScalingPlans: List[ScalingPlanTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScalingPlanTypeDef](./type_defs.md#scalingplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPlanResourcesResponseTypeDef

```python
# DescribeScalingPlanResourcesResponseTypeDef definition

class DescribeScalingPlanResourcesResponseTypeDef(TypedDict):
    ScalingPlanResources: List[ScalingPlanResourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScalingPlanResourceTypeDef](./type_defs.md#scalingplanresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
