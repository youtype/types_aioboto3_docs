# Examples

> [Index](../README.md) > [KendraRanking](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KendraRanking](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#kendraranking)
    type annotations stubs module [types-aiobotocore-kendra-ranking](https://pypi.org/project/types-aiobotocore-kendra-ranking/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kendra-ranking]` package installed.

Write your `KendraRanking` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# KendraRankingClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("kendra-ranking") as client:  # (1)
    result = await client.create_rescore_execution_plan()  # (2)
```

1. client: [KendraRankingClient](./client.md)
2. result: [:material-code-braces: CreateRescoreExecutionPlanResponseTypeDef](./type_defs.md#createrescoreexecutionplanresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[kendra-ranking]`
or a standalone `types_aiobotocore_kendra_ranking` package, you have to explicitly specify
`client: KendraRankingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# KendraRankingClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_kendra_ranking.client import KendraRankingClient
from types_aiobotocore_kendra_ranking.type_defs import CreateRescoreExecutionPlanResponseTypeDef
from types_aiobotocore_kendra_ranking.type_defs import CreateRescoreExecutionPlanRequestTypeDef


session = Session()

client: KendraRankingClient
async with session.client("kendra-ranking") as client:  # (1)
    kwargs: CreateRescoreExecutionPlanRequestTypeDef = {...}  # (2)
    result: CreateRescoreExecutionPlanResponseTypeDef = await client.create_rescore_execution_plan(**kwargs)  # (3)
```

1. client: [KendraRankingClient](./client.md)
2. kwargs: [:material-code-braces: CreateRescoreExecutionPlanRequestTypeDef](./type_defs.md#createrescoreexecutionplanrequesttypedef)
3. result: [:material-code-braces: CreateRescoreExecutionPlanResponseTypeDef](./type_defs.md#createrescoreexecutionplanresponsetypedef)






