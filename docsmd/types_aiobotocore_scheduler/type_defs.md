# Type definitions

> [Index](../README.md) > [EventBridgeScheduler](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EventBridgeScheduler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#eventbridgescheduler)
    type annotations stubs module [types-aiobotocore-scheduler](https://pypi.org/project/types-aiobotocore-scheduler/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AwsVpcConfigurationUnionTypeDef

```python
# AwsVpcConfigurationUnionTypeDef definition

AwsVpcConfigurationUnionTypeDef = Union[
    AwsVpcConfigurationTypeDef,  # (1)
    AwsVpcConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef) 
2. See [:material-code-braces: AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef) 

## SageMakerPipelineParametersUnionTypeDef

```python
# SageMakerPipelineParametersUnionTypeDef definition

SageMakerPipelineParametersUnionTypeDef = Union[
    SageMakerPipelineParametersTypeDef,  # (1)
    SageMakerPipelineParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SageMakerPipelineParametersTypeDef](./type_defs.md#sagemakerpipelineparameterstypedef) 
2. See [:material-code-braces: SageMakerPipelineParametersOutputTypeDef](./type_defs.md#sagemakerpipelineparametersoutputtypedef) 

## NetworkConfigurationUnionTypeDef

```python
# NetworkConfigurationUnionTypeDef definition

NetworkConfigurationUnionTypeDef = Union[
    NetworkConfigurationTypeDef,  # (1)
    NetworkConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 

## EcsParametersUnionTypeDef

```python
# EcsParametersUnionTypeDef definition

EcsParametersUnionTypeDef = Union[
    EcsParametersTypeDef,  # (1)
    EcsParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EcsParametersTypeDef](./type_defs.md#ecsparameterstypedef) 
2. See [:material-code-braces: EcsParametersOutputTypeDef](./type_defs.md#ecsparametersoutputtypedef) 



## AwsVpcConfigurationOutputTypeDef

```python
# AwsVpcConfigurationOutputTypeDef definition

class AwsVpcConfigurationOutputTypeDef(TypedDict):
    Subnets: list[str],
    AssignPublicIp: NotRequired[AssignPublicIpType],  # (1)
    SecurityGroups: NotRequired[list[str]],
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## AwsVpcConfigurationTypeDef

```python
# AwsVpcConfigurationTypeDef definition

class AwsVpcConfigurationTypeDef(TypedDict):
    Subnets: Sequence[str],
    AssignPublicIp: NotRequired[AssignPublicIpType],  # (1)
    SecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## CapacityProviderStrategyItemTypeDef

```python
# CapacityProviderStrategyItemTypeDef definition

class CapacityProviderStrategyItemTypeDef(TypedDict):
    capacityProvider: str,
    base: NotRequired[int],
    weight: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## FlexibleTimeWindowTypeDef

```python
# FlexibleTimeWindowTypeDef definition

class FlexibleTimeWindowTypeDef(TypedDict):
    Mode: FlexibleTimeWindowModeType,  # (1)
    MaximumWindowInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: FlexibleTimeWindowModeType](./literals.md#flexibletimewindowmodetype) 
## DeadLetterConfigTypeDef

```python
# DeadLetterConfigTypeDef definition

class DeadLetterConfigTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## DeleteScheduleGroupInputRequestTypeDef

```python
# DeleteScheduleGroupInputRequestTypeDef definition

class DeleteScheduleGroupInputRequestTypeDef(TypedDict):
    Name: str,
    ClientToken: NotRequired[str],
```

## DeleteScheduleInputRequestTypeDef

```python
# DeleteScheduleInputRequestTypeDef definition

class DeleteScheduleInputRequestTypeDef(TypedDict):
    Name: str,
    ClientToken: NotRequired[str],
    GroupName: NotRequired[str],
```

## PlacementConstraintTypeDef

```python
# PlacementConstraintTypeDef definition

class PlacementConstraintTypeDef(TypedDict):
    expression: NotRequired[str],
    type: NotRequired[PlacementConstraintTypeType],  # (1)
```

1. See [:material-code-brackets: PlacementConstraintTypeType](./literals.md#placementconstrainttypetype) 
## PlacementStrategyTypeDef

```python
# PlacementStrategyTypeDef definition

class PlacementStrategyTypeDef(TypedDict):
    field: NotRequired[str],
    type: NotRequired[PlacementStrategyTypeType],  # (1)
```

1. See [:material-code-brackets: PlacementStrategyTypeType](./literals.md#placementstrategytypetype) 
## EventBridgeParametersTypeDef

```python
# EventBridgeParametersTypeDef definition

class EventBridgeParametersTypeDef(TypedDict):
    DetailType: str,
    Source: str,
```

## GetScheduleGroupInputRequestTypeDef

```python
# GetScheduleGroupInputRequestTypeDef definition

class GetScheduleGroupInputRequestTypeDef(TypedDict):
    Name: str,
```

## GetScheduleInputRequestTypeDef

```python
# GetScheduleInputRequestTypeDef definition

class GetScheduleInputRequestTypeDef(TypedDict):
    Name: str,
    GroupName: NotRequired[str],
```

## KinesisParametersTypeDef

```python
# KinesisParametersTypeDef definition

class KinesisParametersTypeDef(TypedDict):
    PartitionKey: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListScheduleGroupsInputRequestTypeDef

```python
# ListScheduleGroupsInputRequestTypeDef definition

class ListScheduleGroupsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
```

## ScheduleGroupSummaryTypeDef

```python
# ScheduleGroupSummaryTypeDef definition

class ScheduleGroupSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    LastModificationDate: NotRequired[datetime],
    Name: NotRequired[str],
    State: NotRequired[ScheduleGroupStateType],  # (1)
```

1. See [:material-code-brackets: ScheduleGroupStateType](./literals.md#schedulegroupstatetype) 
## ListSchedulesInputRequestTypeDef

```python
# ListSchedulesInputRequestTypeDef definition

class ListSchedulesInputRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    MaxResults: NotRequired[int],
    NamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    State: NotRequired[ScheduleStateType],  # (1)
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## RetryPolicyTypeDef

```python
# RetryPolicyTypeDef definition

class RetryPolicyTypeDef(TypedDict):
    MaximumEventAgeInSeconds: NotRequired[int],
    MaximumRetryAttempts: NotRequired[int],
```

## SageMakerPipelineParameterTypeDef

```python
# SageMakerPipelineParameterTypeDef definition

class SageMakerPipelineParameterTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## TargetSummaryTypeDef

```python
# TargetSummaryTypeDef definition

class TargetSummaryTypeDef(TypedDict):
    Arn: str,
```

## SqsParametersTypeDef

```python
# SqsParametersTypeDef definition

class SqsParametersTypeDef(TypedDict):
    MessageGroupId: NotRequired[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## NetworkConfigurationOutputTypeDef

```python
# NetworkConfigurationOutputTypeDef definition

class NetworkConfigurationOutputTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef) 
## CreateScheduleGroupInputRequestTypeDef

```python
# CreateScheduleGroupInputRequestTypeDef definition

class CreateScheduleGroupInputRequestTypeDef(TypedDict):
    Name: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateScheduleGroupOutputTypeDef

```python
# CreateScheduleGroupOutputTypeDef definition

class CreateScheduleGroupOutputTypeDef(TypedDict):
    ScheduleGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduleOutputTypeDef

```python
# CreateScheduleOutputTypeDef definition

class CreateScheduleOutputTypeDef(TypedDict):
    ScheduleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetScheduleGroupOutputTypeDef

```python
# GetScheduleGroupOutputTypeDef definition

class GetScheduleGroupOutputTypeDef(TypedDict):
    Arn: str,
    CreationDate: datetime,
    LastModificationDate: datetime,
    Name: str,
    State: ScheduleGroupStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ScheduleGroupStateType](./literals.md#schedulegroupstatetype) 
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
## UpdateScheduleOutputTypeDef

```python
# UpdateScheduleOutputTypeDef definition

class UpdateScheduleOutputTypeDef(TypedDict):
    ScheduleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScheduleGroupsInputPaginateTypeDef

```python
# ListScheduleGroupsInputPaginateTypeDef definition

class ListScheduleGroupsInputPaginateTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchedulesInputPaginateTypeDef

```python
# ListSchedulesInputPaginateTypeDef definition

class ListSchedulesInputPaginateTypeDef(TypedDict):
    GroupName: NotRequired[str],
    NamePrefix: NotRequired[str],
    State: NotRequired[ScheduleStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScheduleGroupsOutputTypeDef

```python
# ListScheduleGroupsOutputTypeDef definition

class ListScheduleGroupsOutputTypeDef(TypedDict):
    ScheduleGroups: list[ScheduleGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduleGroupSummaryTypeDef](./type_defs.md#schedulegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SageMakerPipelineParametersOutputTypeDef

```python
# SageMakerPipelineParametersOutputTypeDef definition

class SageMakerPipelineParametersOutputTypeDef(TypedDict):
    PipelineParameterList: NotRequired[list[SageMakerPipelineParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: SageMakerPipelineParameterTypeDef](./type_defs.md#sagemakerpipelineparametertypedef) 
## SageMakerPipelineParametersTypeDef

```python
# SageMakerPipelineParametersTypeDef definition

class SageMakerPipelineParametersTypeDef(TypedDict):
    PipelineParameterList: NotRequired[Sequence[SageMakerPipelineParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: SageMakerPipelineParameterTypeDef](./type_defs.md#sagemakerpipelineparametertypedef) 
## ScheduleSummaryTypeDef

```python
# ScheduleSummaryTypeDef definition

class ScheduleSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    GroupName: NotRequired[str],
    LastModificationDate: NotRequired[datetime],
    Name: NotRequired[str],
    State: NotRequired[ScheduleStateType],  # (1)
    Target: NotRequired[TargetSummaryTypeDef],  # (2)
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
2. See [:material-code-braces: TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef) 
## EcsParametersOutputTypeDef

```python
# EcsParametersOutputTypeDef definition

class EcsParametersOutputTypeDef(TypedDict):
    TaskDefinitionArn: str,
    CapacityProviderStrategy: NotRequired[list[CapacityProviderStrategyItemTypeDef]],  # (1)
    EnableECSManagedTags: NotRequired[bool],
    EnableExecuteCommand: NotRequired[bool],
    Group: NotRequired[str],
    LaunchType: NotRequired[LaunchTypeType],  # (2)
    NetworkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (3)
    PlacementConstraints: NotRequired[list[PlacementConstraintTypeDef]],  # (4)
    PlacementStrategy: NotRequired[list[PlacementStrategyTypeDef]],  # (5)
    PlatformVersion: NotRequired[str],
    PropagateTags: NotRequired[PropagateTagsType],  # (6)
    ReferenceId: NotRequired[str],
    Tags: NotRequired[list[dict[str, str]]],
    TaskCount: NotRequired[int],
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
4. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
5. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
6. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef) [:material-code-braces: AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef) 
## ListSchedulesOutputTypeDef

```python
# ListSchedulesOutputTypeDef definition

class ListSchedulesOutputTypeDef(TypedDict):
    Schedules: list[ScheduleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduleSummaryTypeDef](./type_defs.md#schedulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetOutputTypeDef

```python
# TargetOutputTypeDef definition

class TargetOutputTypeDef(TypedDict):
    Arn: str,
    RoleArn: str,
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (1)
    EcsParameters: NotRequired[EcsParametersOutputTypeDef],  # (2)
    EventBridgeParameters: NotRequired[EventBridgeParametersTypeDef],  # (3)
    Input: NotRequired[str],
    KinesisParameters: NotRequired[KinesisParametersTypeDef],  # (4)
    RetryPolicy: NotRequired[RetryPolicyTypeDef],  # (5)
    SageMakerPipelineParameters: NotRequired[SageMakerPipelineParametersOutputTypeDef],  # (6)
    SqsParameters: NotRequired[SqsParametersTypeDef],  # (7)
```

1. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
2. See [:material-code-braces: EcsParametersOutputTypeDef](./type_defs.md#ecsparametersoutputtypedef) 
3. See [:material-code-braces: EventBridgeParametersTypeDef](./type_defs.md#eventbridgeparameterstypedef) 
4. See [:material-code-braces: KinesisParametersTypeDef](./type_defs.md#kinesisparameterstypedef) 
5. See [:material-code-braces: RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef) 
6. See [:material-code-braces: SageMakerPipelineParametersOutputTypeDef](./type_defs.md#sagemakerpipelineparametersoutputtypedef) 
7. See [:material-code-braces: SqsParametersTypeDef](./type_defs.md#sqsparameterstypedef) 
## GetScheduleOutputTypeDef

```python
# GetScheduleOutputTypeDef definition

class GetScheduleOutputTypeDef(TypedDict):
    ActionAfterCompletion: ActionAfterCompletionType,  # (1)
    Arn: str,
    CreationDate: datetime,
    Description: str,
    EndDate: datetime,
    FlexibleTimeWindow: FlexibleTimeWindowTypeDef,  # (2)
    GroupName: str,
    KmsKeyArn: str,
    LastModificationDate: datetime,
    Name: str,
    ScheduleExpression: str,
    ScheduleExpressionTimezone: str,
    StartDate: datetime,
    State: ScheduleStateType,  # (3)
    Target: TargetOutputTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ActionAfterCompletionType](./literals.md#actionaftercompletiontype) 
2. See [:material-code-braces: FlexibleTimeWindowTypeDef](./type_defs.md#flexibletimewindowtypedef) 
3. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
4. See [:material-code-braces: TargetOutputTypeDef](./type_defs.md#targetoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EcsParametersTypeDef

```python
# EcsParametersTypeDef definition

class EcsParametersTypeDef(TypedDict):
    TaskDefinitionArn: str,
    CapacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (1)
    EnableECSManagedTags: NotRequired[bool],
    EnableExecuteCommand: NotRequired[bool],
    Group: NotRequired[str],
    LaunchType: NotRequired[LaunchTypeType],  # (2)
    NetworkConfiguration: NotRequired[NetworkConfigurationUnionTypeDef],  # (3)
    PlacementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (4)
    PlacementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (5)
    PlatformVersion: NotRequired[str],
    PropagateTags: NotRequired[PropagateTagsType],  # (6)
    ReferenceId: NotRequired[str],
    Tags: NotRequired[Sequence[Mapping[str, str]]],
    TaskCount: NotRequired[int],
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
4. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
5. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
6. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    Arn: str,
    RoleArn: str,
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (1)
    EcsParameters: NotRequired[EcsParametersUnionTypeDef],  # (2)
    EventBridgeParameters: NotRequired[EventBridgeParametersTypeDef],  # (3)
    Input: NotRequired[str],
    KinesisParameters: NotRequired[KinesisParametersTypeDef],  # (4)
    RetryPolicy: NotRequired[RetryPolicyTypeDef],  # (5)
    SageMakerPipelineParameters: NotRequired[SageMakerPipelineParametersUnionTypeDef],  # (6)
    SqsParameters: NotRequired[SqsParametersTypeDef],  # (7)
```

1. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
2. See [:material-code-braces: EcsParametersTypeDef](./type_defs.md#ecsparameterstypedef) [:material-code-braces: EcsParametersOutputTypeDef](./type_defs.md#ecsparametersoutputtypedef) 
3. See [:material-code-braces: EventBridgeParametersTypeDef](./type_defs.md#eventbridgeparameterstypedef) 
4. See [:material-code-braces: KinesisParametersTypeDef](./type_defs.md#kinesisparameterstypedef) 
5. See [:material-code-braces: RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef) 
6. See [:material-code-braces: SageMakerPipelineParametersTypeDef](./type_defs.md#sagemakerpipelineparameterstypedef) [:material-code-braces: SageMakerPipelineParametersOutputTypeDef](./type_defs.md#sagemakerpipelineparametersoutputtypedef) 
7. See [:material-code-braces: SqsParametersTypeDef](./type_defs.md#sqsparameterstypedef) 
## CreateScheduleInputRequestTypeDef

```python
# CreateScheduleInputRequestTypeDef definition

class CreateScheduleInputRequestTypeDef(TypedDict):
    FlexibleTimeWindow: FlexibleTimeWindowTypeDef,  # (1)
    Name: str,
    ScheduleExpression: str,
    Target: TargetTypeDef,  # (2)
    ActionAfterCompletion: NotRequired[ActionAfterCompletionType],  # (3)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    EndDate: NotRequired[TimestampTypeDef],
    GroupName: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    ScheduleExpressionTimezone: NotRequired[str],
    StartDate: NotRequired[TimestampTypeDef],
    State: NotRequired[ScheduleStateType],  # (4)
```

1. See [:material-code-braces: FlexibleTimeWindowTypeDef](./type_defs.md#flexibletimewindowtypedef) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
3. See [:material-code-brackets: ActionAfterCompletionType](./literals.md#actionaftercompletiontype) 
4. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
## UpdateScheduleInputRequestTypeDef

```python
# UpdateScheduleInputRequestTypeDef definition

class UpdateScheduleInputRequestTypeDef(TypedDict):
    FlexibleTimeWindow: FlexibleTimeWindowTypeDef,  # (1)
    Name: str,
    ScheduleExpression: str,
    Target: TargetTypeDef,  # (2)
    ActionAfterCompletion: NotRequired[ActionAfterCompletionType],  # (3)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    EndDate: NotRequired[TimestampTypeDef],
    GroupName: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    ScheduleExpressionTimezone: NotRequired[str],
    StartDate: NotRequired[TimestampTypeDef],
    State: NotRequired[ScheduleStateType],  # (4)
```

1. See [:material-code-braces: FlexibleTimeWindowTypeDef](./type_defs.md#flexibletimewindowtypedef) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
3. See [:material-code-brackets: ActionAfterCompletionType](./literals.md#actionaftercompletiontype) 
4. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 