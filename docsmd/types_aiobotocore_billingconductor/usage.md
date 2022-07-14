# Examples

> [Index](../README.md) > [BillingConductor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BillingConductor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
    type annotations stubs module [types-aiobotocore-billingconductor](https://pypi.org/project/types-aiobotocore-billingconductor/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[billingconductor]` package installed.

Write your `BillingConductor` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("billingconductor") as client:  # (1)
        result = await client.associate_accounts()  # (2)
    ```

    1. client: [BillingConductorClient](./client.md)
    2. result: [:material-code-braces: AssociateAccountsOutputTypeDef](./type_defs.md#associateaccountsoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("billingconductor") as client:  # (1)
        paginator = client.get_paginator("list_account_associations")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [BillingConductorClient](./client.md)
    2. paginator: [ListAccountAssociationsPaginator](./paginators.md#listaccountassociationspaginator)
    3. item: [:material-code-braces: ListAccountAssociationsOutputTypeDef](./type_defs.md#listaccountassociationsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[billingconductor]`
or a standalone `types_aiobotocore_billingconductor` package, you have to explicitly specify
`client: BillingConductorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_billingconductor.client import BillingConductorClient
    from types_aiobotocore_billingconductor.type_defs import AssociateAccountsOutputTypeDef
    from types_aiobotocore_billingconductor.type_defs import AssociateAccountsInputRequestTypeDef


    session = Session()

    client: BillingConductorClient
    async with session.client("billingconductor") as client:  # (1)
        kwargs: AssociateAccountsInputRequestTypeDef = {...}  # (2)
        result: AssociateAccountsOutputTypeDef = await client.associate_accounts(**kwargs)  # (3)
    ```

    1. client: [BillingConductorClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateAccountsInputRequestTypeDef](./type_defs.md#associateaccountsinputrequesttypedef) 
    3. result: [:material-code-braces: AssociateAccountsOutputTypeDef](./type_defs.md#associateaccountsoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_billingconductor.client import BillingConductorClient
    from types_aiobotocore_billingconductor.paginator import ListAccountAssociationsPaginator
    from types_aiobotocore_billingconductor.type_defs import ListAccountAssociationsOutputTypeDef


    session = Session()

    client: BillingConductorClient
    async with session.client("billingconductor") as client:  # (1)
        paginator: ListAccountAssociationsPaginator = client.get_paginator("list_account_associations")  # (2)
        async for item in paginator.paginate(...):
            item: ListAccountAssociationsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [BillingConductorClient](./client.md)
    2. paginator: [ListAccountAssociationsPaginator](./paginators.md#listaccountassociationspaginator)
    3. item: [:material-code-braces: ListAccountAssociationsOutputTypeDef](./type_defs.md#listaccountassociationsoutputtypedef) 




