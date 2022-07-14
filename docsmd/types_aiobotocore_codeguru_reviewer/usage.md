# Examples

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codeguru-reviewer]` package installed.

Write your `CodeGuruReviewer` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codeguru-reviewer") as client:  # (1)
        result = await client.associate_repository()  # (2)
    ```

    1. client: [CodeGuruReviewerClient](./client.md)
    2. result: [:material-code-braces: AssociateRepositoryResponseTypeDef](./type_defs.md#associaterepositoryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codeguru-reviewer") as client:  # (1)
        paginator = client.get_paginator("list_repository_associations")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CodeGuruReviewerClient](./client.md)
    2. paginator: [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)
    3. item: [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("codeguru-reviewer") as client:  # (1)
        waiter = client.get_waiter("code_review_completed")  # (2)
        await waiter.wait()
    ```

    1. client: [CodeGuruReviewerClient](./client.md)
    2. waiter: [CodeReviewCompletedWaiter](./waiters.md#codereviewcompletedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[codeguru-reviewer]`
or a standalone `types_aiobotocore_codeguru_reviewer` package, you have to explicitly specify
`client: CodeGuruReviewerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
    from types_aiobotocore_codeguru_reviewer.type_defs import AssociateRepositoryResponseTypeDef
    from types_aiobotocore_codeguru_reviewer.type_defs import AssociateRepositoryRequestRequestTypeDef


    session = Session()

    client: CodeGuruReviewerClient
    async with session.client("codeguru-reviewer") as client:  # (1)
        kwargs: AssociateRepositoryRequestRequestTypeDef = {...}  # (2)
        result: AssociateRepositoryResponseTypeDef = await client.associate_repository(**kwargs)  # (3)
    ```

    1. client: [CodeGuruReviewerClient](./client.md)
    2. kwargs: [:material-code-braces: AssociateRepositoryRequestRequestTypeDef](./type_defs.md#associaterepositoryrequestrequesttypedef) 
    3. result: [:material-code-braces: AssociateRepositoryResponseTypeDef](./type_defs.md#associaterepositoryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
    from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator
    from types_aiobotocore_codeguru_reviewer.type_defs import ListRepositoryAssociationsResponseTypeDef


    session = Session()

    client: CodeGuruReviewerClient
    async with session.client("codeguru-reviewer") as client:  # (1)
        paginator: ListRepositoryAssociationsPaginator = client.get_paginator("list_repository_associations")  # (2)
        async for item in paginator.paginate(...):
            item: ListRepositoryAssociationsResponseTypeDef
            print(item)  # (3)
    ```

    1. client: [CodeGuruReviewerClient](./client.md)
    2. paginator: [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)
    3. item: [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
    from types_aiobotocore_codeguru_reviewer.waiter import CodeReviewCompletedWaiter


    session = Session()

    async with session.client("codeguru-reviewer") as client:  # (1)
        waiter = client.get_waiter("code_review_completed")  # (2)
        await waiter.wait()
    ```

    1. client: [CodeGuruReviewerClient](./client.md)
    2. waiter: [CodeReviewCompletedWaiter](./waiters.md#codereviewcompletedwaiter)


