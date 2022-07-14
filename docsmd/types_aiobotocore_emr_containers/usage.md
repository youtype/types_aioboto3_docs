# Examples

> [Index](../README.md) > [EMRContainers](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[emr-containers]` package installed.

Write your `EMRContainers` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("emr-containers") as client:  # (1)
        result = await client.cancel_job_run()  # (2)
    ```

    1. client: [EMRContainersClient](./client.md)
    2. result: [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("emr-containers") as client:  # (1)
        paginator = client.get_paginator("list_job_runs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [EMRContainersClient](./client.md)
    2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
    3. item: [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[emr-containers]`
or a standalone `types_aiobotocore_emr_containers` package, you have to explicitly specify
`client: EMRContainersClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_emr_containers.client import EMRContainersClient
    from types_aiobotocore_emr_containers.type_defs import CancelJobRunResponseTypeDef
    from types_aiobotocore_emr_containers.type_defs import CancelJobRunRequestRequestTypeDef


    session = Session()

    client: EMRContainersClient
    async with session.client("emr-containers") as client:  # (1)
        kwargs: CancelJobRunRequestRequestTypeDef = {...}  # (2)
        result: CancelJobRunResponseTypeDef = await client.cancel_job_run(**kwargs)  # (3)
    ```

    1. client: [EMRContainersClient](./client.md)
    2. kwargs: [:material-code-braces: CancelJobRunRequestRequestTypeDef](./type_defs.md#canceljobrunrequestrequesttypedef) 
    3. result: [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_emr_containers.client import EMRContainersClient
    from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator
    from types_aiobotocore_emr_containers.type_defs import ListJobRunsResponseTypeDef


    session = Session()

    client: EMRContainersClient
    async with session.client("emr-containers") as client:  # (1)
        paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")  # (2)
        async for item in paginator.paginate(...):
            item: ListJobRunsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [EMRContainersClient](./client.md)
    2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
    3. item: [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 




