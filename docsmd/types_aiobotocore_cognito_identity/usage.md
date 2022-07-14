# Examples

> [Index](../README.md) > [CognitoIdentity](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
    type annotations stubs module [types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cognito-identity]` package installed.

Write your `CognitoIdentity` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cognito-identity") as client:  # (1)
        result = await client.create_identity_pool()  # (2)
    ```

    1. client: [CognitoIdentityClient](./client.md)
    2. result: [:material-code-braces: IdentityPoolTypeDef](./type_defs.md#identitypooltypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cognito-identity") as client:  # (1)
        paginator = client.get_paginator("list_identity_pools")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CognitoIdentityClient](./client.md)
    2. paginator: [ListIdentityPoolsPaginator](./paginators.md#listidentitypoolspaginator)
    3. item: [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[cognito-identity]`
or a standalone `types_aiobotocore_cognito_identity` package, you have to explicitly specify
`client: CognitoIdentityClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cognito_identity.client import CognitoIdentityClient
    from types_aiobotocore_cognito_identity.type_defs import IdentityPoolTypeDef
    from types_aiobotocore_cognito_identity.type_defs import CreateIdentityPoolInputRequestTypeDef


    session = Session()

    client: CognitoIdentityClient
    async with session.client("cognito-identity") as client:  # (1)
        kwargs: CreateIdentityPoolInputRequestTypeDef = {...}  # (2)
        result: IdentityPoolTypeDef = await client.create_identity_pool(**kwargs)  # (3)
    ```

    1. client: [CognitoIdentityClient](./client.md)
    2. kwargs: [:material-code-braces: CreateIdentityPoolInputRequestTypeDef](./type_defs.md#createidentitypoolinputrequesttypedef) 
    3. result: [:material-code-braces: IdentityPoolTypeDef](./type_defs.md#identitypooltypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cognito_identity.client import CognitoIdentityClient
    from types_aiobotocore_cognito_identity.paginator import ListIdentityPoolsPaginator
    from types_aiobotocore_cognito_identity.type_defs import ListIdentityPoolsResponseTypeDef


    session = Session()

    client: CognitoIdentityClient
    async with session.client("cognito-identity") as client:  # (1)
        paginator: ListIdentityPoolsPaginator = client.get_paginator("list_identity_pools")  # (2)
        async for item in paginator.paginate(...):
            item: ListIdentityPoolsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [CognitoIdentityClient](./client.md)
    2. paginator: [ListIdentityPoolsPaginator](./paginators.md#listidentitypoolspaginator)
    3. item: [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 




