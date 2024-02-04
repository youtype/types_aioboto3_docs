# Paginators

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## DescribeScalingPlanResourcesPaginator

Type annotations and code completion for `#!python session.client("autoscaling-plans").get_paginator("describe_scaling_plan_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources)

```python
# DescribeScalingPlanResourcesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator

session = Session()

session = get_session()
async with session.client("autoscaling-plans") as client:  # (1)
    paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScalingPlanResourcesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingPlansClient](./client.md)
2. paginator: [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
3. item: [:material-code-braces: DescribeScalingPlanResourcesResponsePaginatorTypeDef](./type_defs.md#describescalingplanresourcesresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScalingPlanResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeScalingPlanResourcesResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeScalingPlanResourcesResponsePaginatorTypeDef](./type_defs.md#describescalingplanresourcesresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ScalingPlanVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef](./type_defs.md#describescalingplanresourcesrequestdescribescalingplanresourcespaginatetypedef) 
## DescribeScalingPlansPaginator

Type annotations and code completion for `#!python session.client("autoscaling-plans").get_paginator("describe_scaling_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans)

```python
# DescribeScalingPlansPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlansPaginator

session = Session()

session = get_session()
async with session.client("autoscaling-plans") as client:  # (1)
    paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScalingPlansResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingPlansClient](./client.md)
2. paginator: [DescribeScalingPlansPaginator](./paginators.md#describescalingplanspaginator)
3. item: [:material-code-braces: DescribeScalingPlansResponsePaginatorTypeDef](./type_defs.md#describescalingplansresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScalingPlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ScalingPlanNames: Sequence[str] = ...,
    ScalingPlanVersion: int = ...,
    ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeScalingPlansResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeScalingPlansResponsePaginatorTypeDef](./type_defs.md#describescalingplansresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = {  # (1)
    "ScalingPlanNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef](./type_defs.md#describescalingplansrequestdescribescalingplanspaginatetypedef) 
