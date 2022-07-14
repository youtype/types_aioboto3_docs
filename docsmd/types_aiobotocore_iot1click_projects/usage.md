# Examples

> [Index](../README.md) > [IoT1ClickProjects](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
    type annotations stubs module [types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[iot1click-projects]` package installed.

Write your `IoT1ClickProjects` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iot1click-projects") as client:  # (1)
        result = await client.describe_placement()  # (2)
    ```

    1. client: [IoT1ClickProjectsClient](./client.md)
    2. result: [:material-code-braces: DescribePlacementResponseTypeDef](./type_defs.md#describeplacementresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("iot1click-projects") as client:  # (1)
        paginator = client.get_paginator("list_placements")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [IoT1ClickProjectsClient](./client.md)
    2. paginator: [ListPlacementsPaginator](./paginators.md#listplacementspaginator)
    3. item: [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[iot1click-projects]`
or a standalone `types_aiobotocore_iot1click_projects` package, you have to explicitly specify
`client: IoT1ClickProjectsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iot1click_projects.client import IoT1ClickProjectsClient
    from types_aiobotocore_iot1click_projects.type_defs import DescribePlacementResponseTypeDef
    from types_aiobotocore_iot1click_projects.type_defs import DescribePlacementRequestRequestTypeDef


    session = Session()

    client: IoT1ClickProjectsClient
    async with session.client("iot1click-projects") as client:  # (1)
        kwargs: DescribePlacementRequestRequestTypeDef = {...}  # (2)
        result: DescribePlacementResponseTypeDef = await client.describe_placement(**kwargs)  # (3)
    ```

    1. client: [IoT1ClickProjectsClient](./client.md)
    2. kwargs: [:material-code-braces: DescribePlacementRequestRequestTypeDef](./type_defs.md#describeplacementrequestrequesttypedef) 
    3. result: [:material-code-braces: DescribePlacementResponseTypeDef](./type_defs.md#describeplacementresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_iot1click_projects.client import IoT1ClickProjectsClient
    from types_aiobotocore_iot1click_projects.paginator import ListPlacementsPaginator
    from types_aiobotocore_iot1click_projects.type_defs import ListPlacementsResponseTypeDef


    session = Session()

    client: IoT1ClickProjectsClient
    async with session.client("iot1click-projects") as client:  # (1)
        paginator: ListPlacementsPaginator = client.get_paginator("list_placements")  # (2)
        async for item in paginator.paginate(...):
            item: ListPlacementsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [IoT1ClickProjectsClient](./client.md)
    2. paginator: [ListPlacementsPaginator](./paginators.md#listplacementspaginator)
    3. item: [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 




