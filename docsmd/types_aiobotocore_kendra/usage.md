# Examples

> [Index](../README.md) > [kendra](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [kendra](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
    type annotations stubs module [types-aiobotocore-kendra](https://pypi.org/project/types-aiobotocore-kendra/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[kendra]` package installed.

Write your `kendra` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("kendra") as client:  # (1)
        result = await client.associate_entities_to_experience()  # (2)
    ```

    1. client: [kendraClient](./client.md)
    2. result: [:material-code-braces: AssociateEntitiesToExperienceResponseTypeDef](./type_defs.md#associateentitiestoexperienceresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[kendra]`
or a standalone `types_aiobotocore_kendra` package, you have to explicitly specify
`client: kendraClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_kendra.client import kendraClient
    from types_aiobotocore_kendra.type_defs import AssociateEntitiesToExperienceResponseTypeDef
    from types_aiobotocore_kendra.type_defs import AssociateEntitiesToExperienceRequestRequestTypeDef


    session = Session()

    client: kendraClient
    async with session.client("kendra") as client:  # (1)
        kwargs: AssociateEntitiesToExperienceRequestRequestTypeDef = {...}  # (2)
        result: AssociateEntitiesToExperienceResponseTypeDef = await client.associate_entities_to_experience(**kwargs)  # (3)
    ```

    1. client: [kendraClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateEntitiesToExperienceRequestRequestTypeDef](./type_defs.md#associateentitiestoexperiencerequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateEntitiesToExperienceResponseTypeDef](./type_defs.md#associateentitiestoexperienceresponsetypedef) 






