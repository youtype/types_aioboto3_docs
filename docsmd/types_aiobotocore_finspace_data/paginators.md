# Paginators

> [Index](../README.md) > [FinSpaceData](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
    type annotations stubs module [types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

## ListChangesetsPaginator

Type annotations and code completion for `#!python session.client("finspace-data").get_paginator("list_changesets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListChangesets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_finspace_data.paginator import ListChangesetsPaginator

session = Session()

session = get_session()
async with session.client("finspace-data") as client:  # (1)
    paginator: ListChangesetsPaginator = client.get_paginator("list_changesets")  # (2)
    async for item in paginator.paginate(...):
        item: ListChangesetsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListChangesetsPaginator](./paginators.md#listchangesetspaginator)
3. item: [:material-code-braces: ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChangesetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListChangesetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChangesetsRequestListChangesetsPaginateTypeDef = {  # (1)
    "datasetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChangesetsRequestListChangesetsPaginateTypeDef](./type_defs.md#listchangesetsrequestlistchangesetspaginatetypedef) 
## ListDataViewsPaginator

Type annotations and code completion for `#!python session.client("finspace-data").get_paginator("list_data_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDataViews)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_finspace_data.paginator import ListDataViewsPaginator

session = Session()

session = get_session()
async with session.client("finspace-data") as client:  # (1)
    paginator: ListDataViewsPaginator = client.get_paginator("list_data_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataViewsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListDataViewsPaginator](./paginators.md#listdataviewspaginator)
3. item: [:material-code-braces: ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataViewsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataViewsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataViewsRequestListDataViewsPaginateTypeDef = {  # (1)
    "datasetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataViewsRequestListDataViewsPaginateTypeDef](./type_defs.md#listdataviewsrequestlistdataviewspaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.client("finspace-data").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDatasets)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_finspace_data.paginator import ListDatasetsPaginator

session = Session()

session = get_session()
async with session.client("finspace-data") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListPermissionGroupsPaginator

Type annotations and code completion for `#!python session.client("finspace-data").get_paginator("list_permission_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListPermissionGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_finspace_data.paginator import ListPermissionGroupsPaginator

session = Session()

session = get_session()
async with session.client("finspace-data") as client:  # (1)
    paginator: ListPermissionGroupsPaginator = client.get_paginator("list_permission_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListPermissionGroupsPaginator](./paginators.md#listpermissiongroupspaginator)
3. item: [:material-code-braces: ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPermissionGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef](./type_defs.md#listpermissiongroupsrequestlistpermissiongroupspaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.client("finspace-data").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListUsers)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_finspace_data.paginator import ListUsersPaginator

session = Session()

session = get_session()
async with session.client("finspace-data") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [FinSpaceDataClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsersRequestListUsersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef) 
