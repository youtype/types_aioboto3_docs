# Paginators

> [Index](../README.md) > [IoT1ClickProjects](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#iot1clickprojects)
    type annotations stubs module [types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

## ListPlacementsPaginator

Type annotations and code completion for `#!python session.client("iot1click-projects").get_paginator("list_placements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects/paginator/ListPlacements.html#IoT1ClickProjects.Paginator.ListPlacements)

```python
# ListPlacementsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_iot1click_projects.paginator import ListPlacementsPaginator

session = Session()

session = get_session()
async with session.client("iot1click-projects") as client:  # (1)
    paginator: ListPlacementsPaginator = client.get_paginator("list_placements")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlacementsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoT1ClickProjectsClient](./client.md)
2. paginator: [ListPlacementsPaginator](./paginators.md#listplacementspaginator)
3. item: [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlacementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPlacementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPlacementsRequestPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlacementsRequestPaginateTypeDef](./type_defs.md#listplacementsrequestpaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("iot1click-projects").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects/paginator/ListProjects.html#IoT1ClickProjects.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_iot1click_projects.paginator import ListProjectsPaginator

session = Session()

session = get_session()
async with session.client("iot1click-projects") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoT1ClickProjectsClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef) 