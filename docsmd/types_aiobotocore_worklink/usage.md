# Examples

> [Index](../README.md) > [WorkLink](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkLink](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
    type annotations stubs module [types-aiobotocore-worklink](https://pypi.org/project/types-aiobotocore-worklink/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[worklink]` package installed.

Write your `WorkLink` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("worklink") as client:  # (1)
        result = await client.associate_website_authorization_provider()  # (2)
    ```

    1. client: [WorkLinkClient](./client.md)
    2. result: [:material-code-braces: AssociateWebsiteAuthorizationProviderResponseTypeDef](./type_defs.md#associatewebsiteauthorizationproviderresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[worklink]`
or a standalone `types_aiobotocore_worklink` package, you have to explicitly specify
`client: WorkLinkClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_worklink.client import WorkLinkClient
    from types_aiobotocore_worklink.type_defs import AssociateWebsiteAuthorizationProviderResponseTypeDef
    from types_aiobotocore_worklink.type_defs import AssociateWebsiteAuthorizationProviderRequestRequestTypeDef


    session = Session()

    client: WorkLinkClient
    async with session.client("worklink") as client:  # (1)
        kwargs: AssociateWebsiteAuthorizationProviderRequestRequestTypeDef = {...}  # (2)
        result: AssociateWebsiteAuthorizationProviderResponseTypeDef = await client.associate_website_authorization_provider(**kwargs)  # (3)
    ```

    1. client: [WorkLinkClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateWebsiteAuthorizationProviderRequestRequestTypeDef](./type_defs.md#associatewebsiteauthorizationproviderrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateWebsiteAuthorizationProviderResponseTypeDef](./type_defs.md#associatewebsiteauthorizationproviderresponsetypedef) 






