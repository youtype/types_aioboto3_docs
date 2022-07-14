# Examples

> [Index](../README.md) > [Polly](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
    type annotations stubs module [types-aiobotocore-polly](https://pypi.org/project/types-aiobotocore-polly/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[polly]` package installed.

Write your `Polly` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("polly") as client:  # (1)
        result = await client.describe_voices()  # (2)
    ```

    1. client: [PollyClient](./client.md)
    2. result: [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("polly") as client:  # (1)
        paginator = client.get_paginator("describe_voices")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [PollyClient](./client.md)
    2. paginator: [DescribeVoicesPaginator](./paginators.md#describevoicespaginator)
    3. item: [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[polly]`
or a standalone `types_aiobotocore_polly` package, you have to explicitly specify
`client: PollyClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_polly.client import PollyClient
    from types_aiobotocore_polly.type_defs import DescribeVoicesOutputTypeDef
    from types_aiobotocore_polly.type_defs import DescribeVoicesInputRequestTypeDef


    session = Session()

    client: PollyClient
    async with session.client("polly") as client:  # (1)
        kwargs: DescribeVoicesInputRequestTypeDef = {...}  # (2)
        result: DescribeVoicesOutputTypeDef = await client.describe_voices(**kwargs)  # (3)
    ```

    1. client: [PollyClient](./client.md)
    2. kwargs: [:material-code-braces: DescribeVoicesInputRequestTypeDef](./type_defs.md#describevoicesinputrequesttypedef) 
    3. result: [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_polly.client import PollyClient
    from types_aiobotocore_polly.paginator import DescribeVoicesPaginator
    from types_aiobotocore_polly.type_defs import DescribeVoicesOutputTypeDef


    session = Session()

    client: PollyClient
    async with session.client("polly") as client:  # (1)
        paginator: DescribeVoicesPaginator = client.get_paginator("describe_voices")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeVoicesOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [PollyClient](./client.md)
    2. paginator: [DescribeVoicesPaginator](./paginators.md#describevoicespaginator)
    3. item: [:material-code-braces: DescribeVoicesOutputTypeDef](./type_defs.md#describevoicesoutputtypedef) 




