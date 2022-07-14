# Paginators

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

## ListRepositoryAssociationsPaginator

Type annotations and code completion for `#!python session.client("codeguru-reviewer").get_paginator("list_repository_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator

session = Session()

session = get_session()
async with session.client("codeguru-reviewer") as client:  # (1)
    paginator: ListRepositoryAssociationsPaginator = client.get_paginator("list_repository_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRepositoryAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruReviewerClient](./client.md)
2. paginator: [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)
3. item: [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRepositoryAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProviderTypes: Sequence[ProviderTypeType] = ...,  # (1)
    States: Sequence[RepositoryAssociationStateType] = ...,  # (2)
    Names: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListRepositoryAssociationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = {  # (1)
    "ProviderTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef](./type_defs.md#listrepositoryassociationsrequestlistrepositoryassociationspaginatetypedef) 
