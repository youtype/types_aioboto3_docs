# Examples

> [Index](../README.md) > [Macie](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
    type annotations stubs module [types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[macie]` package installed.

Write your `Macie` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("macie") as client:  # (1)
        result = await client.associate_member_account()  # (2)
    ```

    1. client: [MacieClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("macie") as client:  # (1)
        paginator = client.get_paginator("list_member_accounts")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MacieClient](./client.md)
    2. paginator: [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
    3. item: [:material-code-braces: ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[macie]`
or a standalone `types_aiobotocore_macie` package, you have to explicitly specify
`client: MacieClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_macie.client import MacieClient
    from types_aiobotocore_macie.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef


    session = Session()

    client: MacieClient
    async with session.client("macie") as client:  # (1)
        kwargs: AssociateMemberAccountRequestRequestTypeDef = {...}  # (2)
        result: EmptyResponseMetadataTypeDef = await client.associate_member_account(**kwargs)  # (3)
    ```

    1. client: [MacieClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateMemberAccountRequestRequestTypeDef](./type_defs.md#associatememberaccountrequestrequesttypedef) 
    3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_macie.client import MacieClient
    from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator
    from types_aiobotocore_macie.type_defs import ListMemberAccountsResultTypeDef


    session = Session()

    client: MacieClient
    async with session.client("macie") as client:  # (1)
        paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")  # (2)
        async for item in paginator.paginate(...):
            item: ListMemberAccountsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [MacieClient](./client.md)
    2. paginator: [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
    3. item: [:material-code-braces: ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef) 




