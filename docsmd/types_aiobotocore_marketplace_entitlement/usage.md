# Examples

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[marketplace-entitlement]` package installed.

Write your `MarketplaceEntitlementService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("marketplace-entitlement") as client:  # (1)
        result = await client.get_entitlements()  # (2)
    ```

    1. client: [MarketplaceEntitlementServiceClient](./client.md)
    2. result: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("marketplace-entitlement") as client:  # (1)
        paginator = client.get_paginator("get_entitlements")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MarketplaceEntitlementServiceClient](./client.md)
    2. paginator: [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)
    3. item: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[marketplace-entitlement]`
or a standalone `types_aiobotocore_marketplace_entitlement` package, you have to explicitly specify
`client: MarketplaceEntitlementServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
    from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsResultTypeDef
    from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsRequestRequestTypeDef


    session = Session()

    client: MarketplaceEntitlementServiceClient
    async with session.client("marketplace-entitlement") as client:  # (1)
        kwargs: GetEntitlementsRequestRequestTypeDef = {...}  # (2)
        result: GetEntitlementsResultTypeDef = await client.get_entitlements(**kwargs)  # (3)
    ```

    1. client: [MarketplaceEntitlementServiceClient](./client.md)
    2. kwargs: [:material-code-braces: GetEntitlementsRequestRequestTypeDef](./type_defs.md#getentitlementsrequestrequesttypedef) 
    3. result: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
    from types_aiobotocore_marketplace_entitlement.paginator import GetEntitlementsPaginator
    from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsResultTypeDef


    session = Session()

    client: MarketplaceEntitlementServiceClient
    async with session.client("marketplace-entitlement") as client:  # (1)
        paginator: GetEntitlementsPaginator = client.get_paginator("get_entitlements")  # (2)
        async for item in paginator.paginate(...):
            item: GetEntitlementsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [MarketplaceEntitlementServiceClient](./client.md)
    2. paginator: [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)
    3. item: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 




