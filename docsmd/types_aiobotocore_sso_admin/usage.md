# Examples

> [Index](../README.md) > [SSOAdmin](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
    type annotations stubs module [types-aiobotocore-sso-admin](https://pypi.org/project/types-aiobotocore-sso-admin/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sso-admin]` package installed.

Write your `SSOAdmin` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sso-admin") as client:  # (1)
        result = await client.create_account_assignment()  # (2)
    ```

    1. client: [SSOAdminClient](./client.md)
    2. result: [:material-code-braces: CreateAccountAssignmentResponseTypeDef](./type_defs.md#createaccountassignmentresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("sso-admin") as client:  # (1)
        paginator = client.get_paginator("list_account_assignment_creation_status")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [SSOAdminClient](./client.md)
    2. paginator: [ListAccountAssignmentCreationStatusPaginator](./paginators.md#listaccountassignmentcreationstatuspaginator)
    3. item: [:material-code-braces: ListAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#listaccountassignmentcreationstatusresponsetypedef) 




### Explicit type annotations

With `types-aioboto3-lite[sso-admin]`
or a standalone `types_aiobotocore_sso_admin` package, you have to explicitly specify
`client: SSOAdminClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sso_admin.client import SSOAdminClient
    from types_aiobotocore_sso_admin.type_defs import CreateAccountAssignmentResponseTypeDef
    from types_aiobotocore_sso_admin.type_defs import CreateAccountAssignmentRequestRequestTypeDef


    session = Session()

    client: SSOAdminClient
    async with session.client("sso-admin") as client:  # (1)
        kwargs: CreateAccountAssignmentRequestRequestTypeDef = {...}  # (2)
        result: CreateAccountAssignmentResponseTypeDef = await client.create_account_assignment(**kwargs)  # (3)
    ```

    1. client: [SSOAdminClient](./client.md)
    2. kwargs: [:material-code-braces: CreateAccountAssignmentRequestRequestTypeDef](./type_defs.md#createaccountassignmentrequestrequesttypedef) 
    3. result: [:material-code-braces: CreateAccountAssignmentResponseTypeDef](./type_defs.md#createaccountassignmentresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_sso_admin.client import SSOAdminClient
    from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentCreationStatusPaginator
    from types_aiobotocore_sso_admin.type_defs import ListAccountAssignmentCreationStatusResponseTypeDef


    session = Session()

    client: SSOAdminClient
    async with session.client("sso-admin") as client:  # (1)
        paginator: ListAccountAssignmentCreationStatusPaginator = client.get_paginator("list_account_assignment_creation_status")  # (2)
        async for item in paginator.paginate(...):
            item: ListAccountAssignmentCreationStatusResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [SSOAdminClient](./client.md)
    2. paginator: [ListAccountAssignmentCreationStatusPaginator](./paginators.md#listaccountassignmentcreationstatuspaginator)
    3. item: [:material-code-braces: ListAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#listaccountassignmentcreationstatusresponsetypedef) 




