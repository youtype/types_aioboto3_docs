# Examples

> [Index](../README.md) > [Route53](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
    type annotations stubs module [types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[route53]` package installed.

Write your `Route53` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("route53") as client:  # (1)
        result = await client.activate_key_signing_key()  # (2)
    ```

    1. client: [Route53Client](./client.md)
    2. result: [:material-code-braces: ActivateKeySigningKeyResponseTypeDef](./type_defs.md#activatekeysigningkeyresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("route53") as client:  # (1)
        paginator = client.get_paginator("list_health_checks")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [Route53Client](./client.md)
    2. paginator: [ListHealthChecksPaginator](./paginators.md#listhealthcheckspaginator)
    3. item: [:material-code-braces: ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("route53") as client:  # (1)
        waiter = client.get_waiter("resource_record_sets_changed")  # (2)
        await waiter.wait()
    ```

    1. client: [Route53Client](./client.md)
    2. waiter: [ResourceRecordSetsChangedWaiter](./waiters.md#resourcerecordsetschangedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[route53]`
or a standalone `types_aiobotocore_route53` package, you have to explicitly specify
`client: Route53Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_route53.client import Route53Client
    from types_aiobotocore_route53.type_defs import ActivateKeySigningKeyResponseTypeDef
    from types_aiobotocore_route53.type_defs import ActivateKeySigningKeyRequestRequestTypeDef


    session = Session()

    client: Route53Client
    async with session.client("route53") as client:  # (1)
        kwargs: ActivateKeySigningKeyRequestRequestTypeDef = {...}  # (2)
        result: ActivateKeySigningKeyResponseTypeDef = await client.activate_key_signing_key(**kwargs)  # (3)
    ```

    1. client: [Route53Client](./client.md)
    2. kwargs: [:material-code-braces: ActivateKeySigningKeyRequestRequestTypeDef](./type_defs.md#activatekeysigningkeyrequestrequesttypedef) 
    3. result: [:material-code-braces: ActivateKeySigningKeyResponseTypeDef](./type_defs.md#activatekeysigningkeyresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_route53.client import Route53Client
    from types_aiobotocore_route53.paginator import ListHealthChecksPaginator
    from types_aiobotocore_route53.type_defs import ListHealthChecksResponseTypeDef


    session = Session()

    client: Route53Client
    async with session.client("route53") as client:  # (1)
        paginator: ListHealthChecksPaginator = client.get_paginator("list_health_checks")  # (2)
        async for item in paginator.paginate(...):
            item: ListHealthChecksResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [Route53Client](./client.md)
    2. paginator: [ListHealthChecksPaginator](./paginators.md#listhealthcheckspaginator)
    3. item: [:material-code-braces: ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_route53.client import Route53Client
    from types_aiobotocore_route53.waiter import ResourceRecordSetsChangedWaiter


    session = Session()

    async with session.client("route53") as client:  # (1)
        waiter = client.get_waiter("resource_record_sets_changed")  # (2)
        await waiter.wait()
    ```

    1. client: [Route53Client](./client.md)
    2. waiter: [ResourceRecordSetsChangedWaiter](./waiters.md#resourcerecordsetschangedwaiter)


