# Examples

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cognito-idp]` package installed.

Write your `CognitoIdentityProvider` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cognito-idp") as client:  # (1)
        result = await client.admin_add_user_to_group()  # (2)
    ```

    1. client: [CognitoIdentityProviderClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cognito-idp") as client:  # (1)
        paginator = client.get_paginator("admin_list_groups_for_user")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CognitoIdentityProviderClient](./client.md)
    2. paginator: [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
    3. item: [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cognito-idp]`
or a standalone `types_aiobotocore_cognito_idp` package, you have to explicitly specify
`client: CognitoIdentityProviderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient
    from types_aiobotocore_cognito_idp.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_cognito_idp.type_defs import AdminAddUserToGroupRequestRequestTypeDef


    session = Session()

    client: CognitoIdentityProviderClient
    async with session.client("cognito-idp") as client:  # (1)
        kwargs: AdminAddUserToGroupRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.admin_add_user_to_group(**kwargs)  # (3)
    ```

    1. client: [CognitoIdentityProviderClient](./client.md)
    2. kwargs: [:material-code-braces: AdminAddUserToGroupRequestRequestTypeDef](./type_defs.md#adminaddusertogrouprequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient
    from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator
    from types_aiobotocore_cognito_idp.type_defs import AdminListGroupsForUserResponseTypeDef


    session = Session()

    client: CognitoIdentityProviderClient
    async with session.client("cognito-idp") as client:  # (1)
        paginator: AdminListGroupsForUserPaginator = client.get_paginator("admin_list_groups_for_user")  # (2)
        async for item in paginator.paginate(...):
            item: AdminListGroupsForUserResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [CognitoIdentityProviderClient](./client.md)
    2. paginator: [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
    3. item: [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 




