# Examples

> [Index](../README.md) > [Rekognition](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Rekognition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
    type annotations stubs module [types-aiobotocore-rekognition](https://pypi.org/project/types-aiobotocore-rekognition/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[rekognition]` package installed.

Write your `Rekognition` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rekognition") as client:  # (1)
        result = await client.compare_faces()  # (2)
    ```

    1. client: [RekognitionClient](./client.md)
    2. result: [:material-code-braces: CompareFacesResponseTypeDef](./type_defs.md#comparefacesresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rekognition") as client:  # (1)
        paginator = client.get_paginator("describe_project_versions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [RekognitionClient](./client.md)
    2. paginator: [DescribeProjectVersionsPaginator](./paginators.md#describeprojectversionspaginator)
    3. item: [:material-code-braces: DescribeProjectVersionsResponseTypeDef](./type_defs.md#describeprojectversionsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("rekognition") as client:  # (1)
        waiter = client.get_waiter("project_version_running")  # (2)
        await waiter.wait()
    ```

    1. client: [RekognitionClient](./client.md)
    2. waiter: [ProjectVersionRunningWaiter](./waiters.md#projectversionrunningwaiter)


### Explicit type annotations

With `types-aioboto3-lite[rekognition]`
or a standalone `types_aiobotocore_rekognition` package, you have to explicitly specify
`client: RekognitionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rekognition.client import RekognitionClient
    from types_aiobotocore_rekognition.type_defs import CompareFacesResponseTypeDef
    from types_aiobotocore_rekognition.type_defs import CompareFacesRequestRequestTypeDef


    session = Session()

    client: RekognitionClient
    async with session.client("rekognition") as client:  # (1)
        kwargs: CompareFacesRequestRequestTypeDef = {...}  # (2)
        result: CompareFacesResponseTypeDef = await client.compare_faces(**kwargs)  # (3)
    ```

    1. client: [RekognitionClient](./client.md)
    2. kwargs: [:material-code-braces: CompareFacesRequestRequestTypeDef](./type_defs.md#comparefacesrequestrequesttypedef) 
    3. result: [:material-code-braces: CompareFacesResponseTypeDef](./type_defs.md#comparefacesresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rekognition.client import RekognitionClient
    from types_aiobotocore_rekognition.paginator import DescribeProjectVersionsPaginator
    from types_aiobotocore_rekognition.type_defs import DescribeProjectVersionsResponseTypeDef


    session = Session()

    client: RekognitionClient
    async with session.client("rekognition") as client:  # (1)
        paginator: DescribeProjectVersionsPaginator = client.get_paginator("describe_project_versions")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeProjectVersionsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [RekognitionClient](./client.md)
    2. paginator: [DescribeProjectVersionsPaginator](./paginators.md#describeprojectversionspaginator)
    3. item: [:material-code-braces: DescribeProjectVersionsResponseTypeDef](./type_defs.md#describeprojectversionsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_rekognition.client import RekognitionClient
    from types_aiobotocore_rekognition.waiter import ProjectVersionRunningWaiter


    session = Session()

    async with session.client("rekognition") as client:  # (1)
        waiter = client.get_waiter("project_version_running")  # (2)
        await waiter.wait()
    ```

    1. client: [RekognitionClient](./client.md)
    2. waiter: [ProjectVersionRunningWaiter](./waiters.md#projectversionrunningwaiter)


