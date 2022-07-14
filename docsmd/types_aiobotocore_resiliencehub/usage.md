# Examples

> [Index](../README.md) > [ResilienceHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
    type annotations stubs module [types-aiobotocore-resiliencehub](https://pypi.org/project/types-aiobotocore-resiliencehub/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[resiliencehub]` package installed.

Write your `ResilienceHub` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("resiliencehub") as client:  # (1)
        result = await client.add_draft_app_version_resource_mappings()  # (2)
    ```

    1. client: [ResilienceHubClient](./client.md)
    2. result: [:material-code-braces: AddDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#adddraftappversionresourcemappingsresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[resiliencehub]`
or a standalone `types_aiobotocore_resiliencehub` package, you have to explicitly specify
`client: ResilienceHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_resiliencehub.client import ResilienceHubClient
    from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsResponseTypeDef
    from types_aiobotocore_resiliencehub.type_defs import AddDraftAppVersionResourceMappingsRequestRequestTypeDef


    session = Session()

    client: ResilienceHubClient
    async with session.client("resiliencehub") as client:  # (1)
        kwargs: AddDraftAppVersionResourceMappingsRequestRequestTypeDef = {...}  # (2)
        result: AddDraftAppVersionResourceMappingsResponseTypeDef = await client.add_draft_app_version_resource_mappings(**kwargs)  # (3)
    ```

    1. client: [ResilienceHubClient](./client.md)
    2. kwargs: [:material-code-braces: AddDraftAppVersionResourceMappingsRequestRequestTypeDef](./type_defs.md#adddraftappversionresourcemappingsrequestrequesttypedef) 
    3. result: [:material-code-braces: AddDraftAppVersionResourceMappingsResponseTypeDef](./type_defs.md#adddraftappversionresourcemappingsresponsetypedef) 






