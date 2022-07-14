# Examples

> [Index](../README.md) > [LookoutforVision](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
    type annotations stubs module [types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[lookoutvision]` package installed.

Write your `LookoutforVision` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lookoutvision") as client:  # (1)
        result = await client.create_dataset()  # (2)
    ```

    1. client: [LookoutforVisionClient](./client.md)
    2. result: [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("lookoutvision") as client:  # (1)
        paginator = client.get_paginator("list_dataset_entries")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [LookoutforVisionClient](./client.md)
    2. paginator: [ListDatasetEntriesPaginator](./paginators.md#listdatasetentriespaginator)
    3. item: [:material-code-braces: ListDatasetEntriesResponseTypeDef](./type_defs.md#listdatasetentriesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[lookoutvision]`
or a standalone `types_aiobotocore_lookoutvision` package, you have to explicitly specify
`client: LookoutforVisionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lookoutvision.client import LookoutforVisionClient
    from types_aiobotocore_lookoutvision.type_defs import CreateDatasetResponseTypeDef
    from types_aiobotocore_lookoutvision.type_defs import CreateDatasetRequestRequestTypeDef


    session = Session()

    client: LookoutforVisionClient
    async with session.client("lookoutvision") as client:  # (1)
        kwargs: CreateDatasetRequestRequestTypeDef = {...}  # (2)
        result: CreateDatasetResponseTypeDef = await client.create_dataset(**kwargs)  # (3)
    ```

    1. client: [LookoutforVisionClient](./client.md)
    2. kwargs: [:material-code-braces: CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_lookoutvision.client import LookoutforVisionClient
    from types_aiobotocore_lookoutvision.paginator import ListDatasetEntriesPaginator
    from types_aiobotocore_lookoutvision.type_defs import ListDatasetEntriesResponseTypeDef


    session = Session()

    client: LookoutforVisionClient
    async with session.client("lookoutvision") as client:  # (1)
        paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")  # (2)
        async for item in paginator.paginate(...):
            item: ListDatasetEntriesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [LookoutforVisionClient](./client.md)
    2. paginator: [ListDatasetEntriesPaginator](./paginators.md#listdatasetentriespaginator)
    3. item: [:material-code-braces: ListDatasetEntriesResponseTypeDef](./type_defs.md#listdatasetentriesresponsetypedef) 




