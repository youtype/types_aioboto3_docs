# Examples

> [Index](../README.md) > [MainframeModernization](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[m2]` package installed.

Write your `MainframeModernization` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("m2") as client:  # (1)
        result = await client.create_application()  # (2)
    ```

    1. client: [MainframeModernizationClient](./client.md)
    2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("m2") as client:  # (1)
        paginator = client.get_paginator("list_application_versions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MainframeModernizationClient](./client.md)
    2. paginator: [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
    3. item: [:material-code-braces: ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[m2]`
or a standalone `types_aiobotocore_m2` package, you have to explicitly specify
`client: MainframeModernizationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_m2.client import MainframeModernizationClient
    from types_aiobotocore_m2.type_defs import CreateApplicationResponseTypeDef
    from types_aiobotocore_m2.type_defs import CreateApplicationRequestRequestTypeDef


    session = Session()

    client: MainframeModernizationClient
    async with session.client("m2") as client:  # (1)
        kwargs: CreateApplicationRequestRequestTypeDef = {...}  # (2)
        result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)  # (3)
    ```

    1. client: [MainframeModernizationClient](./client.md)
    2. kwargs: [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_m2.client import MainframeModernizationClient
    from types_aiobotocore_m2.paginator import ListApplicationVersionsPaginator
    from types_aiobotocore_m2.type_defs import ListApplicationVersionsResponseTypeDef


    session = Session()

    client: MainframeModernizationClient
    async with session.client("m2") as client:  # (1)
        paginator: ListApplicationVersionsPaginator = client.get_paginator("list_application_versions")  # (2)
        async for item in paginator.paginate(...):
            item: ListApplicationVersionsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MainframeModernizationClient](./client.md)
    2. paginator: [ListApplicationVersionsPaginator](./paginators.md#listapplicationversionspaginator)
    3. item: [:material-code-braces: ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef) 




