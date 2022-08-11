# AutoScalingPlans module

> [Index](../README.md) > AutoScalingPlans


!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `AutoScalingPlans` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[autoscaling-plans]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[autoscaling-plans]'


# standalone installation
python -m pip install types-aiobotocore-autoscaling-plans
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-autoscaling-plans
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AutoScalingPlansClient

Type annotations and code completion for  `#!python session.client("autoscaling-plans")` as [AutoScalingPlansClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient


session = Session()
async with session.client("autoscaling-plans") as client:
    client: AutoScalingPlansClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("autoscaling-plans").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator

def get_describe_scaling_plan_resources_paginator() -> DescribeScalingPlanResourcesPaginator:
    return client.get_paginator("describe_scaling_plan_resources"))
```

- [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
- [DescribeScalingPlansPaginator](./paginators.md#describescalingplanspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_autoscaling_plans.literals import DescribeScalingPlanResourcesPaginatorName

def get_value() -> DescribeScalingPlanResourcesPaginatorName:
    return "describe_scaling_plan_resources"
```

- [DescribeScalingPlanResourcesPaginatorName](./literals.md#describescalingplanresourcespaginatorname)
- [DescribeScalingPlansPaginatorName](./literals.md#describescalingplanspaginatorname)
- [ForecastDataTypeType](./literals.md#forecastdatatypetype)
- [LoadMetricTypeType](./literals.md#loadmetrictypetype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [PolicyTypeType](./literals.md#policytypetype)
- [PredictiveScalingMaxCapacityBehaviorType](./literals.md#predictivescalingmaxcapacitybehaviortype)
- [PredictiveScalingModeType](./literals.md#predictivescalingmodetype)
- [ScalableDimensionType](./literals.md#scalabledimensiontype)
- [ScalingMetricTypeType](./literals.md#scalingmetrictypetype)
- [ScalingPlanStatusCodeType](./literals.md#scalingplanstatuscodetype)
- [ScalingPolicyUpdateBehaviorType](./literals.md#scalingpolicyupdatebehaviortype)
- [ScalingStatusCodeType](./literals.md#scalingstatuscodetype)
- [ServiceNamespaceType](./literals.md#servicenamespacetype)
- [AutoScalingPlansServiceName](./literals.md#autoscalingplansservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef

def get_value() -> TagFilterTypeDef:
    return {
        "Key": ...,
    }
```

- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef)
- [DatapointTypeDef](./type_defs.md#datapointtypedef)
- [DeleteScalingPlanRequestRequestTypeDef](./type_defs.md#deletescalingplanrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeScalingPlanResourcesRequestRequestTypeDef](./type_defs.md#describescalingplanresourcesrequestrequesttypedef)
- [GetScalingPlanResourceForecastDataRequestRequestTypeDef](./type_defs.md#getscalingplanresourceforecastdatarequestrequesttypedef)
- [PredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predefinedloadmetricspecificationtypedef)
- [PredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predefinedscalingmetricspecificationtypedef)
- [ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef)
- [CreateScalingPlanResponseTypeDef](./type_defs.md#createscalingplanresponsetypedef)
- [CustomizedLoadMetricSpecificationTypeDef](./type_defs.md#customizedloadmetricspecificationtypedef)
- [CustomizedScalingMetricSpecificationTypeDef](./type_defs.md#customizedscalingmetricspecificationtypedef)
- [GetScalingPlanResourceForecastDataResponseTypeDef](./type_defs.md#getscalingplanresourceforecastdataresponsetypedef)
- [DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef](./type_defs.md#describescalingplanresourcesrequestdescribescalingplanresourcespaginatetypedef)
- [DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef](./type_defs.md#describescalingplansrequestdescribescalingplanspaginatetypedef)
- [DescribeScalingPlansRequestRequestTypeDef](./type_defs.md#describescalingplansrequestrequesttypedef)
- [TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef)
- [ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef)
- [ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef)
- [CreateScalingPlanRequestRequestTypeDef](./type_defs.md#createscalingplanrequestrequesttypedef)
- [ScalingPlanTypeDef](./type_defs.md#scalingplantypedef)
- [UpdateScalingPlanRequestRequestTypeDef](./type_defs.md#updatescalingplanrequestrequesttypedef)
- [ScalingPlanResourceTypeDef](./type_defs.md#scalingplanresourcetypedef)
- [DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef)
- [DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef)

