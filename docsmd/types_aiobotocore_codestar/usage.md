# Examples

> [Index](../README.md) > [CodeStar](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeStar](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
    type annotations stubs module [types-aiobotocore-codestar](https://pypi.org/project/types-aiobotocore-codestar/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codestar]` package installed.

Write your `CodeStar` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codestar") as client:  # (1)
        result = await client.associate_team_member()  # (2)
    ```

    1. client: [CodeStarClient](./client.md)
    2. result: [:material-code-braces: AssociateTeamMemberResultTypeDef](./type_defs.md#associateteammemberresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codestar") as client:  # (1)
        paginator = client.get_paginator("list_projects")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CodeStarClient](./client.md)
    2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
    3. item: [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 




### Explicit type annotations

With `types-aioboto3-lite[codestar]`
or a standalone `types_aiobotocore_codestar` package, you have to explicitly specify
`client: CodeStarClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codestar.client import CodeStarClient
    from types_aiobotocore_codestar.type_defs import AssociateTeamMemberResultTypeDef
    from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef


    session = Session()

    client: CodeStarClient
    async with session.client("codestar") as client:  # (1)
        kwargs: AssociateTeamMemberRequestRequestTypeDef = {...}  # (2)
        result: AssociateTeamMemberResultTypeDef = await client.associate_team_member(**kwargs)  # (3)
    ```

    1. client: [CodeStarClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateTeamMemberRequestRequestTypeDef](./type_defs.md#associateteammemberrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateTeamMemberResultTypeDef](./type_defs.md#associateteammemberresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codestar.client import CodeStarClient
    from types_aiobotocore_codestar.paginator import ListProjectsPaginator
    from types_aiobotocore_codestar.type_defs import ListProjectsResultTypeDef


    session = Session()

    client: CodeStarClient
    async with session.client("codestar") as client:  # (1)
        paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
        async for item in paginator.paginate(...):
            item: ListProjectsResultTypeDef
            print(item)  # (3)
    ```

    1. client: [CodeStarClient](./client.md)
    2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
    3. item: [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 




