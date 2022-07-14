# Examples

> [Index](../README.md) > [CodePipeline](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
    type annotations stubs module [types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codepipeline]` package installed.

Write your `CodePipeline` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codepipeline") as client:  # (1)
        result = await client.acknowledge_job()  # (2)
    ```

    1. client: [CodePipelineClient](./client.md)
    2. result: [:material-code-braces: AcknowledgeJobOutputTypeDef](./type_defs.md#acknowledgejoboutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codepipeline") as client:  # (1)
        paginator = client.get_paginator("list_action_executions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CodePipelineClient](./client.md)
    2. paginator: [ListActionExecutionsPaginator](./paginators.md#listactionexecutionspaginator)
    3. item: [:material-code-braces: ListActionExecutionsOutputTypeDef](./type_defs.md#listactionexecutionsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[codepipeline]`
or a standalone `types_aiobotocore_codepipeline` package, you have to explicitly specify
`client: CodePipelineClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codepipeline.client import CodePipelineClient
    from types_aiobotocore_codepipeline.type_defs import AcknowledgeJobOutputTypeDef
    from types_aiobotocore_codepipeline.type_defs import AcknowledgeJobInputRequestTypeDef


    session = Session()

    client: CodePipelineClient
    async with session.client("codepipeline") as client:  # (1)
        kwargs: AcknowledgeJobInputRequestTypeDef = {...}  # (2)
        result: AcknowledgeJobOutputTypeDef = await client.acknowledge_job(**kwargs)  # (3)
    ```

    1. client: [CodePipelineClient](./client.md)
    2. kwargs: [:material-code-braces: AcknowledgeJobInputRequestTypeDef](./type_defs.md#acknowledgejobinputrequesttypedef) 
    3. result: [:material-code-braces: AcknowledgeJobOutputTypeDef](./type_defs.md#acknowledgejoboutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codepipeline.client import CodePipelineClient
    from types_aiobotocore_codepipeline.paginator import ListActionExecutionsPaginator
    from types_aiobotocore_codepipeline.type_defs import ListActionExecutionsOutputTypeDef


    session = Session()

    client: CodePipelineClient
    async with session.client("codepipeline") as client:  # (1)
        paginator: ListActionExecutionsPaginator = client.get_paginator("list_action_executions")  # (2)
        async for item in paginator.paginate(...):
            item: ListActionExecutionsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [CodePipelineClient](./client.md)
    2. paginator: [ListActionExecutionsPaginator](./paginators.md#listactionexecutionspaginator)
    3. item: [:material-code-braces: ListActionExecutionsOutputTypeDef](./type_defs.md#listactionexecutionsoutputtypedef) 




