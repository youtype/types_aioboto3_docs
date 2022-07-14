# Examples

> [Index](../README.md) > [DataExchange](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[dataexchange]` package installed.

Write your `DataExchange` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("dataexchange") as client:  # (1)
        result = await client.cancel_job()  # (2)
    ```

    1. client: [DataExchangeClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("dataexchange") as client:  # (1)
        paginator = client.get_paginator("list_data_set_revisions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [DataExchangeClient](./client.md)
    2. paginator: [ListDataSetRevisionsPaginator](./paginators.md#listdatasetrevisionspaginator)
    3. item: [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[dataexchange]`
or a standalone `types_aiobotocore_dataexchange` package, you have to explicitly specify
`client: DataExchangeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_dataexchange.client import DataExchangeClient
    from types_aiobotocore_dataexchange.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_dataexchange.type_defs import CancelJobRequestRequestTypeDef


    session = Session()

    client: DataExchangeClient
    async with session.client("dataexchange") as client:  # (1)
        kwargs: CancelJobRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.cancel_job(**kwargs)  # (3)
    ```

    1. client: [DataExchangeClient](./client.md)
    2. kwargs: [:material-code-braces: CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_dataexchange.client import DataExchangeClient
    from types_aiobotocore_dataexchange.paginator import ListDataSetRevisionsPaginator
    from types_aiobotocore_dataexchange.type_defs import ListDataSetRevisionsResponseTypeDef


    session = Session()

    client: DataExchangeClient
    async with session.client("dataexchange") as client:  # (1)
        paginator: ListDataSetRevisionsPaginator = client.get_paginator("list_data_set_revisions")  # (2)
        async for item in paginator.paginate(...):
            item: ListDataSetRevisionsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [DataExchangeClient](./client.md)
    2. paginator: [ListDataSetRevisionsPaginator](./paginators.md#listdatasetrevisionspaginator)
    3. item: [:material-code-braces: ListDataSetRevisionsResponseTypeDef](./type_defs.md#listdatasetrevisionsresponsetypedef) 




