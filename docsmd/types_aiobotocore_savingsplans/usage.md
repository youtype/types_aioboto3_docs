# Examples

> [Index](../README.md) > [SavingsPlans](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#savingsplans)
    type annotations stubs module [types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[savingsplans]` package installed.

Write your `SavingsPlans` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SavingsPlansClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("savingsplans") as client:  # (1)
    result = await client.create_savings_plan()  # (2)
```

1. client: [SavingsPlansClient](./client.md)
2. result: [:material-code-braces: CreateSavingsPlanResponseTypeDef](./type_defs.md#createsavingsplanresponsetypedef)






### Explicit type annotations

With `types-aioboto3-lite[savingsplans]`
or a standalone `types_aiobotocore_savingsplans` package, you have to explicitly specify
`client: SavingsPlansClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SavingsPlansClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_savingsplans.client import SavingsPlansClient
from types_aiobotocore_savingsplans.type_defs import CreateSavingsPlanResponseTypeDef
from types_aiobotocore_savingsplans.type_defs import CreateSavingsPlanRequestTypeDef


session = Session()

client: SavingsPlansClient
async with session.client("savingsplans") as client:  # (1)
    kwargs: CreateSavingsPlanRequestTypeDef = {...}  # (2)
    result: CreateSavingsPlanResponseTypeDef = await client.create_savings_plan(**kwargs)  # (3)
```

1. client: [SavingsPlansClient](./client.md)
2. kwargs: [:material-code-braces: CreateSavingsPlanRequestTypeDef](./type_defs.md#createsavingsplanrequesttypedef)
3. result: [:material-code-braces: CreateSavingsPlanResponseTypeDef](./type_defs.md#createsavingsplanresponsetypedef)






