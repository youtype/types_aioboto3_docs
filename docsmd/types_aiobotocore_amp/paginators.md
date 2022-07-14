# Paginators

> [Index](../README.md) > [PrometheusService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## ListRuleGroupsNamespacesPaginator

Type annotations and code completion for `#!python session.client("amp").get_paginator("list_rule_groups_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Paginator.ListRuleGroupsNamespaces)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator

session = Session()

session = get_session()
async with session.client("amp") as client:  # (1)
    paginator: ListRuleGroupsNamespacesPaginator = client.get_paginator("list_rule_groups_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
3. item: [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRuleGroupsNamespacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    workspaceId: str,
    name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRuleGroupsNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsNamespacesRequestListRuleGroupsNamespacesPaginateTypeDef](./type_defs.md#listrulegroupsnamespacesrequestlistrulegroupsnamespacespaginatetypedef) 
## ListWorkspacesPaginator

Type annotations and code completion for `#!python session.client("amp").get_paginator("list_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Paginator.ListWorkspaces)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_amp.paginator import ListWorkspacesPaginator

session = Session()

session = get_session()
async with session.client("amp") as client:  # (1)
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspacesResponseTypeDef
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)
3. item: [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkspacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    alias: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkspacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorkspacesRequestListWorkspacesPaginateTypeDef = {  # (1)
    "alias": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestListWorkspacesPaginateTypeDef](./type_defs.md#listworkspacesrequestlistworkspacespaginatetypedef) 
