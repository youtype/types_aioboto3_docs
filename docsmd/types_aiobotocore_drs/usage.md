# Examples

> [Index](../README.md) > [drs](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[drs]` package installed.

Write your `drs` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("drs") as client:  # (1)
        result = await client.create_extended_source_server()  # (2)
    ```

    1. client: [drsClient](./client.md)
    2. result: [:material-code-braces: CreateExtendedSourceServerResponseTypeDef](./type_defs.md#createextendedsourceserverresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("drs") as client:  # (1)
        paginator = client.get_paginator("describe_job_log_items")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [drsClient](./client.md)
    2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
    3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[drs]`
or a standalone `types_aiobotocore_drs` package, you have to explicitly specify
`client: drsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_drs.client import drsClient
    from types_aiobotocore_drs.type_defs import CreateExtendedSourceServerResponseTypeDef
    from types_aiobotocore_drs.type_defs import CreateExtendedSourceServerRequestRequestTypeDef


    session = Session()

    client: drsClient
    async with session.client("drs") as client:  # (1)
        kwargs: CreateExtendedSourceServerRequestRequestTypeDef = {...}  # (2)
        result: CreateExtendedSourceServerResponseTypeDef = await client.create_extended_source_server(**kwargs)  # (3)
    ```

    1. client: [drsClient](./client.md)
    2. kwargs: [:material-code-braces: CreateExtendedSourceServerRequestRequestTypeDef](./type_defs.md#createextendedsourceserverrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateExtendedSourceServerResponseTypeDef](./type_defs.md#createextendedsourceserverresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_drs.client import drsClient
    from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator
    from types_aiobotocore_drs.type_defs import DescribeJobLogItemsResponseTypeDef


    session = Session()

    client: drsClient
    async with session.client("drs") as client:  # (1)
        paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeJobLogItemsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [drsClient](./client.md)
    2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
    3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 




