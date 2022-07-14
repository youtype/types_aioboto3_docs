# Examples

> [Index](../README.md) > [Account](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[account]` package installed.

Write your `Account` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("account") as client:  # (1)
        result = await client.delete_alternate_contact()  # (2)
    ```

    1. client: [AccountClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aioboto3-lite[account]`
or a standalone `types_aiobotocore_account` package, you have to explicitly specify
`client: AccountClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_account.client import AccountClient
    from types_aiobotocore_account.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_account.type_defs import DeleteAlternateContactRequestRequestTypeDef


    session = Session()

    client: AccountClient
    async with session.client("account") as client:  # (1)
        kwargs: DeleteAlternateContactRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.delete_alternate_contact(**kwargs)  # (3)
    ```

    1. client: [AccountClient](./client.md)
    2. kwargs: [:material-code-braces: DeleteAlternateContactRequestRequestTypeDef](./type_defs.md#deletealternatecontactrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






