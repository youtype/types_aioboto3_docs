# Paginators

> [Index](../README.md) > [Mobile](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Mobile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
    type annotations stubs module [types-aiobotocore-mobile](https://pypi.org/project/types-aiobotocore-mobile/).

## ListBundlesPaginator

Type annotations and code completion for `#!python session.client("mobile").get_paginator("list_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListBundles)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mobile.paginator import ListBundlesPaginator

session = Session()

session = get_session()
async with session.client("mobile") as client:  # (1)
    paginator: ListBundlesPaginator = client.get_paginator("list_bundles")  # (2)
    async for item in paginator.paginate(...):
        item: ListBundlesResultTypeDef
        print(item)  # (3)
```

1. client: [MobileClient](./client.md)
2. paginator: [ListBundlesPaginator](./paginators.md#listbundlespaginator)
3. item: [:material-code-braces: ListBundlesResultTypeDef](./type_defs.md#listbundlesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListBundlesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBundlesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBundlesResultTypeDef](./type_defs.md#listbundlesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListBundlesRequestListBundlesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBundlesRequestListBundlesPaginateTypeDef](./type_defs.md#listbundlesrequestlistbundlespaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.client("mobile").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListProjects)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mobile.paginator import ListProjectsPaginator

session = Session()

session = get_session()
async with session.client("mobile") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResultTypeDef
        print(item)  # (3)
```

1. client: [MobileClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
