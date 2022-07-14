# Examples

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[autoscaling-plans]` package installed.

Write your `AutoScalingPlans` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("autoscaling-plans") as client:  # (1)
        result = await client.create_scaling_plan()  # (2)
    ```

    1. client: [AutoScalingPlansClient](./client.md)
    2. result: [:material-code-braces: CreateScalingPlanResponseTypeDef](./type_defs.md#createscalingplanresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("autoscaling-plans") as client:  # (1)
        paginator = client.get_paginator("describe_scaling_plan_resources")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AutoScalingPlansClient](./client.md)
    2. paginator: [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
    3. item: [:material-code-braces: DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[autoscaling-plans]`
or a standalone `types_aiobotocore_autoscaling_plans` package, you have to explicitly specify
`client: AutoScalingPlansClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient
    from types_aiobotocore_autoscaling_plans.type_defs import CreateScalingPlanResponseTypeDef
    from types_aiobotocore_autoscaling_plans.type_defs import CreateScalingPlanRequestRequestTypeDef


    session = Session()

    client: AutoScalingPlansClient
    async with session.client("autoscaling-plans") as client:  # (1)
        kwargs: CreateScalingPlanRequestRequestTypeDef = {...}  # (2)
        result: CreateScalingPlanResponseTypeDef = await client.create_scaling_plan(**kwargs)  # (3)
    ```

    1. client: [AutoScalingPlansClient](./client.md)
    2. kwargs: [:material-code-braces: CreateScalingPlanRequestRequestTypeDef](./type_defs.md#createscalingplanrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateScalingPlanResponseTypeDef](./type_defs.md#createscalingplanresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient
    from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator
    from types_aiobotocore_autoscaling_plans.type_defs import DescribeScalingPlanResourcesResponseTypeDef


    session = Session()

    client: AutoScalingPlansClient
    async with session.client("autoscaling-plans") as client:  # (1)
        paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeScalingPlanResourcesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [AutoScalingPlansClient](./client.md)
    2. paginator: [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
    3. item: [:material-code-braces: DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef) 




