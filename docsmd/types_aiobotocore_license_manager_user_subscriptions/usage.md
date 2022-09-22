# Examples

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[license-manager-user-subscriptions]` package installed.

Write your `LicenseManagerUserSubscriptions` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("license-manager-user-subscriptions") as client:  # (1)
        result = await client.associate_user()  # (2)
    ```

    1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
    2. result: [:material-code-braces: AssociateUserResponseTypeDef](./type_defs.md#associateuserresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("license-manager-user-subscriptions") as client:  # (1)
        paginator = client.get_paginator("list_identity_providers")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
    2. paginator: [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
    3. item: [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[license-manager-user-subscriptions]`
or a standalone `types_aiobotocore_license_manager_user_subscriptions` package, you have to explicitly specify
`client: LicenseManagerUserSubscriptionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
    from types_aiobotocore_license_manager_user_subscriptions.type_defs import AssociateUserResponseTypeDef
    from types_aiobotocore_license_manager_user_subscriptions.type_defs import AssociateUserRequestRequestTypeDef


    session = Session()

    client: LicenseManagerUserSubscriptionsClient
    async with session.client("license-manager-user-subscriptions") as client:  # (1)
        kwargs: AssociateUserRequestRequestTypeDef = {...}  # (2)
        result: AssociateUserResponseTypeDef = await client.associate_user(**kwargs)  # (3)
    ```

    1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateUserRequestRequestTypeDef](./type_defs.md#associateuserrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateUserResponseTypeDef](./type_defs.md#associateuserresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
    from types_aiobotocore_license_manager_user_subscriptions.paginator import ListIdentityProvidersPaginator
    from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListIdentityProvidersResponseTypeDef


    session = Session()

    client: LicenseManagerUserSubscriptionsClient
    async with session.client("license-manager-user-subscriptions") as client:  # (1)
        paginator: ListIdentityProvidersPaginator = client.get_paginator("list_identity_providers")  # (2)
        async for item in paginator.paginate(...):
            item: ListIdentityProvidersResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
    2. paginator: [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
    3. item: [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 




