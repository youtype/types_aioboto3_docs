# AutoScaling module

> [Index](../README.md) > AutoScaling


!!! note ""

    Auto-generated documentation for [AutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
    type annotations stubs module [types-aiobotocore-autoscaling](https://pypi.org/project/types-aiobotocore-autoscaling/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `AutoScaling`.

### From PyPI with pip

Install `types-aioboto3` for `AutoScaling` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[autoscaling]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[autoscaling]'


# standalone installation
python -m pip install types-aiobotocore-autoscaling
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-autoscaling
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AutoScalingClient

Type annotations and code completion for  `#!python session.client("autoscaling")` as [AutoScalingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_autoscaling.client import AutoScalingClient


session = Session()
async with session.client("autoscaling") as client:
    client: AutoScalingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("autoscaling").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingGroupsPaginator

def get_describe_auto_scaling_groups_paginator() -> DescribeAutoScalingGroupsPaginator:
    return client.get_paginator("describe_auto_scaling_groups"))
```

- [DescribeAutoScalingGroupsPaginator](./paginators.md#describeautoscalinggroupspaginator)
- [DescribeAutoScalingInstancesPaginator](./paginators.md#describeautoscalinginstancespaginator)
- [DescribeLaunchConfigurationsPaginator](./paginators.md#describelaunchconfigurationspaginator)
- [DescribeLoadBalancerTargetGroupsPaginator](./paginators.md#describeloadbalancertargetgroupspaginator)
- [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)
- [DescribeNotificationConfigurationsPaginator](./paginators.md#describenotificationconfigurationspaginator)
- [DescribePoliciesPaginator](./paginators.md#describepoliciespaginator)
- [DescribeScalingActivitiesPaginator](./paginators.md#describescalingactivitiespaginator)
- [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)
- [DescribeTagsPaginator](./paginators.md#describetagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_autoscaling.literals import AcceleratorManufacturerType

def get_value() -> AcceleratorManufacturerType:
    return "amazon-web-services"
```

- [AcceleratorManufacturerType](./literals.md#acceleratormanufacturertype)
- [AcceleratorNameType](./literals.md#acceleratornametype)
- [AcceleratorTypeType](./literals.md#acceleratortypetype)
- [BareMetalType](./literals.md#baremetaltype)
- [BurstablePerformanceType](./literals.md#burstableperformancetype)
- [CpuManufacturerType](./literals.md#cpumanufacturertype)
- [DescribeAutoScalingGroupsPaginatorName](./literals.md#describeautoscalinggroupspaginatorname)
- [DescribeAutoScalingInstancesPaginatorName](./literals.md#describeautoscalinginstancespaginatorname)
- [DescribeLaunchConfigurationsPaginatorName](./literals.md#describelaunchconfigurationspaginatorname)
- [DescribeLoadBalancerTargetGroupsPaginatorName](./literals.md#describeloadbalancertargetgroupspaginatorname)
- [DescribeLoadBalancersPaginatorName](./literals.md#describeloadbalancerspaginatorname)
- [DescribeNotificationConfigurationsPaginatorName](./literals.md#describenotificationconfigurationspaginatorname)
- [DescribePoliciesPaginatorName](./literals.md#describepoliciespaginatorname)
- [DescribeScalingActivitiesPaginatorName](./literals.md#describescalingactivitiespaginatorname)
- [DescribeScheduledActionsPaginatorName](./literals.md#describescheduledactionspaginatorname)
- [DescribeTagsPaginatorName](./literals.md#describetagspaginatorname)
- [InstanceGenerationType](./literals.md#instancegenerationtype)
- [InstanceMetadataEndpointStateType](./literals.md#instancemetadataendpointstatetype)
- [InstanceMetadataHttpTokensStateType](./literals.md#instancemetadatahttptokensstatetype)
- [InstanceRefreshStatusType](./literals.md#instancerefreshstatustype)
- [LifecycleStateType](./literals.md#lifecyclestatetype)
- [LocalStorageType](./literals.md#localstoragetype)
- [LocalStorageTypeType](./literals.md#localstoragetypetype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [MetricTypeType](./literals.md#metrictypetype)
- [PredefinedLoadMetricTypeType](./literals.md#predefinedloadmetrictypetype)
- [PredefinedMetricPairTypeType](./literals.md#predefinedmetricpairtypetype)
- [PredefinedScalingMetricTypeType](./literals.md#predefinedscalingmetrictypetype)
- [PredictiveScalingMaxCapacityBreachBehaviorType](./literals.md#predictivescalingmaxcapacitybreachbehaviortype)
- [PredictiveScalingModeType](./literals.md#predictivescalingmodetype)
- [RefreshStrategyType](./literals.md#refreshstrategytype)
- [ScalingActivityStatusCodeType](./literals.md#scalingactivitystatuscodetype)
- [WarmPoolStateType](./literals.md#warmpoolstatetype)
- [WarmPoolStatusType](./literals.md#warmpoolstatustype)
- [AutoScalingServiceName](./literals.md#autoscalingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_autoscaling.type_defs import AcceleratorCountRequestTypeDef

def get_value() -> AcceleratorCountRequestTypeDef:
    return {
        "Min": ...,
    }
```

- [AcceleratorCountRequestTypeDef](./type_defs.md#acceleratorcountrequesttypedef)
- [AcceleratorTotalMemoryMiBRequestTypeDef](./type_defs.md#acceleratortotalmemorymibrequesttypedef)
- [ActivityTypeDef](./type_defs.md#activitytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AdjustmentTypeTypeDef](./type_defs.md#adjustmenttypetypedef)
- [AlarmTypeDef](./type_defs.md#alarmtypedef)
- [AttachInstancesQueryRequestTypeDef](./type_defs.md#attachinstancesqueryrequesttypedef)
- [AttachLoadBalancerTargetGroupsTypeRequestTypeDef](./type_defs.md#attachloadbalancertargetgroupstyperequesttypedef)
- [AttachLoadBalancersTypeRequestTypeDef](./type_defs.md#attachloadbalancerstyperequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [EnabledMetricTypeDef](./type_defs.md#enabledmetrictypedef)
- [LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef)
- [SuspendedProcessTypeDef](./type_defs.md#suspendedprocesstypedef)
- [TagDescriptionTypeDef](./type_defs.md#tagdescriptiontypedef)
- [BaselineEbsBandwidthMbpsRequestTypeDef](./type_defs.md#baselineebsbandwidthmbpsrequesttypedef)
- [FailedScheduledUpdateGroupActionRequestTypeDef](./type_defs.md#failedscheduledupdategroupactionrequesttypedef)
- [BatchDeleteScheduledActionTypeRequestTypeDef](./type_defs.md#batchdeletescheduledactiontyperequesttypedef)
- [ScheduledUpdateGroupActionRequestTypeDef](./type_defs.md#scheduledupdategroupactionrequesttypedef)
- [EbsTypeDef](./type_defs.md#ebstypedef)
- [CancelInstanceRefreshTypeRequestTypeDef](./type_defs.md#cancelinstancerefreshtyperequesttypedef)
- [CapacityForecastTypeDef](./type_defs.md#capacityforecasttypedef)
- [CompleteLifecycleActionTypeRequestTypeDef](./type_defs.md#completelifecycleactiontyperequesttypedef)
- [LifecycleHookSpecificationTypeDef](./type_defs.md#lifecyclehookspecificationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef)
- [InstanceMonitoringTypeDef](./type_defs.md#instancemonitoringtypedef)
- [MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef)
- [DeleteAutoScalingGroupTypeRequestTypeDef](./type_defs.md#deleteautoscalinggrouptyperequesttypedef)
- [DeleteLifecycleHookTypeRequestTypeDef](./type_defs.md#deletelifecyclehooktyperequesttypedef)
- [DeleteNotificationConfigurationTypeRequestTypeDef](./type_defs.md#deletenotificationconfigurationtyperequesttypedef)
- [DeletePolicyTypeRequestTypeDef](./type_defs.md#deletepolicytyperequesttypedef)
- [DeleteScheduledActionTypeRequestTypeDef](./type_defs.md#deletescheduledactiontyperequesttypedef)
- [DeleteWarmPoolTypeRequestTypeDef](./type_defs.md#deletewarmpooltyperequesttypedef)
- [DescribeAutoScalingInstancesTypeRequestTypeDef](./type_defs.md#describeautoscalinginstancestyperequesttypedef)
- [DescribeInstanceRefreshesTypeRequestTypeDef](./type_defs.md#describeinstancerefreshestyperequesttypedef)
- [LifecycleHookTypeDef](./type_defs.md#lifecyclehooktypedef)
- [DescribeLifecycleHooksTypeRequestTypeDef](./type_defs.md#describelifecyclehookstyperequesttypedef)
- [DescribeLoadBalancerTargetGroupsRequestRequestTypeDef](./type_defs.md#describeloadbalancertargetgroupsrequestrequesttypedef)
- [LoadBalancerTargetGroupStateTypeDef](./type_defs.md#loadbalancertargetgroupstatetypedef)
- [DescribeLoadBalancersRequestRequestTypeDef](./type_defs.md#describeloadbalancersrequestrequesttypedef)
- [LoadBalancerStateTypeDef](./type_defs.md#loadbalancerstatetypedef)
- [MetricCollectionTypeTypeDef](./type_defs.md#metriccollectiontypetypedef)
- [MetricGranularityTypeTypeDef](./type_defs.md#metricgranularitytypetypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [DescribeNotificationConfigurationsTypeRequestTypeDef](./type_defs.md#describenotificationconfigurationstyperequesttypedef)
- [DescribePoliciesTypeRequestTypeDef](./type_defs.md#describepoliciestyperequesttypedef)
- [DescribeScalingActivitiesTypeRequestTypeDef](./type_defs.md#describescalingactivitiestyperequesttypedef)
- [DescribeScheduledActionsTypeRequestTypeDef](./type_defs.md#describescheduledactionstyperequesttypedef)
- [DescribeWarmPoolTypeRequestTypeDef](./type_defs.md#describewarmpooltyperequesttypedef)
- [DetachInstancesQueryRequestTypeDef](./type_defs.md#detachinstancesqueryrequesttypedef)
- [DetachLoadBalancerTargetGroupsTypeRequestTypeDef](./type_defs.md#detachloadbalancertargetgroupstyperequesttypedef)
- [DetachLoadBalancersTypeRequestTypeDef](./type_defs.md#detachloadbalancerstyperequesttypedef)
- [DisableMetricsCollectionQueryRequestTypeDef](./type_defs.md#disablemetricscollectionqueryrequesttypedef)
- [EnableMetricsCollectionQueryRequestTypeDef](./type_defs.md#enablemetricscollectionqueryrequesttypedef)
- [EnterStandbyQueryRequestTypeDef](./type_defs.md#enterstandbyqueryrequesttypedef)
- [ExecutePolicyTypeRequestTypeDef](./type_defs.md#executepolicytyperequesttypedef)
- [ExitStandbyQueryRequestTypeDef](./type_defs.md#exitstandbyqueryrequesttypedef)
- [GetPredictiveScalingForecastTypeRequestTypeDef](./type_defs.md#getpredictivescalingforecasttyperequesttypedef)
- [InstanceRefreshLivePoolProgressTypeDef](./type_defs.md#instancerefreshlivepoolprogresstypedef)
- [InstanceRefreshWarmPoolProgressTypeDef](./type_defs.md#instancerefreshwarmpoolprogresstypedef)
- [RefreshPreferencesTypeDef](./type_defs.md#refreshpreferencestypedef)
- [MemoryGiBPerVCpuRequestTypeDef](./type_defs.md#memorygibpervcpurequesttypedef)
- [MemoryMiBRequestTypeDef](./type_defs.md#memorymibrequesttypedef)
- [NetworkInterfaceCountRequestTypeDef](./type_defs.md#networkinterfacecountrequesttypedef)
- [TotalLocalStorageGBRequestTypeDef](./type_defs.md#totallocalstoragegbrequesttypedef)
- [VCpuCountRequestTypeDef](./type_defs.md#vcpucountrequesttypedef)
- [InstanceReusePolicyTypeDef](./type_defs.md#instancereusepolicytypedef)
- [InstancesDistributionTypeDef](./type_defs.md#instancesdistributiontypedef)
- [LaunchConfigurationNameTypeRequestTypeDef](./type_defs.md#launchconfigurationnametyperequesttypedef)
- [LaunchConfigurationNamesTypeRequestTypeDef](./type_defs.md#launchconfigurationnamestyperequesttypedef)
- [PredefinedMetricSpecificationTypeDef](./type_defs.md#predefinedmetricspecificationtypedef)
- [PredictiveScalingPredefinedLoadMetricTypeDef](./type_defs.md#predictivescalingpredefinedloadmetrictypedef)
- [PredictiveScalingPredefinedMetricPairTypeDef](./type_defs.md#predictivescalingpredefinedmetricpairtypedef)
- [PredictiveScalingPredefinedScalingMetricTypeDef](./type_defs.md#predictivescalingpredefinedscalingmetrictypedef)
- [ProcessTypeTypeDef](./type_defs.md#processtypetypedef)
- [PutLifecycleHookTypeRequestTypeDef](./type_defs.md#putlifecyclehooktyperequesttypedef)
- [PutNotificationConfigurationTypeRequestTypeDef](./type_defs.md#putnotificationconfigurationtyperequesttypedef)
- [StepAdjustmentTypeDef](./type_defs.md#stepadjustmenttypedef)
- [PutScheduledUpdateGroupActionTypeRequestTypeDef](./type_defs.md#putscheduledupdategroupactiontyperequesttypedef)
- [RecordLifecycleActionHeartbeatTypeRequestTypeDef](./type_defs.md#recordlifecycleactionheartbeattyperequesttypedef)
- [ScalingProcessQueryRequestTypeDef](./type_defs.md#scalingprocessqueryrequesttypedef)
- [ScheduledUpdateGroupActionTypeDef](./type_defs.md#scheduledupdategroupactiontypedef)
- [SetDesiredCapacityTypeRequestTypeDef](./type_defs.md#setdesiredcapacitytyperequesttypedef)
- [SetInstanceHealthQueryRequestTypeDef](./type_defs.md#setinstancehealthqueryrequesttypedef)
- [SetInstanceProtectionQueryRequestTypeDef](./type_defs.md#setinstanceprotectionqueryrequesttypedef)
- [TerminateInstanceInAutoScalingGroupTypeRequestTypeDef](./type_defs.md#terminateinstanceinautoscalinggrouptyperequesttypedef)
- [ActivitiesTypeTypeDef](./type_defs.md#activitiestypetypedef)
- [ActivityTypeTypeDef](./type_defs.md#activitytypetypedef)
- [CancelInstanceRefreshAnswerTypeDef](./type_defs.md#cancelinstancerefreshanswertypedef)
- [DescribeAccountLimitsAnswerTypeDef](./type_defs.md#describeaccountlimitsanswertypedef)
- [DescribeAutoScalingNotificationTypesAnswerTypeDef](./type_defs.md#describeautoscalingnotificationtypesanswertypedef)
- [DescribeLifecycleHookTypesAnswerTypeDef](./type_defs.md#describelifecyclehooktypesanswertypedef)
- [DescribeTerminationPolicyTypesAnswerTypeDef](./type_defs.md#describeterminationpolicytypesanswertypedef)
- [DetachInstancesAnswerTypeDef](./type_defs.md#detachinstancesanswertypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EnterStandbyAnswerTypeDef](./type_defs.md#enterstandbyanswertypedef)
- [ExitStandbyAnswerTypeDef](./type_defs.md#exitstandbyanswertypedef)
- [StartInstanceRefreshAnswerTypeDef](./type_defs.md#startinstancerefreshanswertypedef)
- [DescribeAdjustmentTypesAnswerTypeDef](./type_defs.md#describeadjustmenttypesanswertypedef)
- [PolicyARNTypeTypeDef](./type_defs.md#policyarntypetypedef)
- [AutoScalingGroupNamesTypeRequestTypeDef](./type_defs.md#autoscalinggroupnamestyperequesttypedef)
- [DescribeTagsTypeRequestTypeDef](./type_defs.md#describetagstyperequesttypedef)
- [AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef](./type_defs.md#autoscalinggroupnamestypedescribeautoscalinggroupspaginatetypedef)
- [DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef](./type_defs.md#describeautoscalinginstancestypedescribeautoscalinginstancespaginatetypedef)
- [DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef](./type_defs.md#describeloadbalancertargetgroupsrequestdescribeloadbalancertargetgroupspaginatetypedef)
- [DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef](./type_defs.md#describeloadbalancersrequestdescribeloadbalancerspaginatetypedef)
- [DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef](./type_defs.md#describenotificationconfigurationstypedescribenotificationconfigurationspaginatetypedef)
- [DescribePoliciesTypeDescribePoliciesPaginateTypeDef](./type_defs.md#describepoliciestypedescribepoliciespaginatetypedef)
- [DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef](./type_defs.md#describescalingactivitiestypedescribescalingactivitiespaginatetypedef)
- [DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef](./type_defs.md#describescheduledactionstypedescribescheduledactionspaginatetypedef)
- [DescribeTagsTypeDescribeTagsPaginateTypeDef](./type_defs.md#describetagstypedescribetagspaginatetypedef)
- [LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef](./type_defs.md#launchconfigurationnamestypedescribelaunchconfigurationspaginatetypedef)
- [AutoScalingInstanceDetailsTypeDef](./type_defs.md#autoscalinginstancedetailstypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [TagsTypeTypeDef](./type_defs.md#tagstypetypedef)
- [BatchDeleteScheduledActionAnswerTypeDef](./type_defs.md#batchdeletescheduledactionanswertypedef)
- [BatchPutScheduledUpdateGroupActionAnswerTypeDef](./type_defs.md#batchputscheduledupdategroupactionanswertypedef)
- [BatchPutScheduledUpdateGroupActionTypeRequestTypeDef](./type_defs.md#batchputscheduledupdategroupactiontyperequesttypedef)
- [BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef)
- [CreateOrUpdateTagsTypeRequestTypeDef](./type_defs.md#createorupdatetagstyperequesttypedef)
- [DeleteTagsTypeRequestTypeDef](./type_defs.md#deletetagstyperequesttypedef)
- [CustomizedMetricSpecificationTypeDef](./type_defs.md#customizedmetricspecificationtypedef)
- [MetricTypeDef](./type_defs.md#metrictypedef)
- [DescribeLifecycleHooksAnswerTypeDef](./type_defs.md#describelifecyclehooksanswertypedef)
- [DescribeLoadBalancerTargetGroupsResponseTypeDef](./type_defs.md#describeloadbalancertargetgroupsresponsetypedef)
- [DescribeLoadBalancersResponseTypeDef](./type_defs.md#describeloadbalancersresponsetypedef)
- [DescribeMetricCollectionTypesAnswerTypeDef](./type_defs.md#describemetriccollectiontypesanswertypedef)
- [DescribeNotificationConfigurationsAnswerTypeDef](./type_defs.md#describenotificationconfigurationsanswertypedef)
- [InstanceRefreshProgressDetailsTypeDef](./type_defs.md#instancerefreshprogressdetailstypedef)
- [InstanceRequirementsTypeDef](./type_defs.md#instancerequirementstypedef)
- [PutWarmPoolTypeRequestTypeDef](./type_defs.md#putwarmpooltyperequesttypedef)
- [WarmPoolConfigurationTypeDef](./type_defs.md#warmpoolconfigurationtypedef)
- [ProcessesTypeTypeDef](./type_defs.md#processestypetypedef)
- [ScheduledActionsTypeTypeDef](./type_defs.md#scheduledactionstypetypedef)
- [AutoScalingInstancesTypeTypeDef](./type_defs.md#autoscalinginstancestypetypedef)
- [CreateLaunchConfigurationTypeRequestTypeDef](./type_defs.md#createlaunchconfigurationtyperequesttypedef)
- [LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef)
- [TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef)
- [MetricStatTypeDef](./type_defs.md#metricstattypedef)
- [LaunchTemplateOverridesTypeDef](./type_defs.md#launchtemplateoverridestypedef)
- [DescribeWarmPoolAnswerTypeDef](./type_defs.md#describewarmpoolanswertypedef)
- [LaunchConfigurationsTypeTypeDef](./type_defs.md#launchconfigurationstypetypedef)
- [MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef)
- [LaunchTemplateTypeDef](./type_defs.md#launchtemplatetypedef)
- [PredictiveScalingCustomizedCapacityMetricTypeDef](./type_defs.md#predictivescalingcustomizedcapacitymetrictypedef)
- [PredictiveScalingCustomizedLoadMetricTypeDef](./type_defs.md#predictivescalingcustomizedloadmetrictypedef)
- [PredictiveScalingCustomizedScalingMetricTypeDef](./type_defs.md#predictivescalingcustomizedscalingmetrictypedef)
- [MixedInstancesPolicyTypeDef](./type_defs.md#mixedinstancespolicytypedef)
- [PredictiveScalingMetricSpecificationTypeDef](./type_defs.md#predictivescalingmetricspecificationtypedef)
- [AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef)
- [CreateAutoScalingGroupTypeRequestTypeDef](./type_defs.md#createautoscalinggrouptyperequesttypedef)
- [DesiredConfigurationTypeDef](./type_defs.md#desiredconfigurationtypedef)
- [UpdateAutoScalingGroupTypeRequestTypeDef](./type_defs.md#updateautoscalinggrouptyperequesttypedef)
- [LoadForecastTypeDef](./type_defs.md#loadforecasttypedef)
- [PredictiveScalingConfigurationTypeDef](./type_defs.md#predictivescalingconfigurationtypedef)
- [AutoScalingGroupsTypeTypeDef](./type_defs.md#autoscalinggroupstypetypedef)
- [InstanceRefreshTypeDef](./type_defs.md#instancerefreshtypedef)
- [StartInstanceRefreshTypeRequestTypeDef](./type_defs.md#startinstancerefreshtyperequesttypedef)
- [GetPredictiveScalingForecastAnswerTypeDef](./type_defs.md#getpredictivescalingforecastanswertypedef)
- [PutScalingPolicyTypeRequestTypeDef](./type_defs.md#putscalingpolicytyperequesttypedef)
- [ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef)
- [DescribeInstanceRefreshesAnswerTypeDef](./type_defs.md#describeinstancerefreshesanswertypedef)
- [PoliciesTypeTypeDef](./type_defs.md#policiestypetypedef)

