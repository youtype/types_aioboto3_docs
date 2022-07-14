# Paginators

> [Index](../README.md) > [ResourceGroups](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## ListGroupResourcesPaginator

Type annotations and code completion for `#!python session.client("resource-groups").get_paginator("list_group_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator

session = Session()

session = get_session()
async with session.client("resource-groups") as client:  # (1)
    paginator: ListGroupResourcesPaginator = client.get_paginator("list_group_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
3. item: [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GroupName: str = ...,
    Group: str = ...,
    Filters: Sequence[ResourceFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListGroupResourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupResourcesInputListGroupResourcesPaginateTypeDef = {  # (1)
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupResourcesInputListGroupResourcesPaginateTypeDef](./type_defs.md#listgroupresourcesinputlistgroupresourcespaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.client("resource-groups").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_resource_groups.paginator import ListGroupsPaginator

session = Session()

session = get_session()
async with session.client("resource-groups") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[GroupFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListGroupsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: GroupFilterTypeDef](./type_defs.md#groupfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGroupsInputListGroupsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsInputListGroupsPaginateTypeDef](./type_defs.md#listgroupsinputlistgroupspaginatetypedef) 
## SearchResourcesPaginator

Type annotations and code completion for `#!python session.client("resource-groups").get_paginator("search_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_resource_groups.paginator import SearchResourcesPaginator

session = Session()

session = get_session()
async with session.client("resource-groups") as client:  # (1)
    paginator: SearchResourcesPaginator = client.get_paginator("search_resources")  # (2)
    async for item in paginator.paginate(...):
        item: SearchResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)
3. item: [:material-code-braces: SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python SearchResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchResourcesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: SearchResourcesInputSearchResourcesPaginateTypeDef = {  # (1)
    "ResourceQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchResourcesInputSearchResourcesPaginateTypeDef](./type_defs.md#searchresourcesinputsearchresourcespaginatetypedef) 
