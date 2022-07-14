# Examples

> [Index](../README.md) > [CloudControlApi](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudcontrol]` package installed.

Write your `CloudControlApi` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudcontrol") as client:  # (1)
        result = await client.cancel_resource_request()  # (2)
    ```

    1. client: [CloudControlApiClient](./client.md)
    2. result: [:material-code-braces: CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudcontrol") as client:  # (1)
        paginator = client.get_paginator("list_resource_requests")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudControlApiClient](./client.md)
    2. paginator: [ListResourceRequestsPaginator](./paginators.md#listresourcerequestspaginator)
    3. item: [:material-code-braces: ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudcontrol") as client:  # (1)
        waiter = client.get_waiter("resource_request_success")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudControlApiClient](./client.md)
    2. waiter: [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)


### Explicit type annotations

With `types-aioboto3-lite[cloudcontrol]`
or a standalone `types_aiobotocore_cloudcontrol` package, you have to explicitly specify
`client: CloudControlApiClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
    from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestOutputTypeDef
    from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef


    session = Session()

    client: CloudControlApiClient
    async with session.client("cloudcontrol") as client:  # (1)
        kwargs: CancelResourceRequestInputRequestTypeDef = {...}  # (2)
        result: CancelResourceRequestOutputTypeDef = await client.cancel_resource_request(**kwargs)  # (3)
    ```

    1. client: [CloudControlApiClient](./client.md)
    2. kwargs: [:material-code-braces: CancelResourceRequestInputRequestTypeDef](./type_defs.md#cancelresourcerequestinputrequesttypedef) 
    3. result: [:material-code-braces: CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
    from types_aiobotocore_cloudcontrol.paginator import ListResourceRequestsPaginator
    from types_aiobotocore_cloudcontrol.type_defs import ListResourceRequestsOutputTypeDef


    session = Session()

    client: CloudControlApiClient
    async with session.client("cloudcontrol") as client:  # (1)
        paginator: ListResourceRequestsPaginator = client.get_paginator("list_resource_requests")  # (2)
        async for item in paginator.paginate(...):
            item: ListResourceRequestsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [CloudControlApiClient](./client.md)
    2. paginator: [ListResourceRequestsPaginator](./paginators.md#listresourcerequestspaginator)
    3. item: [:material-code-braces: ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
    from types_aiobotocore_cloudcontrol.waiter import ResourceRequestSuccessWaiter


    session = Session()

    async with session.client("cloudcontrol") as client:  # (1)
        waiter = client.get_waiter("resource_request_success")  # (2)
        await waiter.wait()
    ```

    1. client: [CloudControlApiClient](./client.md)
    2. waiter: [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)


