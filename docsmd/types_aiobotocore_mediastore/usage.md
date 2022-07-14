# Examples

> [Index](../README.md) > [MediaStore](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
    type annotations stubs module [types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mediastore]` package installed.

Write your `MediaStore` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediastore") as client:  # (1)
        result = await client.create_container()  # (2)
    ```

    1. client: [MediaStoreClient](./client.md)
    2. result: [:material-code-braces: CreateContainerOutputTypeDef](./type_defs.md#createcontaineroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediastore") as client:  # (1)
        paginator = client.get_paginator("list_containers")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MediaStoreClient](./client.md)
    2. paginator: [ListContainersPaginator](./paginators.md#listcontainerspaginator)
    3. item: [:material-code-braces: ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[mediastore]`
or a standalone `types_aiobotocore_mediastore` package, you have to explicitly specify
`client: MediaStoreClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediastore.client import MediaStoreClient
    from types_aiobotocore_mediastore.type_defs import CreateContainerOutputTypeDef
    from types_aiobotocore_mediastore.type_defs import CreateContainerInputRequestTypeDef


    session = Session()

    client: MediaStoreClient
    async with session.client("mediastore") as client:  # (1)
        kwargs: CreateContainerInputRequestTypeDef = {...}  # (2)
        result: CreateContainerOutputTypeDef = await client.create_container(**kwargs)  # (3)
    ```

    1. client: [MediaStoreClient](./client.md)
    2. kwargs: [:material-code-braces: CreateContainerInputRequestTypeDef](./type_defs.md#createcontainerinputrequesttypedef) 
    3. result: [:material-code-braces: CreateContainerOutputTypeDef](./type_defs.md#createcontaineroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediastore.client import MediaStoreClient
    from types_aiobotocore_mediastore.paginator import ListContainersPaginator
    from types_aiobotocore_mediastore.type_defs import ListContainersOutputTypeDef


    session = Session()

    client: MediaStoreClient
    async with session.client("mediastore") as client:  # (1)
        paginator: ListContainersPaginator = client.get_paginator("list_containers")  # (2)
        async for item in paginator.paginate(...):
            item: ListContainersOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [MediaStoreClient](./client.md)
    2. paginator: [ListContainersPaginator](./paginators.md#listcontainerspaginator)
    3. item: [:material-code-braces: ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef) 




