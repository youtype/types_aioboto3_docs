# Examples

> [Index](../README.md) > [SSM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#ssm)
    type annotations stubs module [types-aiobotocore-ssm](https://pypi.org/project/types-aiobotocore-ssm/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ssm]` package installed.

Write your `SSM` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SSMClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm") as client:  # (1)
    result = await client.associate_ops_item_related_item()  # (2)
```

1. client: [SSMClient](./client.md)
2. result: [:material-code-braces: AssociateOpsItemRelatedItemResponseTypeDef](./type_defs.md#associateopsitemrelateditemresponsetypedef)



#### Paginator usage example

```python
# DescribeActivationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm") as client:  # (1)
    paginator = client.get_paginator("describe_activations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SSMClient](./client.md)
2. paginator: [DescribeActivationsPaginator](./paginators.md#describeactivationspaginator)
3. item: [:material-code-braces: DescribeActivationsResultTypeDef](./type_defs.md#describeactivationsresulttypedef)



#### Waiter usage example

```python
# CommandExecutedWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm") as client:  # (1)
    waiter = client.get_waiter("command_executed")  # (2)
    await waiter.wait(...)
```

1. client: [SSMClient](./client.md)
2. waiter: [CommandExecutedWaiter](./waiters.md#commandexecutedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[ssm]`
or a standalone `types_aiobotocore_ssm` package, you have to explicitly specify
`client: SSMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SSMClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.type_defs import AssociateOpsItemRelatedItemResponseTypeDef
from types_aiobotocore_ssm.type_defs import AssociateOpsItemRelatedItemRequestTypeDef


session = Session()

client: SSMClient
async with session.client("ssm") as client:  # (1)
    kwargs: AssociateOpsItemRelatedItemRequestTypeDef = {...}  # (2)
    result: AssociateOpsItemRelatedItemResponseTypeDef = await client.associate_ops_item_related_item(**kwargs)  # (3)
```

1. client: [SSMClient](./client.md)
2. kwargs: [:material-code-braces: AssociateOpsItemRelatedItemRequestTypeDef](./type_defs.md#associateopsitemrelateditemrequesttypedef)
3. result: [:material-code-braces: AssociateOpsItemRelatedItemResponseTypeDef](./type_defs.md#associateopsitemrelateditemresponsetypedef)



#### Paginator usage example

```python
# DescribeActivationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.paginator import DescribeActivationsPaginator
from types_aiobotocore_ssm.type_defs import DescribeActivationsResultTypeDef


session = Session()

client: SSMClient
async with session.client("ssm") as client:  # (1)
    paginator: DescribeActivationsPaginator = client.get_paginator("describe_activations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeActivationsResultTypeDef
        print(item)  # (3)
```

1. client: [SSMClient](./client.md)
2. paginator: [DescribeActivationsPaginator](./paginators.md#describeactivationspaginator)
3. item: [:material-code-braces: DescribeActivationsResultTypeDef](./type_defs.md#describeactivationsresulttypedef)



#### Waiter usage example

```python
# CommandExecutedWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm.client import SSMClient
from types_aiobotocore_ssm.waiter import CommandExecutedWaiter


session = Session()

async with session.client("ssm") as client:  # (1)
    waiter = client.get_waiter("command_executed")  # (2)
    await waiter.wait(...)
```

1. client: [SSMClient](./client.md)
2. waiter: [CommandExecutedWaiter](./waiters.md#commandexecutedwaiter)


