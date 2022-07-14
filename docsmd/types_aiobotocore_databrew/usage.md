# Examples

> [Index](../README.md) > [GlueDataBrew](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[databrew]` package installed.

Write your `GlueDataBrew` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("databrew") as client:  # (1)
        result = await client.batch_delete_recipe_version()  # (2)
    ```

    1. client: [GlueDataBrewClient](./client.md)
    2. result: [:material-code-braces: BatchDeleteRecipeVersionResponseTypeDef](./type_defs.md#batchdeleterecipeversionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("databrew") as client:  # (1)
        paginator = client.get_paginator("list_datasets")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GlueDataBrewClient](./client.md)
    2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
    3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[databrew]`
or a standalone `types_aiobotocore_databrew` package, you have to explicitly specify
`client: GlueDataBrewClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_databrew.client import GlueDataBrewClient
    from types_aiobotocore_databrew.type_defs import BatchDeleteRecipeVersionResponseTypeDef
    from types_aiobotocore_databrew.type_defs import BatchDeleteRecipeVersionRequestRequestTypeDef


    session = Session()

    client: GlueDataBrewClient
    async with session.client("databrew") as client:  # (1)
        kwargs: BatchDeleteRecipeVersionRequestRequestTypeDef = {...}  # (2)
        result: BatchDeleteRecipeVersionResponseTypeDef = await client.batch_delete_recipe_version(**kwargs)  # (3)
    ```

    1. client: [GlueDataBrewClient](./client.md)
    2. kwargs: [:material-code-braces: BatchDeleteRecipeVersionRequestRequestTypeDef](./type_defs.md#batchdeleterecipeversionrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchDeleteRecipeVersionResponseTypeDef](./type_defs.md#batchdeleterecipeversionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_databrew.client import GlueDataBrewClient
    from types_aiobotocore_databrew.paginator import ListDatasetsPaginator
    from types_aiobotocore_databrew.type_defs import ListDatasetsResponseTypeDef


    session = Session()

    client: GlueDataBrewClient
    async with session.client("databrew") as client:  # (1)
        paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
        async for item in paginator.paginate(...):
            item: ListDatasetsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [GlueDataBrewClient](./client.md)
    2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
    3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 




