# Examples

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[elastictranscoder]` package installed.

Write your `ElasticTranscoder` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elastictranscoder") as client:  # (1)
        result = await client.create_job()  # (2)
    ```

    1. client: [ElasticTranscoderClient](./client.md)
    2. result: [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elastictranscoder") as client:  # (1)
        paginator = client.get_paginator("list_jobs_by_pipeline")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ElasticTranscoderClient](./client.md)
    2. paginator: [ListJobsByPipelinePaginator](./paginators.md#listjobsbypipelinepaginator)
    3. item: [:material-code-braces: ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elastictranscoder") as client:  # (1)
        waiter = client.get_waiter("job_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [ElasticTranscoderClient](./client.md)
    2. waiter: [JobCompleteWaiter](./waiters.md#jobcompletewaiter)


### Explicit type annotations

With `types-aioboto3-lite[elastictranscoder]`
or a standalone `types_aiobotocore_elastictranscoder` package, you have to explicitly specify
`client: ElasticTranscoderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elastictranscoder.client import ElasticTranscoderClient
    from types_aiobotocore_elastictranscoder.type_defs import CreateJobResponseTypeDef
    from types_aiobotocore_elastictranscoder.type_defs import CreateJobRequestRequestTypeDef


    session = Session()

    client: ElasticTranscoderClient
    async with session.client("elastictranscoder") as client:  # (1)
        kwargs: CreateJobRequestRequestTypeDef = {...}  # (2)
        result: CreateJobResponseTypeDef = await client.create_job(**kwargs)  # (3)
    ```

    1. client: [ElasticTranscoderClient](./client.md)
    2. kwargs: [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elastictranscoder.client import ElasticTranscoderClient
    from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator
    from types_aiobotocore_elastictranscoder.type_defs import ListJobsByPipelineResponseTypeDef


    session = Session()

    client: ElasticTranscoderClient
    async with session.client("elastictranscoder") as client:  # (1)
        paginator: ListJobsByPipelinePaginator = client.get_paginator("list_jobs_by_pipeline")  # (2)
        async for item in paginator.paginate(...):
            item: ListJobsByPipelineResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [ElasticTranscoderClient](./client.md)
    2. paginator: [ListJobsByPipelinePaginator](./paginators.md#listjobsbypipelinepaginator)
    3. item: [:material-code-braces: ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elastictranscoder.client import ElasticTranscoderClient
    from types_aiobotocore_elastictranscoder.waiter import JobCompleteWaiter


    session = Session()

    async with session.client("elastictranscoder") as client:  # (1)
        waiter = client.get_waiter("job_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [ElasticTranscoderClient](./client.md)
    2. waiter: [JobCompleteWaiter](./waiters.md#jobcompletewaiter)


