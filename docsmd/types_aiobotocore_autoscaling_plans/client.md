# AutoScalingPlansClient

> [Index](../README.md) > [AutoScalingPlans](./README.md) > AutoScalingPlansClient

!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#autoscalingplans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## AutoScalingPlansClient

Type annotations and code completion for `#!python session.client("autoscaling-plans")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# AutoScalingPlansClient usage example

from aioboto3.session import Session
from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient

session = Session()
async with session.client("autoscaling-plans") as client:
    client: AutoScalingPlansClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("autoscaling-plans").exceptions` structure.

```python
# AutoScalingPlansClient.exceptions usage example

async with session.client("autoscaling-plans") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConcurrentUpdateException,
        client.exceptions.InternalServiceException,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.LimitExceededException,
        client.exceptions.ObjectNotFoundException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# AutoScalingPlansClient.exceptions type checking example

from types_aiobotocore_autoscaling_plans.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("autoscaling-plans").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("autoscaling-plans").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_scaling\_plan

Creates a scaling plan.

Type annotations and code completion for `#!python session.client("autoscaling-plans").create_scaling_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# create_scaling_plan method definition

await def create_scaling_plan(
    self,
    *,
    ScalingPlanName: str,
    ApplicationSource: ApplicationSourceTypeDef,  # (1)
    ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef],  # (2)
) -> CreateScalingPlanResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) [:material-code-braces: ScalingInstructionOutputTypeDef](./type_defs.md#scalinginstructionoutputtypedef) 
3. See [:material-code-braces: CreateScalingPlanResponseTypeDef](./type_defs.md#createscalingplanresponsetypedef) 


```python
# create_scaling_plan method usage example with argument unpacking

kwargs: CreateScalingPlanRequestRequestTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ApplicationSource": ...,
    "ScalingInstructions": ...,
}

parent.create_scaling_plan(**kwargs)
```

1. See [:material-code-braces: CreateScalingPlanRequestRequestTypeDef](./type_defs.md#createscalingplanrequestrequesttypedef) 

### delete\_scaling\_plan

Deletes the specified scaling plan.

Type annotations and code completion for `#!python session.client("autoscaling-plans").delete_scaling_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# delete_scaling_plan method definition

await def delete_scaling_plan(
    self,
    *,
    ScalingPlanName: str,
    ScalingPlanVersion: int,
) -> dict[str, Any]:
    ...
```



```python
# delete_scaling_plan method usage example with argument unpacking

kwargs: DeleteScalingPlanRequestRequestTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ScalingPlanVersion": ...,
}

parent.delete_scaling_plan(**kwargs)
```

1. See [:material-code-braces: DeleteScalingPlanRequestRequestTypeDef](./type_defs.md#deletescalingplanrequestrequesttypedef) 

### describe\_scaling\_plan\_resources

Describes the scalable resources in the specified scaling plan.

Type annotations and code completion for `#!python session.client("autoscaling-plans").describe_scaling_plan_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# describe_scaling_plan_resources method definition

await def describe_scaling_plan_resources(
    self,
    *,
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeScalingPlanResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef) 


```python
# describe_scaling_plan_resources method usage example with argument unpacking

kwargs: DescribeScalingPlanResourcesRequestRequestTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ScalingPlanVersion": ...,
}

parent.describe_scaling_plan_resources(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPlanResourcesRequestRequestTypeDef](./type_defs.md#describescalingplanresourcesrequestrequesttypedef) 

### describe\_scaling\_plans

Describes one or more of your scaling plans.

Type annotations and code completion for `#!python session.client("autoscaling-plans").describe_scaling_plans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# describe_scaling_plans method definition

await def describe_scaling_plans(
    self,
    *,
    ScalingPlanNames: Sequence[str] = ...,
    ScalingPlanVersion: int = ...,
    ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeScalingPlansResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef) 


```python
# describe_scaling_plans method usage example with argument unpacking

kwargs: DescribeScalingPlansRequestRequestTypeDef = {  # (1)
    "ScalingPlanNames": ...,
}

parent.describe_scaling_plans(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPlansRequestRequestTypeDef](./type_defs.md#describescalingplansrequestrequesttypedef) 

### get\_scaling\_plan\_resource\_forecast\_data

Retrieves the forecast data for a scalable resource.

Type annotations and code completion for `#!python session.client("autoscaling-plans").get_scaling_plan_resource_forecast_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# get_scaling_plan_resource_forecast_data method definition

await def get_scaling_plan_resource_forecast_data(
    self,
    *,
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    ForecastDataType: ForecastDataTypeType,  # (3)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
) -> GetScalingPlanResourceForecastDataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: ForecastDataTypeType](./literals.md#forecastdatatypetype) 
4. See [:material-code-braces: GetScalingPlanResourceForecastDataResponseTypeDef](./type_defs.md#getscalingplanresourceforecastdataresponsetypedef) 


```python
# get_scaling_plan_resource_forecast_data method usage example with argument unpacking

kwargs: GetScalingPlanResourceForecastDataRequestRequestTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ScalingPlanVersion": ...,
    "ServiceNamespace": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
    "ForecastDataType": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_scaling_plan_resource_forecast_data(**kwargs)
```

1. See [:material-code-braces: GetScalingPlanResourceForecastDataRequestRequestTypeDef](./type_defs.md#getscalingplanresourceforecastdatarequestrequesttypedef) 

### update\_scaling\_plan

Updates the specified scaling plan.

Type annotations and code completion for `#!python session.client("autoscaling-plans").update_scaling_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# update_scaling_plan method definition

await def update_scaling_plan(
    self,
    *,
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ApplicationSource: ApplicationSourceTypeDef = ...,  # (1)
    ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) 


```python
# update_scaling_plan method usage example with argument unpacking

kwargs: UpdateScalingPlanRequestRequestTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ScalingPlanVersion": ...,
}

parent.update_scaling_plan(**kwargs)
```

1. See [:material-code-braces: UpdateScalingPlanRequestRequestTypeDef](./type_defs.md#updatescalingplanrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("autoscaling-plans").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("autoscaling-plans").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("autoscaling-plans").get_paginator` method with overloads.

- `client.get_paginator("describe_scaling_plan_resources")` -> [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
- `client.get_paginator("describe_scaling_plans")` -> [DescribeScalingPlansPaginator](./paginators.md#describescalingplanspaginator)


