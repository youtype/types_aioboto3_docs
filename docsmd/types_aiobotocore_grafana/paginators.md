# Paginators

> [Index](../README.md) > [ManagedGrafana](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## ListPermissionsPaginator

Type annotations and code completion for `#!python session.client("grafana").get_paginator("list_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_grafana.paginator import ListPermissionsPaginator

session = Session()

session = get_session()
async with session.client("grafana") as client:  # (1)
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
3. item: [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    workspaceId: str,
    groupId: str = ...,
    userId: str = ...,
    userType: UserTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPermissionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPermissionsRequestListPermissionsPaginateTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionsRequestListPermissionsPaginateTypeDef](./type_defs.md#listpermissionsrequestlistpermissionspaginatetypedef) 
## ListWorkspacesPaginator

Type annotations and code completion for `#!python session.client("grafana").get_paginator("list_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_grafana.paginator import ListWorkspacesPaginator

session = Session()

session = get_session()
async with session.client("grafana") as client:  # (1)
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspacesResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedGrafanaClient](./client.md)
2. paginator: [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)
3. item: [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkspacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkspacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorkspacesRequestListWorkspacesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestListWorkspacesPaginateTypeDef](./type_defs.md#listworkspacesrequestlistworkspacespaginatetypedef) 
