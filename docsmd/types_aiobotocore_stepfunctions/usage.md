# Examples

> [Index](../README.md) > [SFN](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
    type annotations stubs module [types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[stepfunctions]` package installed.

Write your `SFN` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("stepfunctions") as client:  # (1)
        result = await client.create_activity()  # (2)
    ```

    1. client: [SFNClient](./client.md)
    2. result: [:material-code-braces: CreateActivityOutputTypeDef](./type_defs.md#createactivityoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("stepfunctions") as client:  # (1)
        paginator = client.get_paginator("get_execution_history")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [SFNClient](./client.md)
    2. paginator: [GetExecutionHistoryPaginator](./paginators.md#getexecutionhistorypaginator)
    3. item: [:material-code-braces: GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[stepfunctions]`
or a standalone `types_aiobotocore_stepfunctions` package, you have to explicitly specify
`client: SFNClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_stepfunctions.client import SFNClient
    from types_aiobotocore_stepfunctions.type_defs import CreateActivityOutputTypeDef
    from types_aiobotocore_stepfunctions.type_defs import CreateActivityInputRequestTypeDef


    session = Session()

    client: SFNClient
    async with session.client("stepfunctions") as client:  # (1)
        kwargs: CreateActivityInputRequestTypeDef = {...}  # (2)
        result: CreateActivityOutputTypeDef = await client.create_activity(**kwargs)  # (3)
    ```

    1. client: [SFNClient](./client.md)
    2. kwargs: [:material-code-braces: CreateActivityInputRequestTypeDef](./type_defs.md#createactivityinputrequesttypedef) 
    3. result: [:material-code-braces: CreateActivityOutputTypeDef](./type_defs.md#createactivityoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_stepfunctions.client import SFNClient
    from types_aiobotocore_stepfunctions.paginator import GetExecutionHistoryPaginator
    from types_aiobotocore_stepfunctions.type_defs import GetExecutionHistoryOutputTypeDef


    session = Session()

    client: SFNClient
    async with session.client("stepfunctions") as client:  # (1)
        paginator: GetExecutionHistoryPaginator = client.get_paginator("get_execution_history")  # (2)
        async for item in paginator.paginate(...):
            item: GetExecutionHistoryOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [SFNClient](./client.md)
    2. paginator: [GetExecutionHistoryPaginator](./paginators.md#getexecutionhistorypaginator)
    3. item: [:material-code-braces: GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef) 




