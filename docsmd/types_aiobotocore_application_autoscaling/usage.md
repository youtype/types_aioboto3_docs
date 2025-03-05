# Examples

> [Index](../README.md) > [ApplicationAutoScaling](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#applicationautoscaling)
    type annotations stubs module [types-aiobotocore-application-autoscaling](https://pypi.org/project/types-aiobotocore-application-autoscaling/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[application-autoscaling]` package installed.

Write your `ApplicationAutoScaling` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ApplicationAutoScalingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("application-autoscaling") as client:  # (1)
    result = await client.describe_scalable_targets()  # (2)
```

1. client: [ApplicationAutoScalingClient](./client.md)
2. result: [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef)



#### Paginator usage example

```python
# DescribeScalableTargetsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("application-autoscaling") as client:  # (1)
    paginator = client.get_paginator("describe_scalable_targets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ApplicationAutoScalingClient](./client.md)
2. paginator: [DescribeScalableTargetsPaginator](./paginators.md#describescalabletargetspaginator)
3. item: [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[application-autoscaling]`
or a standalone `types_aiobotocore_application_autoscaling` package, you have to explicitly specify
`client: ApplicationAutoScalingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ApplicationAutoScalingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient
from types_aiobotocore_application_autoscaling.type_defs import DescribeScalableTargetsResponseTypeDef
from types_aiobotocore_application_autoscaling.type_defs import DescribeScalableTargetsRequestTypeDef


session = Session()

client: ApplicationAutoScalingClient
async with session.client("application-autoscaling") as client:  # (1)
    kwargs: DescribeScalableTargetsRequestTypeDef = {...}  # (2)
    result: DescribeScalableTargetsResponseTypeDef = await client.describe_scalable_targets(**kwargs)  # (3)
```

1. client: [ApplicationAutoScalingClient](./client.md)
2. kwargs: [:material-code-braces: DescribeScalableTargetsRequestTypeDef](./type_defs.md#describescalabletargetsrequesttypedef)
3. result: [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef)



#### Paginator usage example

```python
# DescribeScalableTargetsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient
from types_aiobotocore_application_autoscaling.paginator import DescribeScalableTargetsPaginator
from types_aiobotocore_application_autoscaling.type_defs import DescribeScalableTargetsResponseTypeDef


session = Session()

client: ApplicationAutoScalingClient
async with session.client("application-autoscaling") as client:  # (1)
    paginator: DescribeScalableTargetsPaginator = client.get_paginator("describe_scalable_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScalableTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationAutoScalingClient](./client.md)
2. paginator: [DescribeScalableTargetsPaginator](./paginators.md#describescalabletargetspaginator)
3. item: [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef)




