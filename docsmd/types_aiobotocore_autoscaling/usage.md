# Examples

> [Index](../README.md) > [AutoScaling](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#autoscaling)
    type annotations stubs module [types-aiobotocore-autoscaling](https://pypi.org/project/types-aiobotocore-autoscaling/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[autoscaling]` package installed.

Write your `AutoScaling` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# AutoScalingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("autoscaling") as client:  # (1)
    result = await client.attach_instances()  # (2)
```

1. client: [AutoScalingClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribeAutoScalingGroupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("autoscaling") as client:  # (1)
    paginator = client.get_paginator("describe_auto_scaling_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeAutoScalingGroupsPaginator](./paginators.md#describeautoscalinggroupspaginator)
3. item: [:material-code-braces: AutoScalingGroupsTypeTypeDef](./type_defs.md#autoscalinggroupstypetypedef)




### Explicit type annotations

With `types-aioboto3-lite[autoscaling]`
or a standalone `types_aiobotocore_autoscaling` package, you have to explicitly specify
`client: AutoScalingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# AutoScalingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_autoscaling.client import AutoScalingClient
from types_aiobotocore_autoscaling.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_autoscaling.type_defs import AttachInstancesQueryTypeDef


session = Session()

client: AutoScalingClient
async with session.client("autoscaling") as client:  # (1)
    kwargs: AttachInstancesQueryTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.attach_instances(**kwargs)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. kwargs: [:material-code-braces: AttachInstancesQueryTypeDef](./type_defs.md#attachinstancesquerytypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# DescribeAutoScalingGroupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_autoscaling.client import AutoScalingClient
from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingGroupsPaginator
from types_aiobotocore_autoscaling.type_defs import AutoScalingGroupsTypeTypeDef


session = Session()

client: AutoScalingClient
async with session.client("autoscaling") as client:  # (1)
    paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")  # (2)
    async for item in paginator.paginate(...):
        item: AutoScalingGroupsTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeAutoScalingGroupsPaginator](./paginators.md#describeautoscalinggroupspaginator)
3. item: [:material-code-braces: AutoScalingGroupsTypeTypeDef](./type_defs.md#autoscalinggroupstypetypedef)




