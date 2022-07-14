# Examples

> [Index](../README.md) > [MediaConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[mediaconnect]` package installed.

Write your `MediaConnect` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediaconnect") as client:  # (1)
        result = await client.add_flow_media_streams()  # (2)
    ```

    1. client: [MediaConnectClient](./client.md)
    2. result: [:material-code-braces: AddFlowMediaStreamsResponseTypeDef](./type_defs.md#addflowmediastreamsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediaconnect") as client:  # (1)
        paginator = client.get_paginator("list_entitlements")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MediaConnectClient](./client.md)
    2. paginator: [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
    3. item: [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("mediaconnect") as client:  # (1)
        waiter = client.get_waiter("flow_active")  # (2)
        await waiter.wait()
    ```

    1. client: [MediaConnectClient](./client.md)
    2. waiter: [FlowActiveWaiter](./waiters.md#flowactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[mediaconnect]`
or a standalone `types_aiobotocore_mediaconnect` package, you have to explicitly specify
`client: MediaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediaconnect.client import MediaConnectClient
    from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsResponseTypeDef
    from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsRequestRequestTypeDef


    session = Session()

    client: MediaConnectClient
    async with session.client("mediaconnect") as client:  # (1)
        kwargs: AddFlowMediaStreamsRequestRequestTypeDef = {...}  # (2)
        result: AddFlowMediaStreamsResponseTypeDef = await client.add_flow_media_streams(**kwargs)  # (3)
    ```

    1. client: [MediaConnectClient](./client.md)
    2. kwargs: [:material-code-braces: AddFlowMediaStreamsRequestRequestTypeDef](./type_defs.md#addflowmediastreamsrequestrequesttypedef) 
    3. result: [:material-code-braces: AddFlowMediaStreamsResponseTypeDef](./type_defs.md#addflowmediastreamsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediaconnect.client import MediaConnectClient
    from types_aiobotocore_mediaconnect.paginator import ListEntitlementsPaginator
    from types_aiobotocore_mediaconnect.type_defs import ListEntitlementsResponseTypeDef


    session = Session()

    client: MediaConnectClient
    async with session.client("mediaconnect") as client:  # (1)
        paginator: ListEntitlementsPaginator = client.get_paginator("list_entitlements")  # (2)
        async for item in paginator.paginate(...):
            item: ListEntitlementsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [MediaConnectClient](./client.md)
    2. paginator: [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
    3. item: [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_mediaconnect.client import MediaConnectClient
    from types_aiobotocore_mediaconnect.waiter import FlowActiveWaiter


    session = Session()

    async with session.client("mediaconnect") as client:  # (1)
        waiter = client.get_waiter("flow_active")  # (2)
        await waiter.wait()
    ```

    1. client: [MediaConnectClient](./client.md)
    2. waiter: [FlowActiveWaiter](./waiters.md#flowactivewaiter)


