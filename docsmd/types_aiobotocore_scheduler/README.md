# EventBridgeScheduler module

> [Index](../README.md) > EventBridgeScheduler


!!! note ""

    Auto-generated documentation for [EventBridgeScheduler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#eventbridgescheduler)
    type annotations stubs module [types-aiobotocore-scheduler](https://pypi.org/project/types-aiobotocore-scheduler/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `EventBridgeScheduler` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `EventBridgeScheduler` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[scheduler]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[scheduler]'

# standalone installation
python -m pip install types-aiobotocore-scheduler
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-scheduler
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EventBridgeSchedulerClient

Type annotations and code completion for  `#!python session.client("scheduler")` as [EventBridgeSchedulerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client)

```python
# EventBridgeSchedulerClient usage example

from aioboto3.session import Session

from types_aiobotocore_scheduler.client import EventBridgeSchedulerClient


session = Session()
async with session.client("scheduler") as client:
    client: EventBridgeSchedulerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("scheduler").get_paginator("...")`.

```python
# ListScheduleGroupsPaginator usage example

from types_aiobotocore_scheduler.paginator import ListScheduleGroupsPaginator

def get_list_schedule_groups_paginator() -> ListScheduleGroupsPaginator:
    return client.get_paginator("list_schedule_groups"))
```

- [ListScheduleGroupsPaginator](./paginators.md#listschedulegroupspaginator)
- [ListSchedulesPaginator](./paginators.md#listschedulespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionAfterCompletionType usage example

from types_aiobotocore_scheduler.literals import ActionAfterCompletionType

def get_value() -> ActionAfterCompletionType:
    return "DELETE"
```

- [ActionAfterCompletionType](./literals.md#actionaftercompletiontype)
- [AssignPublicIpType](./literals.md#assignpubliciptype)
- [FlexibleTimeWindowModeType](./literals.md#flexibletimewindowmodetype)
- [LaunchTypeType](./literals.md#launchtypetype)
- [ListScheduleGroupsPaginatorName](./literals.md#listschedulegroupspaginatorname)
- [ListSchedulesPaginatorName](./literals.md#listschedulespaginatorname)
- [PlacementConstraintTypeType](./literals.md#placementconstrainttypetype)
- [PlacementStrategyTypeType](./literals.md#placementstrategytypetype)
- [PropagateTagsType](./literals.md#propagatetagstype)
- [ScheduleGroupStateType](./literals.md#schedulegroupstatetype)
- [ScheduleStateType](./literals.md#schedulestatetype)
- [EventBridgeSchedulerServiceName](./literals.md#eventbridgeschedulerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef)
- [AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef)
- [CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FlexibleTimeWindowTypeDef](./type_defs.md#flexibletimewindowtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef)
- [DeleteScheduleGroupInputRequestTypeDef](./type_defs.md#deleteschedulegroupinputrequesttypedef)
- [DeleteScheduleInputRequestTypeDef](./type_defs.md#deletescheduleinputrequesttypedef)
- [PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef)
- [PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef)
- [EventBridgeParametersTypeDef](./type_defs.md#eventbridgeparameterstypedef)
- [GetScheduleGroupInputRequestTypeDef](./type_defs.md#getschedulegroupinputrequesttypedef)
- [GetScheduleInputRequestTypeDef](./type_defs.md#getscheduleinputrequesttypedef)
- [KinesisParametersTypeDef](./type_defs.md#kinesisparameterstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListScheduleGroupsInputRequestTypeDef](./type_defs.md#listschedulegroupsinputrequesttypedef)
- [ScheduleGroupSummaryTypeDef](./type_defs.md#schedulegroupsummarytypedef)
- [ListSchedulesInputRequestTypeDef](./type_defs.md#listschedulesinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef)
- [SageMakerPipelineParameterTypeDef](./type_defs.md#sagemakerpipelineparametertypedef)
- [TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef)
- [SqsParametersTypeDef](./type_defs.md#sqsparameterstypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef)
- [AwsVpcConfigurationUnionTypeDef](./type_defs.md#awsvpcconfigurationuniontypedef)
- [CreateScheduleGroupInputRequestTypeDef](./type_defs.md#createschedulegroupinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [CreateScheduleGroupOutputTypeDef](./type_defs.md#createschedulegroupoutputtypedef)
- [CreateScheduleOutputTypeDef](./type_defs.md#createscheduleoutputtypedef)
- [GetScheduleGroupOutputTypeDef](./type_defs.md#getschedulegroupoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [UpdateScheduleOutputTypeDef](./type_defs.md#updatescheduleoutputtypedef)
- [ListScheduleGroupsInputPaginateTypeDef](./type_defs.md#listschedulegroupsinputpaginatetypedef)
- [ListSchedulesInputPaginateTypeDef](./type_defs.md#listschedulesinputpaginatetypedef)
- [ListScheduleGroupsOutputTypeDef](./type_defs.md#listschedulegroupsoutputtypedef)
- [SageMakerPipelineParametersOutputTypeDef](./type_defs.md#sagemakerpipelineparametersoutputtypedef)
- [SageMakerPipelineParametersTypeDef](./type_defs.md#sagemakerpipelineparameterstypedef)
- [ScheduleSummaryTypeDef](./type_defs.md#schedulesummarytypedef)
- [EcsParametersOutputTypeDef](./type_defs.md#ecsparametersoutputtypedef)
- [NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
- [SageMakerPipelineParametersUnionTypeDef](./type_defs.md#sagemakerpipelineparametersuniontypedef)
- [ListSchedulesOutputTypeDef](./type_defs.md#listschedulesoutputtypedef)
- [TargetOutputTypeDef](./type_defs.md#targetoutputtypedef)
- [NetworkConfigurationUnionTypeDef](./type_defs.md#networkconfigurationuniontypedef)
- [GetScheduleOutputTypeDef](./type_defs.md#getscheduleoutputtypedef)
- [EcsParametersTypeDef](./type_defs.md#ecsparameterstypedef)
- [EcsParametersUnionTypeDef](./type_defs.md#ecsparametersuniontypedef)
- [TargetTypeDef](./type_defs.md#targettypedef)
- [CreateScheduleInputRequestTypeDef](./type_defs.md#createscheduleinputrequesttypedef)
- [UpdateScheduleInputRequestTypeDef](./type_defs.md#updatescheduleinputrequesttypedef)
