# Examples

> [Index](../README.md) > [Honeycode](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
    type annotations stubs module [types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[honeycode]` package installed.

Write your `Honeycode` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("honeycode") as client:  # (1)
        result = await client.batch_create_table_rows()  # (2)
    ```

    1. client: [HoneycodeClient](./client.md)
    2. result: [:material-code-braces: BatchCreateTableRowsResultTypeDef](./type_defs.md#batchcreatetablerowsresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("honeycode") as client:  # (1)
        paginator = client.get_paginator("list_table_columns")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [HoneycodeClient](./client.md)
    2. paginator: [ListTableColumnsPaginator](./paginators.md#listtablecolumnspaginator)
    3. item: [:material-code-braces: ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[honeycode]`
or a standalone `types_aiobotocore_honeycode` package, you have to explicitly specify
`client: HoneycodeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_honeycode.client import HoneycodeClient
    from types_aiobotocore_honeycode.type_defs import BatchCreateTableRowsResultTypeDef
    from types_aiobotocore_honeycode.type_defs import BatchCreateTableRowsRequestRequestTypeDef


    session = Session()

    client: HoneycodeClient
    async with session.client("honeycode") as client:  # (1)
        kwargs: BatchCreateTableRowsRequestRequestTypeDef = {...}  # (2)
        result: BatchCreateTableRowsResultTypeDef = await client.batch_create_table_rows(**kwargs)  # (3)
    ```

    1. client: [HoneycodeClient](./client.md)
    2. kwargs: [:material-code-braces: BatchCreateTableRowsRequestRequestTypeDef](./type_defs.md#batchcreatetablerowsrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchCreateTableRowsResultTypeDef](./type_defs.md#batchcreatetablerowsresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_honeycode.client import HoneycodeClient
    from types_aiobotocore_honeycode.paginator import ListTableColumnsPaginator
    from types_aiobotocore_honeycode.type_defs import ListTableColumnsResultTypeDef


    session = Session()

    client: HoneycodeClient
    async with session.client("honeycode") as client:  # (1)
        paginator: ListTableColumnsPaginator = client.get_paginator("list_table_columns")  # (2)
        async for item in paginator.paginate(...):
            item: ListTableColumnsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [HoneycodeClient](./client.md)
    2. paginator: [ListTableColumnsPaginator](./paginators.md#listtablecolumnspaginator)
    3. item: [:material-code-braces: ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef) 




