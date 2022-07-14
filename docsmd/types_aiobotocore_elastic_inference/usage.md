# Examples

> [Index](../README.md) > [ElasticInference](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
    type annotations stubs module [types-aiobotocore-elastic-inference](https://pypi.org/project/types-aiobotocore-elastic-inference/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[elastic-inference]` package installed.

Write your `ElasticInference` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elastic-inference") as client:  # (1)
        result = await client.describe_accelerator_offerings()  # (2)
    ```

    1. client: [ElasticInferenceClient](./client.md)
    2. result: [:material-code-braces: DescribeAcceleratorOfferingsResponseTypeDef](./type_defs.md#describeacceleratorofferingsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elastic-inference") as client:  # (1)
        paginator = client.get_paginator("describe_accelerators")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ElasticInferenceClient](./client.md)
    2. paginator: [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)
    3. item: [:material-code-braces: DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[elastic-inference]`
or a standalone `types_aiobotocore_elastic_inference` package, you have to explicitly specify
`client: ElasticInferenceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elastic_inference.client import ElasticInferenceClient
    from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorOfferingsResponseTypeDef
    from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorOfferingsRequestRequestTypeDef


    session = Session()

    client: ElasticInferenceClient
    async with session.client("elastic-inference") as client:  # (1)
        kwargs: DescribeAcceleratorOfferingsRequestRequestTypeDef = {...}  # (2)
        result: DescribeAcceleratorOfferingsResponseTypeDef = await client.describe_accelerator_offerings(**kwargs)  # (3)
    ```

    1. client: [ElasticInferenceClient](./client.md)
    2. kwargs: [:material-code-braces: DescribeAcceleratorOfferingsRequestRequestTypeDef](./type_defs.md#describeacceleratorofferingsrequestrequesttypedef) 
    3. result: [:material-code-braces: DescribeAcceleratorOfferingsResponseTypeDef](./type_defs.md#describeacceleratorofferingsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elastic_inference.client import ElasticInferenceClient
    from types_aiobotocore_elastic_inference.paginator import DescribeAcceleratorsPaginator
    from types_aiobotocore_elastic_inference.type_defs import DescribeAcceleratorsResponseTypeDef


    session = Session()

    client: ElasticInferenceClient
    async with session.client("elastic-inference") as client:  # (1)
        paginator: DescribeAcceleratorsPaginator = client.get_paginator("describe_accelerators")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeAcceleratorsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [ElasticInferenceClient](./client.md)
    2. paginator: [DescribeAcceleratorsPaginator](./paginators.md#describeacceleratorspaginator)
    3. item: [:material-code-braces: DescribeAcceleratorsResponseTypeDef](./type_defs.md#describeacceleratorsresponsetypedef) 




