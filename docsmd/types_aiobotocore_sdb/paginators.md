# Paginators

> [Index](../README.md) > [SimpleDB](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
    type annotations stubs module [types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

## ListDomainsPaginator

Type annotations and code completion for `#!python session.client("sdb").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sdb.paginator import ListDomainsPaginator

session = Session()

session = get_session()
async with session.client("sdb") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResultTypeDef
        print(item)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDomainsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDomainsRequestListDomainsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestListDomainsPaginateTypeDef](./type_defs.md#listdomainsrequestlistdomainspaginatetypedef) 
## SelectPaginator

Type annotations and code completion for `#!python session.client("sdb").get_paginator("select")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sdb.paginator import SelectPaginator

session = Session()

session = get_session()
async with session.client("sdb") as client:  # (1)
    paginator: SelectPaginator = client.get_paginator("select")  # (2)
    async for item in paginator.paginate(...):
        item: SelectResultTypeDef
        print(item)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. paginator: [SelectPaginator](./paginators.md#selectpaginator)
3. item: [:material-code-braces: SelectResultTypeDef](./type_defs.md#selectresulttypedef) 


### paginate

Type annotations and code completion for `#!python SelectPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SelectExpression: str,
    ConsistentRead: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SelectResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SelectResultTypeDef](./type_defs.md#selectresulttypedef) 


```python title="Usage example with kwargs"
kwargs: SelectRequestSelectPaginateTypeDef = {  # (1)
    "SelectExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SelectRequestSelectPaginateTypeDef](./type_defs.md#selectrequestselectpaginatetypedef) 
