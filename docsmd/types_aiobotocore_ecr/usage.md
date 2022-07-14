# Examples

> [Index](../README.md) > [ECR](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ecr]` package installed.

Write your `ECR` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ecr") as client:  # (1)
        result = await client.batch_check_layer_availability()  # (2)
    ```

    1. client: [ECRClient](./client.md)
    2. result: [:material-code-braces: BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ecr") as client:  # (1)
        paginator = client.get_paginator("describe_image_scan_findings")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ECRClient](./client.md)
    2. paginator: [DescribeImageScanFindingsPaginator](./paginators.md#describeimagescanfindingspaginator)
    3. item: [:material-code-braces: DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ecr") as client:  # (1)
        waiter = client.get_waiter("image_scan_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [ECRClient](./client.md)
    2. waiter: [ImageScanCompleteWaiter](./waiters.md#imagescancompletewaiter)


### Explicit type annotations

With `types-aioboto3-lite[ecr]`
or a standalone `types_aiobotocore_ecr` package, you have to explicitly specify
`client: ECRClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ecr.client import ECRClient
    from types_aiobotocore_ecr.type_defs import BatchCheckLayerAvailabilityResponseTypeDef
    from types_aiobotocore_ecr.type_defs import BatchCheckLayerAvailabilityRequestRequestTypeDef


    session = Session()

    client: ECRClient
    async with session.client("ecr") as client:  # (1)
        kwargs: BatchCheckLayerAvailabilityRequestRequestTypeDef = {...}  # (2)
        result: BatchCheckLayerAvailabilityResponseTypeDef = await client.batch_check_layer_availability(**kwargs)  # (3)
    ```

    1. client: [ECRClient](./client.md)
    2. kwargs: [:material-code-braces: BatchCheckLayerAvailabilityRequestRequestTypeDef](./type_defs.md#batchchecklayeravailabilityrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ecr.client import ECRClient
    from types_aiobotocore_ecr.paginator import DescribeImageScanFindingsPaginator
    from types_aiobotocore_ecr.type_defs import DescribeImageScanFindingsResponseTypeDef


    session = Session()

    client: ECRClient
    async with session.client("ecr") as client:  # (1)
        paginator: DescribeImageScanFindingsPaginator = client.get_paginator("describe_image_scan_findings")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeImageScanFindingsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [ECRClient](./client.md)
    2. paginator: [DescribeImageScanFindingsPaginator](./paginators.md#describeimagescanfindingspaginator)
    3. item: [:material-code-braces: DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ecr.client import ECRClient
    from types_aiobotocore_ecr.waiter import ImageScanCompleteWaiter


    session = Session()

    async with session.client("ecr") as client:  # (1)
        waiter = client.get_waiter("image_scan_complete")  # (2)
        await waiter.wait()
    ```

    1. client: [ECRClient](./client.md)
    2. waiter: [ImageScanCompleteWaiter](./waiters.md#imagescancompletewaiter)


