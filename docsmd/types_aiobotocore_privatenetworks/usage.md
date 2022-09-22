# Examples

> [Index](../README.md) > [Private5G](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[privatenetworks]` package installed.

Write your `Private5G` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("privatenetworks") as client:  # (1)
        result = await client.acknowledge_order_receipt()  # (2)
    ```

    1. client: [Private5GClient](./client.md)
    2. result: [:material-code-braces: AcknowledgeOrderReceiptResponseTypeDef](./type_defs.md#acknowledgeorderreceiptresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("privatenetworks") as client:  # (1)
        paginator = client.get_paginator("list_device_identifiers")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [Private5GClient](./client.md)
    2. paginator: [ListDeviceIdentifiersPaginator](./paginators.md#listdeviceidentifierspaginator)
    3. item: [:material-code-braces: ListDeviceIdentifiersResponseTypeDef](./type_defs.md#listdeviceidentifiersresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[privatenetworks]`
or a standalone `types_aiobotocore_privatenetworks` package, you have to explicitly specify
`client: Private5GClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_privatenetworks.client import Private5GClient
    from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptResponseTypeDef
    from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef


    session = Session()

    client: Private5GClient
    async with session.client("privatenetworks") as client:  # (1)
        kwargs: AcknowledgeOrderReceiptRequestRequestTypeDef = {...}  # (2)
        result: AcknowledgeOrderReceiptResponseTypeDef = await client.acknowledge_order_receipt(**kwargs)  # (3)
    ```

    1. client: [Private5GClient](./client.md)
    2. kwargs: [:material-code-braces: AcknowledgeOrderReceiptRequestRequestTypeDef](./type_defs.md#acknowledgeorderreceiptrequestrequesttypedef) 
    3. result: [:material-code-braces: AcknowledgeOrderReceiptResponseTypeDef](./type_defs.md#acknowledgeorderreceiptresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_privatenetworks.client import Private5GClient
    from types_aiobotocore_privatenetworks.paginator import ListDeviceIdentifiersPaginator
    from types_aiobotocore_privatenetworks.type_defs import ListDeviceIdentifiersResponseTypeDef


    session = Session()

    client: Private5GClient
    async with session.client("privatenetworks") as client:  # (1)
        paginator: ListDeviceIdentifiersPaginator = client.get_paginator("list_device_identifiers")  # (2)
        async for item in paginator.paginate(...):
            item: ListDeviceIdentifiersResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [Private5GClient](./client.md)
    2. paginator: [ListDeviceIdentifiersPaginator](./paginators.md#listdeviceidentifierspaginator)
    3. item: [:material-code-braces: ListDeviceIdentifiersResponseTypeDef](./type_defs.md#listdeviceidentifiersresponsetypedef) 




