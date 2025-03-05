# Examples

> [Index](../README.md) > [EKS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[eks]` package installed.

Write your `EKS` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# EKSClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("eks") as client:  # (1)
    result = await client.associate_access_policy()  # (2)
```

1. client: [EKSClient](./client.md)
2. result: [:material-code-braces: AssociateAccessPolicyResponseTypeDef](./type_defs.md#associateaccesspolicyresponsetypedef)



#### Paginator usage example

```python
# DescribeAddonVersionsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("eks") as client:  # (1)
    paginator = client.get_paginator("describe_addon_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
3. item: [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef)



#### Waiter usage example

```python
# AddonActiveWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("eks") as client:  # (1)
    waiter = client.get_waiter("addon_active")  # (2)
    await waiter.wait(...)
```

1. client: [EKSClient](./client.md)
2. waiter: [AddonActiveWaiter](./waiters.md#addonactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[eks]`
or a standalone `types_aiobotocore_eks` package, you have to explicitly specify
`client: EKSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# EKSClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.type_defs import AssociateAccessPolicyResponseTypeDef
from types_aiobotocore_eks.type_defs import AssociateAccessPolicyRequestTypeDef


session = Session()

client: EKSClient
async with session.client("eks") as client:  # (1)
    kwargs: AssociateAccessPolicyRequestTypeDef = {...}  # (2)
    result: AssociateAccessPolicyResponseTypeDef = await client.associate_access_policy(**kwargs)  # (3)
```

1. client: [EKSClient](./client.md)
2. kwargs: [:material-code-braces: AssociateAccessPolicyRequestTypeDef](./type_defs.md#associateaccesspolicyrequesttypedef)
3. result: [:material-code-braces: AssociateAccessPolicyResponseTypeDef](./type_defs.md#associateaccesspolicyresponsetypedef)



#### Paginator usage example

```python
# DescribeAddonVersionsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.paginator import DescribeAddonVersionsPaginator
from types_aiobotocore_eks.type_defs import DescribeAddonVersionsResponseTypeDef


session = Session()

client: EKSClient
async with session.client("eks") as client:  # (1)
    paginator: DescribeAddonVersionsPaginator = client.get_paginator("describe_addon_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddonVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
3. item: [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef)



#### Waiter usage example

```python
# AddonActiveWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.waiter import AddonActiveWaiter


session = Session()

async with session.client("eks") as client:  # (1)
    waiter = client.get_waiter("addon_active")  # (2)
    await waiter.wait(...)
```

1. client: [EKSClient](./client.md)
2. waiter: [AddonActiveWaiter](./waiters.md#addonactivewaiter)


