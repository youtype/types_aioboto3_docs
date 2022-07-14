# Examples

> [Index](../README.md) > [MTurk](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
    type annotations stubs module [types-aiobotocore-mturk](https://pypi.org/project/types-aiobotocore-mturk/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mturk]` package installed.

Write your `MTurk` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mturk") as client:  # (1)
        result = await client.create_hit()  # (2)
    ```

    1. client: [MTurkClient](./client.md)
    2. result: [:material-code-braces: CreateHITResponseTypeDef](./type_defs.md#createhitresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mturk") as client:  # (1)
        paginator = client.get_paginator("list_assignments_for_hit")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MTurkClient](./client.md)
    2. paginator: [ListAssignmentsForHITPaginator](./paginators.md#listassignmentsforhitpaginator)
    3. item: [:material-code-braces: ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mturk]`
or a standalone `types_aiobotocore_mturk` package, you have to explicitly specify
`client: MTurkClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mturk.client import MTurkClient
    from types_aiobotocore_mturk.type_defs import CreateHITResponseTypeDef
    from types_aiobotocore_mturk.type_defs import CreateHITRequestRequestTypeDef


    session = Session()

    client: MTurkClient
    async with session.client("mturk") as client:  # (1)
        kwargs: CreateHITRequestRequestTypeDef = {...}  # (2)
        result: CreateHITResponseTypeDef = await client.create_hit(**kwargs)  # (3)
    ```

    1. client: [MTurkClient](./client.md)
    2. kwargs: [:material-code-braces: CreateHITRequestRequestTypeDef](./type_defs.md#createhitrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateHITResponseTypeDef](./type_defs.md#createhitresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mturk.client import MTurkClient
    from types_aiobotocore_mturk.paginator import ListAssignmentsForHITPaginator
    from types_aiobotocore_mturk.type_defs import ListAssignmentsForHITResponseTypeDef


    session = Session()

    client: MTurkClient
    async with session.client("mturk") as client:  # (1)
        paginator: ListAssignmentsForHITPaginator = client.get_paginator("list_assignments_for_hit")  # (2)
        async for item in paginator.paginate(...):
            item: ListAssignmentsForHITResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MTurkClient](./client.md)
    2. paginator: [ListAssignmentsForHITPaginator](./paginators.md#listassignmentsforhitpaginator)
    3. item: [:material-code-braces: ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef) 




