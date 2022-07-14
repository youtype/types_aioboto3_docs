# Examples

> [Index](../README.md) > [StorageGateway](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [StorageGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
    type annotations stubs module [types-aiobotocore-storagegateway](https://pypi.org/project/types-aiobotocore-storagegateway/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[storagegateway]` package installed.

Write your `StorageGateway` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("storagegateway") as client:  # (1)
        result = await client.activate_gateway()  # (2)
    ```

    1. client: [StorageGatewayClient](./client.md)
    2. result: [:material-code-braces: ActivateGatewayOutputTypeDef](./type_defs.md#activategatewayoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("storagegateway") as client:  # (1)
        paginator = client.get_paginator("describe_tape_archives")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [StorageGatewayClient](./client.md)
    2. paginator: [DescribeTapeArchivesPaginator](./paginators.md#describetapearchivespaginator)
    3. item: [:material-code-braces: DescribeTapeArchivesOutputTypeDef](./type_defs.md#describetapearchivesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[storagegateway]`
or a standalone `types_aiobotocore_storagegateway` package, you have to explicitly specify
`client: StorageGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_storagegateway.client import StorageGatewayClient
    from types_aiobotocore_storagegateway.type_defs import ActivateGatewayOutputTypeDef
    from types_aiobotocore_storagegateway.type_defs import ActivateGatewayInputRequestTypeDef


    session = Session()

    client: StorageGatewayClient
    async with session.client("storagegateway") as client:  # (1)
        kwargs: ActivateGatewayInputRequestTypeDef = {...}  # (2)
        result: ActivateGatewayOutputTypeDef = await client.activate_gateway(**kwargs)  # (3)
    ```

    1. client: [StorageGatewayClient](./client.md)
    2. kwargs: [:material-code-braces: ActivateGatewayInputRequestTypeDef](./type_defs.md#activategatewayinputrequesttypedef) 
    3. result: [:material-code-braces: ActivateGatewayOutputTypeDef](./type_defs.md#activategatewayoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_storagegateway.client import StorageGatewayClient
    from types_aiobotocore_storagegateway.paginator import DescribeTapeArchivesPaginator
    from types_aiobotocore_storagegateway.type_defs import DescribeTapeArchivesOutputTypeDef


    session = Session()

    client: StorageGatewayClient
    async with session.client("storagegateway") as client:  # (1)
        paginator: DescribeTapeArchivesPaginator = client.get_paginator("describe_tape_archives")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeTapeArchivesOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [StorageGatewayClient](./client.md)
    2. paginator: [DescribeTapeArchivesPaginator](./paginators.md#describetapearchivespaginator)
    3. item: [:material-code-braces: DescribeTapeArchivesOutputTypeDef](./type_defs.md#describetapearchivesoutputtypedef) 




