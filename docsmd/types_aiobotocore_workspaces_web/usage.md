# Examples

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[workspaces-web]` package installed.

Write your `WorkSpacesWeb` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("workspaces-web") as client:  # (1)
        result = await client.associate_browser_settings()  # (2)
    ```

    1. client: [WorkSpacesWebClient](./client.md)
    2. result: [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[workspaces-web]`
or a standalone `types_aiobotocore_workspaces_web` package, you have to explicitly specify
`client: WorkSpacesWebClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_workspaces_web.client import WorkSpacesWebClient
    from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsResponseTypeDef
    from types_aiobotocore_workspaces_web.type_defs import AssociateBrowserSettingsRequestRequestTypeDef


    session = Session()

    client: WorkSpacesWebClient
    async with session.client("workspaces-web") as client:  # (1)
        kwargs: AssociateBrowserSettingsRequestRequestTypeDef = {...}  # (2)
        result: AssociateBrowserSettingsResponseTypeDef = await client.associate_browser_settings(**kwargs)  # (3)
    ```

    1. client: [WorkSpacesWebClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateBrowserSettingsRequestRequestTypeDef](./type_defs.md#associatebrowsersettingsrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateBrowserSettingsResponseTypeDef](./type_defs.md#associatebrowsersettingsresponsetypedef) 






