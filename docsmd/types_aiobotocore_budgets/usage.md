# Examples

> [Index](../README.md) > [Budgets](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
    type annotations stubs module [types-aiobotocore-budgets](https://pypi.org/project/types-aiobotocore-budgets/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[budgets]` package installed.

Write your `Budgets` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("budgets") as client:  # (1)
        result = await client.create_budget_action()  # (2)
    ```

    1. client: [BudgetsClient](./client.md)
    2. result: [:material-code-braces: CreateBudgetActionResponseTypeDef](./type_defs.md#createbudgetactionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("budgets") as client:  # (1)
        paginator = client.get_paginator("describe_budget_action_histories")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [BudgetsClient](./client.md)
    2. paginator: [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
    3. item: [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[budgets]`
or a standalone `types_aiobotocore_budgets` package, you have to explicitly specify
`client: BudgetsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_budgets.client import BudgetsClient
    from types_aiobotocore_budgets.type_defs import CreateBudgetActionResponseTypeDef
    from types_aiobotocore_budgets.type_defs import CreateBudgetActionRequestRequestTypeDef


    session = Session()

    client: BudgetsClient
    async with session.client("budgets") as client:  # (1)
        kwargs: CreateBudgetActionRequestRequestTypeDef = {...}  # (2)
        result: CreateBudgetActionResponseTypeDef = await client.create_budget_action(**kwargs)  # (3)
    ```

    1. client: [BudgetsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateBudgetActionRequestRequestTypeDef](./type_defs.md#createbudgetactionrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateBudgetActionResponseTypeDef](./type_defs.md#createbudgetactionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_budgets.client import BudgetsClient
    from types_aiobotocore_budgets.paginator import DescribeBudgetActionHistoriesPaginator
    from types_aiobotocore_budgets.type_defs import DescribeBudgetActionHistoriesResponseTypeDef


    session = Session()

    client: BudgetsClient
    async with session.client("budgets") as client:  # (1)
        paginator: DescribeBudgetActionHistoriesPaginator = client.get_paginator("describe_budget_action_histories")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeBudgetActionHistoriesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [BudgetsClient](./client.md)
    2. paginator: [DescribeBudgetActionHistoriesPaginator](./paginators.md#describebudgetactionhistoriespaginator)
    3. item: [:material-code-braces: DescribeBudgetActionHistoriesResponseTypeDef](./type_defs.md#describebudgetactionhistoriesresponsetypedef) 




