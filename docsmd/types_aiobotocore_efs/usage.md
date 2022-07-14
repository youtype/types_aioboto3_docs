# Examples

> [Index](../README.md) > [EFS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[efs]` package installed.

Write your `EFS` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("efs") as client:  # (1)
        result = await client.create_access_point()  # (2)
    ```

    1. client: [EFSClient](./client.md)
    2. result: [:material-code-braces: AccessPointDescriptionResponseMetadataTypeDef](./type_defs.md#accesspointdescriptionresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("efs") as client:  # (1)
        paginator = client.get_paginator("describe_file_systems")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [EFSClient](./client.md)
    2. paginator: [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
    3. item: [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[efs]`
or a standalone `types_aiobotocore_efs` package, you have to explicitly specify
`client: EFSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_efs.client import EFSClient
    from types_aiobotocore_efs.type_defs import AccessPointDescriptionResponseMetadataTypeDef
    from types_aiobotocore_efs.type_defs import CreateAccessPointRequestRequestTypeDef


    session = Session()

    client: EFSClient
    async with session.client("efs") as client:  # (1)
        kwargs: CreateAccessPointRequestRequestTypeDef = {...}  # (2)
        result: AccessPointDescriptionResponseMetadataTypeDef = await client.create_access_point(**kwargs)  # (3)
    ```

    1. client: [EFSClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAccessPointRequestRequestTypeDef](./type_defs.md#createaccesspointrequestrequesttypedef) 
    3. result: [:material-code-braces: AccessPointDescriptionResponseMetadataTypeDef](./type_defs.md#accesspointdescriptionresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_efs.client import EFSClient
    from types_aiobotocore_efs.paginator import DescribeFileSystemsPaginator
    from types_aiobotocore_efs.type_defs import DescribeFileSystemsResponseTypeDef


    session = Session()

    client: EFSClient
    async with session.client("efs") as client:  # (1)
        paginator: DescribeFileSystemsPaginator = client.get_paginator("describe_file_systems")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeFileSystemsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [EFSClient](./client.md)
    2. paginator: [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
    3. item: [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 




