# SWF module

> [Index](../README.md) > SWF


!!! note ""

    Auto-generated documentation for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#swf)
    type annotations stubs module [types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `SWF` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `SWF` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[swf]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[swf]'

# standalone installation
python -m pip install types-aiobotocore-swf
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-swf
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SWFClient

Type annotations and code completion for  `#!python session.client("swf")` as [SWFClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Client)

```python
# SWFClient usage example

from aioboto3.session import Session

from types_aiobotocore_swf.client import SWFClient


session = Session()
async with session.client("swf") as client:
    client: SWFClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("swf").get_paginator("...")`.

```python
# GetWorkflowExecutionHistoryPaginator usage example

from types_aiobotocore_swf.paginator import GetWorkflowExecutionHistoryPaginator

def get_get_workflow_execution_history_paginator() -> GetWorkflowExecutionHistoryPaginator:
    return client.get_paginator("get_workflow_execution_history"))
```

- [GetWorkflowExecutionHistoryPaginator](./paginators.md#getworkflowexecutionhistorypaginator)
- [ListActivityTypesPaginator](./paginators.md#listactivitytypespaginator)
- [ListClosedWorkflowExecutionsPaginator](./paginators.md#listclosedworkflowexecutionspaginator)
- [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- [ListOpenWorkflowExecutionsPaginator](./paginators.md#listopenworkflowexecutionspaginator)
- [ListWorkflowTypesPaginator](./paginators.md#listworkflowtypespaginator)
- [PollForDecisionTaskPaginator](./paginators.md#pollfordecisiontaskpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActivityTaskTimeoutTypeType usage example

from types_aiobotocore_swf.literals import ActivityTaskTimeoutTypeType

def get_value() -> ActivityTaskTimeoutTypeType:
    return "HEARTBEAT"
```

- [ActivityTaskTimeoutTypeType](./literals.md#activitytasktimeouttypetype)
- [CancelTimerFailedCauseType](./literals.md#canceltimerfailedcausetype)
- [CancelWorkflowExecutionFailedCauseType](./literals.md#cancelworkflowexecutionfailedcausetype)
- [ChildPolicyType](./literals.md#childpolicytype)
- [CloseStatusType](./literals.md#closestatustype)
- [CompleteWorkflowExecutionFailedCauseType](./literals.md#completeworkflowexecutionfailedcausetype)
- [ContinueAsNewWorkflowExecutionFailedCauseType](./literals.md#continueasnewworkflowexecutionfailedcausetype)
- [DecisionTaskTimeoutTypeType](./literals.md#decisiontasktimeouttypetype)
- [DecisionTypeType](./literals.md#decisiontypetype)
- [EventTypeType](./literals.md#eventtypetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [FailWorkflowExecutionFailedCauseType](./literals.md#failworkflowexecutionfailedcausetype)
- [GetWorkflowExecutionHistoryPaginatorName](./literals.md#getworkflowexecutionhistorypaginatorname)
- [LambdaFunctionTimeoutTypeType](./literals.md#lambdafunctiontimeouttypetype)
- [ListActivityTypesPaginatorName](./literals.md#listactivitytypespaginatorname)
- [ListClosedWorkflowExecutionsPaginatorName](./literals.md#listclosedworkflowexecutionspaginatorname)
- [ListDomainsPaginatorName](./literals.md#listdomainspaginatorname)
- [ListOpenWorkflowExecutionsPaginatorName](./literals.md#listopenworkflowexecutionspaginatorname)
- [ListWorkflowTypesPaginatorName](./literals.md#listworkflowtypespaginatorname)
- [PollForDecisionTaskPaginatorName](./literals.md#pollfordecisiontaskpaginatorname)
- [RecordMarkerFailedCauseType](./literals.md#recordmarkerfailedcausetype)
- [RegistrationStatusType](./literals.md#registrationstatustype)
- [RequestCancelActivityTaskFailedCauseType](./literals.md#requestcancelactivitytaskfailedcausetype)
- [RequestCancelExternalWorkflowExecutionFailedCauseType](./literals.md#requestcancelexternalworkflowexecutionfailedcausetype)
- [ScheduleActivityTaskFailedCauseType](./literals.md#scheduleactivitytaskfailedcausetype)
- [ScheduleLambdaFunctionFailedCauseType](./literals.md#schedulelambdafunctionfailedcausetype)
- [SignalExternalWorkflowExecutionFailedCauseType](./literals.md#signalexternalworkflowexecutionfailedcausetype)
- [StartChildWorkflowExecutionFailedCauseType](./literals.md#startchildworkflowexecutionfailedcausetype)
- [StartLambdaFunctionFailedCauseType](./literals.md#startlambdafunctionfailedcausetype)
- [StartTimerFailedCauseType](./literals.md#starttimerfailedcausetype)
- [WorkflowExecutionCancelRequestedCauseType](./literals.md#workflowexecutioncancelrequestedcausetype)
- [WorkflowExecutionTerminatedCauseType](./literals.md#workflowexecutionterminatedcausetype)
- [WorkflowExecutionTimeoutTypeType](./literals.md#workflowexecutiontimeouttypetype)
- [SWFServiceName](./literals.md#swfservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActivityTaskCancelRequestedEventAttributesTypeDef](./type_defs.md#activitytaskcancelrequestedeventattributestypedef)
- [ActivityTaskCanceledEventAttributesTypeDef](./type_defs.md#activitytaskcanceledeventattributestypedef)
- [ActivityTaskCompletedEventAttributesTypeDef](./type_defs.md#activitytaskcompletedeventattributestypedef)
- [ActivityTaskFailedEventAttributesTypeDef](./type_defs.md#activitytaskfailedeventattributestypedef)
- [ActivityTypeTypeDef](./type_defs.md#activitytypetypedef)
- [TaskListTypeDef](./type_defs.md#tasklisttypedef)
- [ActivityTaskStartedEventAttributesTypeDef](./type_defs.md#activitytaskstartedeventattributestypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ActivityTaskTimedOutEventAttributesTypeDef](./type_defs.md#activitytasktimedouteventattributestypedef)
- [WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef)
- [CancelTimerDecisionAttributesTypeDef](./type_defs.md#canceltimerdecisionattributestypedef)
- [CancelTimerFailedEventAttributesTypeDef](./type_defs.md#canceltimerfailedeventattributestypedef)
- [CancelWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#cancelworkflowexecutiondecisionattributestypedef)
- [CancelWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#cancelworkflowexecutionfailedeventattributestypedef)
- [WorkflowTypeTypeDef](./type_defs.md#workflowtypetypedef)
- [CloseStatusFilterTypeDef](./type_defs.md#closestatusfiltertypedef)
- [CompleteWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#completeworkflowexecutiondecisionattributestypedef)
- [CompleteWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#completeworkflowexecutionfailedeventattributestypedef)
- [ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#continueasnewworkflowexecutionfailedeventattributestypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef)
- [WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef)
- [DecisionTaskStartedEventAttributesTypeDef](./type_defs.md#decisiontaskstartedeventattributestypedef)
- [DecisionTaskTimedOutEventAttributesTypeDef](./type_defs.md#decisiontasktimedouteventattributestypedef)
- [FailWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#failworkflowexecutiondecisionattributestypedef)
- [RecordMarkerDecisionAttributesTypeDef](./type_defs.md#recordmarkerdecisionattributestypedef)
- [RequestCancelActivityTaskDecisionAttributesTypeDef](./type_defs.md#requestcancelactivitytaskdecisionattributestypedef)
- [RequestCancelExternalWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#requestcancelexternalworkflowexecutiondecisionattributestypedef)
- [ScheduleLambdaFunctionDecisionAttributesTypeDef](./type_defs.md#schedulelambdafunctiondecisionattributestypedef)
- [SignalExternalWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#signalexternalworkflowexecutiondecisionattributestypedef)
- [StartTimerDecisionAttributesTypeDef](./type_defs.md#starttimerdecisionattributestypedef)
- [DeprecateDomainInputRequestTypeDef](./type_defs.md#deprecatedomaininputrequesttypedef)
- [DescribeDomainInputRequestTypeDef](./type_defs.md#describedomaininputrequesttypedef)
- [DomainConfigurationTypeDef](./type_defs.md#domainconfigurationtypedef)
- [DomainInfoTypeDef](./type_defs.md#domaininfotypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [FailWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#failworkflowexecutionfailedeventattributestypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [LambdaFunctionCompletedEventAttributesTypeDef](./type_defs.md#lambdafunctioncompletedeventattributestypedef)
- [LambdaFunctionFailedEventAttributesTypeDef](./type_defs.md#lambdafunctionfailedeventattributestypedef)
- [LambdaFunctionScheduledEventAttributesTypeDef](./type_defs.md#lambdafunctionscheduledeventattributestypedef)
- [LambdaFunctionStartedEventAttributesTypeDef](./type_defs.md#lambdafunctionstartedeventattributestypedef)
- [LambdaFunctionTimedOutEventAttributesTypeDef](./type_defs.md#lambdafunctiontimedouteventattributestypedef)
- [MarkerRecordedEventAttributesTypeDef](./type_defs.md#markerrecordedeventattributestypedef)
- [RecordMarkerFailedEventAttributesTypeDef](./type_defs.md#recordmarkerfailedeventattributestypedef)
- [RequestCancelActivityTaskFailedEventAttributesTypeDef](./type_defs.md#requestcancelactivitytaskfailedeventattributestypedef)
- [RequestCancelExternalWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#requestcancelexternalworkflowexecutionfailedeventattributestypedef)
- [RequestCancelExternalWorkflowExecutionInitiatedEventAttributesTypeDef](./type_defs.md#requestcancelexternalworkflowexecutioninitiatedeventattributestypedef)
- [ScheduleLambdaFunctionFailedEventAttributesTypeDef](./type_defs.md#schedulelambdafunctionfailedeventattributestypedef)
- [SignalExternalWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#signalexternalworkflowexecutionfailedeventattributestypedef)
- [SignalExternalWorkflowExecutionInitiatedEventAttributesTypeDef](./type_defs.md#signalexternalworkflowexecutioninitiatedeventattributestypedef)
- [StartLambdaFunctionFailedEventAttributesTypeDef](./type_defs.md#startlambdafunctionfailedeventattributestypedef)
- [StartTimerFailedEventAttributesTypeDef](./type_defs.md#starttimerfailedeventattributestypedef)
- [TimerCanceledEventAttributesTypeDef](./type_defs.md#timercanceledeventattributestypedef)
- [TimerFiredEventAttributesTypeDef](./type_defs.md#timerfiredeventattributestypedef)
- [TimerStartedEventAttributesTypeDef](./type_defs.md#timerstartedeventattributestypedef)
- [WorkflowExecutionCanceledEventAttributesTypeDef](./type_defs.md#workflowexecutioncanceledeventattributestypedef)
- [WorkflowExecutionCompletedEventAttributesTypeDef](./type_defs.md#workflowexecutioncompletedeventattributestypedef)
- [WorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#workflowexecutionfailedeventattributestypedef)
- [WorkflowExecutionTerminatedEventAttributesTypeDef](./type_defs.md#workflowexecutionterminatedeventattributestypedef)
- [WorkflowExecutionTimedOutEventAttributesTypeDef](./type_defs.md#workflowexecutiontimedouteventattributestypedef)
- [ListActivityTypesInputRequestTypeDef](./type_defs.md#listactivitytypesinputrequesttypedef)
- [ListDomainsInputRequestTypeDef](./type_defs.md#listdomainsinputrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [ListWorkflowTypesInputRequestTypeDef](./type_defs.md#listworkflowtypesinputrequesttypedef)
- [RecordActivityTaskHeartbeatInputRequestTypeDef](./type_defs.md#recordactivitytaskheartbeatinputrequesttypedef)
- [RequestCancelWorkflowExecutionInputRequestTypeDef](./type_defs.md#requestcancelworkflowexecutioninputrequesttypedef)
- [RespondActivityTaskCanceledInputRequestTypeDef](./type_defs.md#respondactivitytaskcanceledinputrequesttypedef)
- [RespondActivityTaskCompletedInputRequestTypeDef](./type_defs.md#respondactivitytaskcompletedinputrequesttypedef)
- [RespondActivityTaskFailedInputRequestTypeDef](./type_defs.md#respondactivitytaskfailedinputrequesttypedef)
- [SignalWorkflowExecutionInputRequestTypeDef](./type_defs.md#signalworkflowexecutioninputrequesttypedef)
- [TerminateWorkflowExecutionInputRequestTypeDef](./type_defs.md#terminateworkflowexecutioninputrequesttypedef)
- [UndeprecateDomainInputRequestTypeDef](./type_defs.md#undeprecatedomaininputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [WorkflowExecutionOpenCountsTypeDef](./type_defs.md#workflowexecutionopencountstypedef)
- [ActivityTypeInfoTypeDef](./type_defs.md#activitytypeinfotypedef)
- [DeleteActivityTypeInputRequestTypeDef](./type_defs.md#deleteactivitytypeinputrequesttypedef)
- [DeprecateActivityTypeInputRequestTypeDef](./type_defs.md#deprecateactivitytypeinputrequesttypedef)
- [DescribeActivityTypeInputRequestTypeDef](./type_defs.md#describeactivitytypeinputrequesttypedef)
- [ScheduleActivityTaskFailedEventAttributesTypeDef](./type_defs.md#scheduleactivitytaskfailedeventattributestypedef)
- [UndeprecateActivityTypeInputRequestTypeDef](./type_defs.md#undeprecateactivitytypeinputrequesttypedef)
- [ActivityTaskScheduledEventAttributesTypeDef](./type_defs.md#activitytaskscheduledeventattributestypedef)
- [ActivityTypeConfigurationTypeDef](./type_defs.md#activitytypeconfigurationtypedef)
- [ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#continueasnewworkflowexecutiondecisionattributestypedef)
- [CountPendingActivityTasksInputRequestTypeDef](./type_defs.md#countpendingactivitytasksinputrequesttypedef)
- [CountPendingDecisionTasksInputRequestTypeDef](./type_defs.md#countpendingdecisiontasksinputrequesttypedef)
- [DecisionTaskCompletedEventAttributesTypeDef](./type_defs.md#decisiontaskcompletedeventattributestypedef)
- [DecisionTaskScheduledEventAttributesTypeDef](./type_defs.md#decisiontaskscheduledeventattributestypedef)
- [PollForActivityTaskInputRequestTypeDef](./type_defs.md#pollforactivitytaskinputrequesttypedef)
- [PollForDecisionTaskInputRequestTypeDef](./type_defs.md#pollfordecisiontaskinputrequesttypedef)
- [RegisterActivityTypeInputRequestTypeDef](./type_defs.md#registeractivitytypeinputrequesttypedef)
- [RegisterWorkflowTypeInputRequestTypeDef](./type_defs.md#registerworkflowtypeinputrequesttypedef)
- [ScheduleActivityTaskDecisionAttributesTypeDef](./type_defs.md#scheduleactivitytaskdecisionattributestypedef)
- [WorkflowExecutionConfigurationTypeDef](./type_defs.md#workflowexecutionconfigurationtypedef)
- [WorkflowTypeConfigurationTypeDef](./type_defs.md#workflowtypeconfigurationtypedef)
- [ActivityTaskStatusTypeDef](./type_defs.md#activitytaskstatustypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [PendingTaskCountTypeDef](./type_defs.md#pendingtaskcounttypedef)
- [RunTypeDef](./type_defs.md#runtypedef)
- [WorkflowExecutionCountTypeDef](./type_defs.md#workflowexecutioncounttypedef)
- [ActivityTaskTypeDef](./type_defs.md#activitytasktypedef)
- [DescribeWorkflowExecutionInputRequestTypeDef](./type_defs.md#describeworkflowexecutioninputrequesttypedef)
- [ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef](./type_defs.md#externalworkflowexecutioncancelrequestedeventattributestypedef)
- [ExternalWorkflowExecutionSignaledEventAttributesTypeDef](./type_defs.md#externalworkflowexecutionsignaledeventattributestypedef)
- [GetWorkflowExecutionHistoryInputRequestTypeDef](./type_defs.md#getworkflowexecutionhistoryinputrequesttypedef)
- [WorkflowExecutionCancelRequestedEventAttributesTypeDef](./type_defs.md#workflowexecutioncancelrequestedeventattributestypedef)
- [WorkflowExecutionSignaledEventAttributesTypeDef](./type_defs.md#workflowexecutionsignaledeventattributestypedef)
- [ChildWorkflowExecutionCanceledEventAttributesTypeDef](./type_defs.md#childworkflowexecutioncanceledeventattributestypedef)
- [ChildWorkflowExecutionCompletedEventAttributesTypeDef](./type_defs.md#childworkflowexecutioncompletedeventattributestypedef)
- [ChildWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#childworkflowexecutionfailedeventattributestypedef)
- [ChildWorkflowExecutionStartedEventAttributesTypeDef](./type_defs.md#childworkflowexecutionstartedeventattributestypedef)
- [ChildWorkflowExecutionTerminatedEventAttributesTypeDef](./type_defs.md#childworkflowexecutionterminatedeventattributestypedef)
- [ChildWorkflowExecutionTimedOutEventAttributesTypeDef](./type_defs.md#childworkflowexecutiontimedouteventattributestypedef)
- [DeleteWorkflowTypeInputRequestTypeDef](./type_defs.md#deleteworkflowtypeinputrequesttypedef)
- [DeprecateWorkflowTypeInputRequestTypeDef](./type_defs.md#deprecateworkflowtypeinputrequesttypedef)
- [DescribeWorkflowTypeInputRequestTypeDef](./type_defs.md#describeworkflowtypeinputrequesttypedef)
- [StartChildWorkflowExecutionDecisionAttributesTypeDef](./type_defs.md#startchildworkflowexecutiondecisionattributestypedef)
- [StartChildWorkflowExecutionFailedEventAttributesTypeDef](./type_defs.md#startchildworkflowexecutionfailedeventattributestypedef)
- [StartChildWorkflowExecutionInitiatedEventAttributesTypeDef](./type_defs.md#startchildworkflowexecutioninitiatedeventattributestypedef)
- [StartWorkflowExecutionInputRequestTypeDef](./type_defs.md#startworkflowexecutioninputrequesttypedef)
- [UndeprecateWorkflowTypeInputRequestTypeDef](./type_defs.md#undeprecateworkflowtypeinputrequesttypedef)
- [WorkflowExecutionContinuedAsNewEventAttributesTypeDef](./type_defs.md#workflowexecutioncontinuedasneweventattributestypedef)
- [WorkflowExecutionInfoTypeDef](./type_defs.md#workflowexecutioninfotypedef)
- [WorkflowExecutionStartedEventAttributesTypeDef](./type_defs.md#workflowexecutionstartedeventattributestypedef)
- [WorkflowTypeInfoTypeDef](./type_defs.md#workflowtypeinfotypedef)
- [DomainDetailTypeDef](./type_defs.md#domaindetailtypedef)
- [DomainInfosTypeDef](./type_defs.md#domaininfostypedef)
- [ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef)
- [GetWorkflowExecutionHistoryInputPaginateTypeDef](./type_defs.md#getworkflowexecutionhistoryinputpaginatetypedef)
- [ListActivityTypesInputPaginateTypeDef](./type_defs.md#listactivitytypesinputpaginatetypedef)
- [ListDomainsInputPaginateTypeDef](./type_defs.md#listdomainsinputpaginatetypedef)
- [ListWorkflowTypesInputPaginateTypeDef](./type_defs.md#listworkflowtypesinputpaginatetypedef)
- [PollForDecisionTaskInputPaginateTypeDef](./type_defs.md#pollfordecisiontaskinputpaginatetypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [RegisterDomainInputRequestTypeDef](./type_defs.md#registerdomaininputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [ActivityTypeInfosTypeDef](./type_defs.md#activitytypeinfostypedef)
- [ActivityTypeDetailTypeDef](./type_defs.md#activitytypedetailtypedef)
- [DecisionTypeDef](./type_defs.md#decisiontypedef)
- [WorkflowExecutionDetailTypeDef](./type_defs.md#workflowexecutiondetailtypedef)
- [WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef)
- [HistoryEventTypeDef](./type_defs.md#historyeventtypedef)
- [WorkflowTypeDetailTypeDef](./type_defs.md#workflowtypedetailtypedef)
- [WorkflowTypeInfosTypeDef](./type_defs.md#workflowtypeinfostypedef)
- [CountClosedWorkflowExecutionsInputRequestTypeDef](./type_defs.md#countclosedworkflowexecutionsinputrequesttypedef)
- [CountOpenWorkflowExecutionsInputRequestTypeDef](./type_defs.md#countopenworkflowexecutionsinputrequesttypedef)
- [ListClosedWorkflowExecutionsInputPaginateTypeDef](./type_defs.md#listclosedworkflowexecutionsinputpaginatetypedef)
- [ListClosedWorkflowExecutionsInputRequestTypeDef](./type_defs.md#listclosedworkflowexecutionsinputrequesttypedef)
- [ListOpenWorkflowExecutionsInputPaginateTypeDef](./type_defs.md#listopenworkflowexecutionsinputpaginatetypedef)
- [ListOpenWorkflowExecutionsInputRequestTypeDef](./type_defs.md#listopenworkflowexecutionsinputrequesttypedef)
- [RespondDecisionTaskCompletedInputRequestTypeDef](./type_defs.md#responddecisiontaskcompletedinputrequesttypedef)
- [DecisionTaskTypeDef](./type_defs.md#decisiontasktypedef)
- [HistoryTypeDef](./type_defs.md#historytypedef)
