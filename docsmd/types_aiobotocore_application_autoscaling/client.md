# ApplicationAutoScalingClient

> [Index](../README.md) > [ApplicationAutoScaling](./README.md) > ApplicationAutoScalingClient

!!! note ""

    Auto-generated documentation for [ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#applicationautoscaling)
    type annotations stubs module [types-aiobotocore-application-autoscaling](https://pypi.org/project/types-aiobotocore-application-autoscaling/).

## ApplicationAutoScalingClient

Type annotations and code completion for `#!python session.client("application-autoscaling")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# ApplicationAutoScalingClient usage example

from aioboto3.session import Session
from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient

session = Session()
async with session.client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("application-autoscaling").exceptions` structure.

```python
# ApplicationAutoScalingClient.exceptions usage example

async with session.client("application-autoscaling") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConcurrentUpdateException,
        client.exceptions.FailedResourceAccessException,
        client.exceptions.InternalServiceException,
        client.exceptions.InvalidNextTokenException,
        client.exceptions.LimitExceededException,
        client.exceptions.ObjectNotFoundException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.TooManyTagsException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# ApplicationAutoScalingClient.exceptions type checking example

from types_aiobotocore_application_autoscaling.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("application-autoscaling").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("application-autoscaling").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

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


### delete\_scaling\_policy

Deletes the specified scaling policy for an Application Auto Scaling scalable
target.

Type annotations and code completion for `#!python session.client("application-autoscaling").delete_scaling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# delete_scaling_policy method definition

await def delete_scaling_policy(
    self,
    *,
    PolicyName: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 


```python
# delete_scaling_policy method usage example with argument unpacking

kwargs: DeleteScalingPolicyRequestRequestTypeDef = {  # (1)
    "PolicyName": ...,
    "ServiceNamespace": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
}

parent.delete_scaling_policy(**kwargs)
```

1. See [:material-code-braces: DeleteScalingPolicyRequestRequestTypeDef](./type_defs.md#deletescalingpolicyrequestrequesttypedef) 

### delete\_scheduled\_action

Deletes the specified scheduled action for an Application Auto Scaling scalable
target.

Type annotations and code completion for `#!python session.client("application-autoscaling").delete_scheduled_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# delete_scheduled_action method definition

await def delete_scheduled_action(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionName: str,
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 


```python
# delete_scheduled_action method usage example with argument unpacking

kwargs: DeleteScheduledActionRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
    "ScheduledActionName": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
}

parent.delete_scheduled_action(**kwargs)
```

1. See [:material-code-braces: DeleteScheduledActionRequestRequestTypeDef](./type_defs.md#deletescheduledactionrequestrequesttypedef) 

### deregister\_scalable\_target

Deregisters an Application Auto Scaling scalable target when you have finished
using it.

Type annotations and code completion for `#!python session.client("application-autoscaling").deregister_scalable_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# deregister_scalable_target method definition

await def deregister_scalable_target(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 


```python
# deregister_scalable_target method usage example with argument unpacking

kwargs: DeregisterScalableTargetRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
}

parent.deregister_scalable_target(**kwargs)
```

1. See [:material-code-braces: DeregisterScalableTargetRequestRequestTypeDef](./type_defs.md#deregisterscalabletargetrequestrequesttypedef) 

### describe\_scalable\_targets

Gets information about the scalable targets in the specified namespace.

Type annotations and code completion for `#!python session.client("application-autoscaling").describe_scalable_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# describe_scalable_targets method definition

await def describe_scalable_targets(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceIds: Sequence[str] = ...,
    ScalableDimension: ScalableDimensionType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeScalableTargetsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef) 


```python
# describe_scalable_targets method usage example with argument unpacking

kwargs: DescribeScalableTargetsRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
}

parent.describe_scalable_targets(**kwargs)
```

1. See [:material-code-braces: DescribeScalableTargetsRequestRequestTypeDef](./type_defs.md#describescalabletargetsrequestrequesttypedef) 

### describe\_scaling\_activities

Provides descriptive information about the scaling activities in the specified
namespace from the previous six weeks.

Type annotations and code completion for `#!python session.client("application-autoscaling").describe_scaling_activities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# describe_scaling_activities method definition

await def describe_scaling_activities(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str = ...,
    ScalableDimension: ScalableDimensionType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
    IncludeNotScaledActivities: bool = ...,
) -> DescribeScalingActivitiesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: DescribeScalingActivitiesResponseTypeDef](./type_defs.md#describescalingactivitiesresponsetypedef) 


```python
# describe_scaling_activities method usage example with argument unpacking

kwargs: DescribeScalingActivitiesRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
}

parent.describe_scaling_activities(**kwargs)
```

1. See [:material-code-braces: DescribeScalingActivitiesRequestRequestTypeDef](./type_defs.md#describescalingactivitiesrequestrequesttypedef) 

### describe\_scaling\_policies

Describes the Application Auto Scaling scaling policies for the specified
service namespace.

Type annotations and code completion for `#!python session.client("application-autoscaling").describe_scaling_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# describe_scaling_policies method definition

await def describe_scaling_policies(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    PolicyNames: Sequence[str] = ...,
    ResourceId: str = ...,
    ScalableDimension: ScalableDimensionType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeScalingPoliciesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: DescribeScalingPoliciesResponseTypeDef](./type_defs.md#describescalingpoliciesresponsetypedef) 


```python
# describe_scaling_policies method usage example with argument unpacking

kwargs: DescribeScalingPoliciesRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
}

parent.describe_scaling_policies(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPoliciesRequestRequestTypeDef](./type_defs.md#describescalingpoliciesrequestrequesttypedef) 

### describe\_scheduled\_actions

Describes the Application Auto Scaling scheduled actions for the specified
service namespace.

Type annotations and code completion for `#!python session.client("application-autoscaling").describe_scheduled_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# describe_scheduled_actions method definition

await def describe_scheduled_actions(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionNames: Sequence[str] = ...,
    ResourceId: str = ...,
    ScalableDimension: ScalableDimensionType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeScheduledActionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: DescribeScheduledActionsResponseTypeDef](./type_defs.md#describescheduledactionsresponsetypedef) 


```python
# describe_scheduled_actions method usage example with argument unpacking

kwargs: DescribeScheduledActionsRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
}

parent.describe_scheduled_actions(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledActionsRequestRequestTypeDef](./type_defs.md#describescheduledactionsrequestrequesttypedef) 

### get\_predictive\_scaling\_forecast

Retrieves the forecast data for a predictive scaling policy.

Type annotations and code completion for `#!python session.client("application-autoscaling").get_predictive_scaling_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# get_predictive_scaling_forecast method definition

await def get_predictive_scaling_forecast(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    PolicyName: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
) -> GetPredictiveScalingForecastResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: GetPredictiveScalingForecastResponseTypeDef](./type_defs.md#getpredictivescalingforecastresponsetypedef) 


```python
# get_predictive_scaling_forecast method usage example with argument unpacking

kwargs: GetPredictiveScalingForecastRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
    "PolicyName": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_predictive_scaling_forecast(**kwargs)
```

1. See [:material-code-braces: GetPredictiveScalingForecastRequestRequestTypeDef](./type_defs.md#getpredictivescalingforecastrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns all the tags on the specified Application Auto Scaling scalable target.

Type annotations and code completion for `#!python session.client("application-autoscaling").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_scaling\_policy

Creates or updates a scaling policy for an Application Auto Scaling scalable
target.

Type annotations and code completion for `#!python session.client("application-autoscaling").put_scaling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# put_scaling_policy method definition

await def put_scaling_policy(
    self,
    *,
    PolicyName: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    PolicyType: PolicyTypeType = ...,  # (3)
    StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,  # (4)
    TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...,  # (5)
    PredictiveScalingPolicyConfiguration: PredictiveScalingPolicyConfigurationTypeDef = ...,  # (6)
) -> PutScalingPolicyResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
4. See [:material-code-braces: StepScalingPolicyConfigurationTypeDef](./type_defs.md#stepscalingpolicyconfigurationtypedef) 
5. See [:material-code-braces: TargetTrackingScalingPolicyConfigurationTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationtypedef) 
6. See [:material-code-braces: PredictiveScalingPolicyConfigurationTypeDef](./type_defs.md#predictivescalingpolicyconfigurationtypedef) 
7. See [:material-code-braces: PutScalingPolicyResponseTypeDef](./type_defs.md#putscalingpolicyresponsetypedef) 


```python
# put_scaling_policy method usage example with argument unpacking

kwargs: PutScalingPolicyRequestRequestTypeDef = {  # (1)
    "PolicyName": ...,
    "ServiceNamespace": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
}

parent.put_scaling_policy(**kwargs)
```

1. See [:material-code-braces: PutScalingPolicyRequestRequestTypeDef](./type_defs.md#putscalingpolicyrequestrequesttypedef) 

### put\_scheduled\_action

Creates or updates a scheduled action for an Application Auto Scaling scalable
target.

Type annotations and code completion for `#!python session.client("application-autoscaling").put_scheduled_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# put_scheduled_action method definition

await def put_scheduled_action(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionName: str,
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    Schedule: str = ...,
    Timezone: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    ScalableTargetAction: ScalableTargetActionTypeDef = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: ScalableTargetActionTypeDef](./type_defs.md#scalabletargetactiontypedef) 


```python
# put_scheduled_action method usage example with argument unpacking

kwargs: PutScheduledActionRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
    "ScheduledActionName": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
}

parent.put_scheduled_action(**kwargs)
```

1. See [:material-code-braces: PutScheduledActionRequestRequestTypeDef](./type_defs.md#putscheduledactionrequestrequesttypedef) 

### register\_scalable\_target

Registers or updates a scalable target, which is the resource that you want to
scale.

Type annotations and code completion for `#!python session.client("application-autoscaling").register_scalable_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# register_scalable_target method definition

await def register_scalable_target(
    self,
    *,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: int = ...,
    MaxCapacity: int = ...,
    RoleARN: str = ...,
    SuspendedState: SuspendedStateTypeDef = ...,  # (3)
    Tags: Mapping[str, str] = ...,
) -> RegisterScalableTargetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: SuspendedStateTypeDef](./type_defs.md#suspendedstatetypedef) 
4. See [:material-code-braces: RegisterScalableTargetResponseTypeDef](./type_defs.md#registerscalabletargetresponsetypedef) 


```python
# register_scalable_target method usage example with argument unpacking

kwargs: RegisterScalableTargetRequestRequestTypeDef = {  # (1)
    "ServiceNamespace": ...,
    "ResourceId": ...,
    "ScalableDimension": ...,
}

parent.register_scalable_target(**kwargs)
```

1. See [:material-code-braces: RegisterScalableTargetRequestRequestTypeDef](./type_defs.md#registerscalabletargetrequestrequesttypedef) 

### tag\_resource

Adds or edits tags on an Application Auto Scaling scalable target.

Type annotations and code completion for `#!python session.client("application-autoscaling").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes tags from an Application Auto Scaling scalable target.

Type annotations and code completion for `#!python session.client("application-autoscaling").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("application-autoscaling").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("application-autoscaling").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

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

Type annotations and code completion for `#!python session.client("application-autoscaling").get_paginator` method with overloads.

- `client.get_paginator("describe_scalable_targets")` -> [DescribeScalableTargetsPaginator](./paginators.md#describescalabletargetspaginator)
- `client.get_paginator("describe_scaling_activities")` -> [DescribeScalingActivitiesPaginator](./paginators.md#describescalingactivitiespaginator)
- `client.get_paginator("describe_scaling_policies")` -> [DescribeScalingPoliciesPaginator](./paginators.md#describescalingpoliciespaginator)
- `client.get_paginator("describe_scheduled_actions")` -> [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)


