# Examples

> [Index](../README.md) > [RAM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
    type annotations stubs module [types-aiobotocore-ram](https://pypi.org/project/types-aiobotocore-ram/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ram]` package installed.

Write your `RAM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ram") as client:  # (1)
        result = await client.accept_resource_share_invitation()  # (2)
    ```

    1. client: [RAMClient](./client.md)
    2. result: [:material-code-braces: AcceptResourceShareInvitationResponseTypeDef](./type_defs.md#acceptresourceshareinvitationresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("ram") as client:  # (1)
        paginator = client.get_paginator("get_resource_policies")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [RAMClient](./client.md)
    2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
    3. item: [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[ram]`
or a standalone `types_aiobotocore_ram` package, you have to explicitly specify
`client: RAMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ram.client import RAMClient
    from types_aiobotocore_ram.type_defs import AcceptResourceShareInvitationResponseTypeDef
    from types_aiobotocore_ram.type_defs import AcceptResourceShareInvitationRequestRequestTypeDef


    session = Session()

    client: RAMClient
    async with session.client("ram") as client:  # (1)
        kwargs: AcceptResourceShareInvitationRequestRequestTypeDef = {...}  # (2)
        result: AcceptResourceShareInvitationResponseTypeDef = await client.accept_resource_share_invitation(**kwargs)  # (3)
    ```

    1. client: [RAMClient](./client.md)
    2. kwargs: [:material-code-braces: AcceptResourceShareInvitationRequestRequestTypeDef](./type_defs.md#acceptresourceshareinvitationrequestrequesttypedef) 
    3. result: [:material-code-braces: AcceptResourceShareInvitationResponseTypeDef](./type_defs.md#acceptresourceshareinvitationresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_ram.client import RAMClient
    from types_aiobotocore_ram.paginator import GetResourcePoliciesPaginator
    from types_aiobotocore_ram.type_defs import GetResourcePoliciesResponseTypeDef


    session = Session()

    client: RAMClient
    async with session.client("ram") as client:  # (1)
        paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")  # (2)
        async for item in paginator.paginate(...):
            item: GetResourcePoliciesResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [RAMClient](./client.md)
    2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
    3. item: [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 




