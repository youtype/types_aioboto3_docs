# Examples

> [Index](../README.md) > [SSOOIDC](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
    type annotations stubs module [types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sso-oidc]` package installed.

Write your `SSOOIDC` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sso-oidc") as client:  # (1)
        result = await client.create_token()  # (2)
    ```

    1. client: [SSOOIDCClient](./client.md)
    2. result: [:material-code-braces: CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[sso-oidc]`
or a standalone `types_aiobotocore_sso_oidc` package, you have to explicitly specify
`client: SSOOIDCClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sso_oidc.client import SSOOIDCClient
    from types_aiobotocore_sso_oidc.type_defs import CreateTokenResponseTypeDef
    from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef


    session = Session()

    client: SSOOIDCClient
    async with session.client("sso-oidc") as client:  # (1)
        kwargs: CreateTokenRequestRequestTypeDef = {...}  # (2)
        result: CreateTokenResponseTypeDef = await client.create_token(**kwargs)  # (3)
    ```

    1. client: [SSOOIDCClient](./client.md)
    2. kwargs: [:material-code-braces: CreateTokenRequestRequestTypeDef](./type_defs.md#createtokenrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef) 






