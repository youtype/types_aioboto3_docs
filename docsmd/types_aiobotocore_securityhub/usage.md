# Examples

> [Index](../README.md) > [SecurityHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#securityhub)
    type annotations stubs module [types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[securityhub]` package installed.

Write your `SecurityHub` code as usual,
type checking and code completion should work out of the box.



```python
# SecurityHubClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("securityhub") as client:  # (1)
    result = await client.batch_delete_automation_rules()  # (2)
```

1. client: [SecurityHubClient](./client.md)
2. result: [:material-code-braces: BatchDeleteAutomationRulesResponseTypeDef](./type_defs.md#batchdeleteautomationrulesresponsetypedef) 



```python
# DescribeActionTargetsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("securityhub") as client:  # (1)
    paginator = client.get_paginator("describe_action_targets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeActionTargetsPaginator](./paginators.md#describeactiontargetspaginator)
3. item: [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[securityhub]`
or a standalone `types_aiobotocore_securityhub` package, you have to explicitly specify
`client: SecurityHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SecurityHubClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_securityhub.client import SecurityHubClient
from types_aiobotocore_securityhub.type_defs import BatchDeleteAutomationRulesResponseTypeDef
from types_aiobotocore_securityhub.type_defs import BatchDeleteAutomationRulesRequestRequestTypeDef


session = Session()

client: SecurityHubClient
async with session.client("securityhub") as client:  # (1)
    kwargs: BatchDeleteAutomationRulesRequestRequestTypeDef = {...}  # (2)
    result: BatchDeleteAutomationRulesResponseTypeDef = await client.batch_delete_automation_rules(**kwargs)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteAutomationRulesRequestRequestTypeDef](./type_defs.md#batchdeleteautomationrulesrequestrequesttypedef) 
3. result: [:material-code-braces: BatchDeleteAutomationRulesResponseTypeDef](./type_defs.md#batchdeleteautomationrulesresponsetypedef) 



```python
# DescribeActionTargetsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_securityhub.client import SecurityHubClient
from types_aiobotocore_securityhub.paginator import DescribeActionTargetsPaginator
from types_aiobotocore_securityhub.type_defs import DescribeActionTargetsResponseTypeDef


session = Session()

client: SecurityHubClient
async with session.client("securityhub") as client:  # (1)
    paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeActionTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecurityHubClient](./client.md)
2. paginator: [DescribeActionTargetsPaginator](./paginators.md#describeactiontargetspaginator)
3. item: [:material-code-braces: DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef) 



