# Examples

> [Index](../README.md) > [ConnectCases](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[connectcases]` package installed.

Write your `ConnectCases` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ConnectCasesClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectcases") as client:  # (1)
    result = await client.batch_get_case_rule()  # (2)
```

1. client: [ConnectCasesClient](./client.md)
2. result: [:material-code-braces: BatchGetCaseRuleResponseTypeDef](./type_defs.md#batchgetcaseruleresponsetypedef)



#### Paginator usage example

```python
# ListCaseRulesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("connectcases") as client:  # (1)
    paginator = client.get_paginator("list_case_rules")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [ListCaseRulesPaginator](./paginators.md#listcaserulespaginator)
3. item: [:material-code-braces: ListCaseRulesResponseTypeDef](./type_defs.md#listcaserulesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[connectcases]`
or a standalone `types_aiobotocore_connectcases` package, you have to explicitly specify
`client: ConnectCasesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ConnectCasesClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectcases.client import ConnectCasesClient
from types_aiobotocore_connectcases.type_defs import BatchGetCaseRuleResponseTypeDef
from types_aiobotocore_connectcases.type_defs import BatchGetCaseRuleRequestTypeDef


session = Session()

client: ConnectCasesClient
async with session.client("connectcases") as client:  # (1)
    kwargs: BatchGetCaseRuleRequestTypeDef = {...}  # (2)
    result: BatchGetCaseRuleResponseTypeDef = await client.batch_get_case_rule(**kwargs)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetCaseRuleRequestTypeDef](./type_defs.md#batchgetcaserulerequesttypedef)
3. result: [:material-code-braces: BatchGetCaseRuleResponseTypeDef](./type_defs.md#batchgetcaseruleresponsetypedef)



#### Paginator usage example

```python
# ListCaseRulesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connectcases.client import ConnectCasesClient
from types_aiobotocore_connectcases.paginator import ListCaseRulesPaginator
from types_aiobotocore_connectcases.type_defs import ListCaseRulesResponseTypeDef


session = Session()

client: ConnectCasesClient
async with session.client("connectcases") as client:  # (1)
    paginator: ListCaseRulesPaginator = client.get_paginator("list_case_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListCaseRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [ListCaseRulesPaginator](./paginators.md#listcaserulespaginator)
3. item: [:material-code-braces: ListCaseRulesResponseTypeDef](./type_defs.md#listcaserulesresponsetypedef)




