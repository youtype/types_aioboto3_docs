# Examples

> [Index](../README.md) > [XRay](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[xray]` package installed.

Write your `XRay` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("xray") as client:  # (1)
        result = await client.batch_get_traces()  # (2)
    ```

    1. client: [XRayClient](./client.md)
    2. result: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("xray") as client:  # (1)
        paginator = client.get_paginator("batch_get_traces")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [XRayClient](./client.md)
    2. paginator: [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
    3. item: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[xray]`
or a standalone `types_aiobotocore_xray` package, you have to explicitly specify
`client: XRayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_xray.client import XRayClient
    from types_aiobotocore_xray.type_defs import BatchGetTracesResultTypeDef
    from types_aiobotocore_xray.type_defs import BatchGetTracesRequestRequestTypeDef


    session = Session()

    client: XRayClient
    async with session.client("xray") as client:  # (1)
        kwargs: BatchGetTracesRequestRequestTypeDef = {...}  # (2)
        result: BatchGetTracesResultTypeDef = await client.batch_get_traces(**kwargs)  # (3)
    ```

    1. client: [XRayClient](./client.md)
    2. kwargs: [:material-code-braces: BatchGetTracesRequestRequestTypeDef](./type_defs.md#batchgettracesrequestrequesttypedef) 
    3. result: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_xray.client import XRayClient
    from types_aiobotocore_xray.paginator import BatchGetTracesPaginator
    from types_aiobotocore_xray.type_defs import BatchGetTracesResultTypeDef


    session = Session()

    client: XRayClient
    async with session.client("xray") as client:  # (1)
        paginator: BatchGetTracesPaginator = client.get_paginator("batch_get_traces")  # (2)
        async for item in paginator.paginate(...):
            item: BatchGetTracesResultTypeDef
            print(item)  # (3)
    ```

    1. client: [XRayClient](./client.md)
    2. paginator: [BatchGetTracesPaginator](./paginators.md#batchgettracespaginator)
    3. item: [:material-code-braces: BatchGetTracesResultTypeDef](./type_defs.md#batchgettracesresulttypedef) 




