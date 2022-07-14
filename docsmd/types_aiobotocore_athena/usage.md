# Examples

> [Index](../README.md) > [Athena](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
    type annotations stubs module [types-aiobotocore-athena](https://pypi.org/project/types-aiobotocore-athena/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[athena]` package installed.

Write your `Athena` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("athena") as client:  # (1)
        result = await client.batch_get_named_query()  # (2)
    ```

    1. client: [AthenaClient](./client.md)
    2. result: [:material-code-braces: BatchGetNamedQueryOutputTypeDef](./type_defs.md#batchgetnamedqueryoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("athena") as client:  # (1)
        paginator = client.get_paginator("get_query_results")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AthenaClient](./client.md)
    2. paginator: [GetQueryResultsPaginator](./paginators.md#getqueryresultspaginator)
    3. item: [:material-code-braces: GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[athena]`
or a standalone `types_aiobotocore_athena` package, you have to explicitly specify
`client: AthenaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_athena.client import AthenaClient
    from types_aiobotocore_athena.type_defs import BatchGetNamedQueryOutputTypeDef
    from types_aiobotocore_athena.type_defs import BatchGetNamedQueryInputRequestTypeDef


    session = Session()

    client: AthenaClient
    async with session.client("athena") as client:  # (1)
        kwargs: BatchGetNamedQueryInputRequestTypeDef = {...}  # (2)
        result: BatchGetNamedQueryOutputTypeDef = await client.batch_get_named_query(**kwargs)  # (3)
    ```

    1. client: [AthenaClient](./client.md)
    2. kwargs: [:material-code-braces: BatchGetNamedQueryInputRequestTypeDef](./type_defs.md#batchgetnamedqueryinputrequesttypedef) 
    3. result: [:material-code-braces: BatchGetNamedQueryOutputTypeDef](./type_defs.md#batchgetnamedqueryoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_athena.client import AthenaClient
    from types_aiobotocore_athena.paginator import GetQueryResultsPaginator
    from types_aiobotocore_athena.type_defs import GetQueryResultsOutputTypeDef


    session = Session()

    client: AthenaClient
    async with session.client("athena") as client:  # (1)
        paginator: GetQueryResultsPaginator = client.get_paginator("get_query_results")  # (2)
        async for item in paginator.paginate(...):
            item: GetQueryResultsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [AthenaClient](./client.md)
    2. paginator: [GetQueryResultsPaginator](./paginators.md#getqueryresultspaginator)
    3. item: [:material-code-braces: GetQueryResultsOutputTypeDef](./type_defs.md#getqueryresultsoutputtypedef) 




