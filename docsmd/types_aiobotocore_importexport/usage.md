# Examples

> [Index](../README.md) > [ImportExport](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[importexport]` package installed.

Write your `ImportExport` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("importexport") as client:  # (1)
        result = await client.cancel_job()  # (2)
    ```

    1. client: [ImportExportClient](./client.md)
    2. result: [:material-code-braces: CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("importexport") as client:  # (1)
        paginator = client.get_paginator("list_jobs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ImportExportClient](./client.md)
    2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
    3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[importexport]`
or a standalone `types_aiobotocore_importexport` package, you have to explicitly specify
`client: ImportExportClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_importexport.client import ImportExportClient
    from types_aiobotocore_importexport.type_defs import CancelJobOutputTypeDef
    from types_aiobotocore_importexport.type_defs import CancelJobInputRequestTypeDef


    session = Session()

    client: ImportExportClient
    async with session.client("importexport") as client:  # (1)
        kwargs: CancelJobInputRequestTypeDef = {...}  # (2)
        result: CancelJobOutputTypeDef = await client.cancel_job(**kwargs)  # (3)
    ```

    1. client: [ImportExportClient](./client.md)
    2. kwargs: [:material-code-braces: CancelJobInputRequestTypeDef](./type_defs.md#canceljobinputrequesttypedef) 
    3. result: [:material-code-braces: CancelJobOutputTypeDef](./type_defs.md#canceljoboutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_importexport.client import ImportExportClient
    from types_aiobotocore_importexport.paginator import ListJobsPaginator
    from types_aiobotocore_importexport.type_defs import ListJobsOutputTypeDef


    session = Session()

    client: ImportExportClient
    async with session.client("importexport") as client:  # (1)
        paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
        async for item in paginator.paginate(...):
            item: ListJobsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [ImportExportClient](./client.md)
    2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
    3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 




