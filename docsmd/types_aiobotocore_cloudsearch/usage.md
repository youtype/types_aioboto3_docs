# Examples

> [Index](../README.md) > [CloudSearch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
    type annotations stubs module [types-aiobotocore-cloudsearch](https://pypi.org/project/types-aiobotocore-cloudsearch/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudsearch]` package installed.

Write your `CloudSearch` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("cloudsearch") as client:  # (1)
        result = await client.build_suggesters()  # (2)
    ```

    1. client: [CloudSearchClient](./client.md)
    2. result: [:material-code-braces: BuildSuggestersResponseTypeDef](./type_defs.md#buildsuggestersresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[cloudsearch]`
or a standalone `types_aiobotocore_cloudsearch` package, you have to explicitly specify
`client: CloudSearchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_cloudsearch.client import CloudSearchClient
    from types_aiobotocore_cloudsearch.type_defs import BuildSuggestersResponseTypeDef
    from types_aiobotocore_cloudsearch.type_defs import BuildSuggestersRequestRequestTypeDef


    session = Session()

    client: CloudSearchClient
    async with session.client("cloudsearch") as client:  # (1)
        kwargs: BuildSuggestersRequestRequestTypeDef = {...}  # (2)
        result: BuildSuggestersResponseTypeDef = await client.build_suggesters(**kwargs)  # (3)
    ```

    1. client: [CloudSearchClient](./client.md)
    2. kwargs: [:material-code-braces: BuildSuggestersRequestRequestTypeDef](./type_defs.md#buildsuggestersrequestrequesttypedef) 
    3. result: [:material-code-braces: BuildSuggestersResponseTypeDef](./type_defs.md#buildsuggestersresponsetypedef) 






