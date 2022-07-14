# Paginators

> [Index](../README.md) > [Shield](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
    type annotations stubs module [types-aiobotocore-shield](https://pypi.org/project/types-aiobotocore-shield/).

## ListAttacksPaginator

Type annotations and code completion for `#!python session.client("shield").get_paginator("list_attacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_shield.paginator import ListAttacksPaginator

session = Session()

session = get_session()
async with session.client("shield") as client:  # (1)
    paginator: ListAttacksPaginator = client.get_paginator("list_attacks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAttacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ShieldClient](./client.md)
2. paginator: [ListAttacksPaginator](./paginators.md#listattackspaginator)
3. item: [:material-code-braces: ListAttacksResponseTypeDef](./type_defs.md#listattacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAttacksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArns: Sequence[str] = ...,
    StartTime: TimeRangeTypeDef = ...,  # (1)
    EndTime: TimeRangeTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListAttacksResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAttacksResponseTypeDef](./type_defs.md#listattacksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttacksRequestListAttacksPaginateTypeDef = {  # (1)
    "ResourceArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttacksRequestListAttacksPaginateTypeDef](./type_defs.md#listattacksrequestlistattackspaginatetypedef) 
## ListProtectionsPaginator

Type annotations and code completion for `#!python session.client("shield").get_paginator("list_protections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_shield.paginator import ListProtectionsPaginator

session = Session()

session = get_session()
async with session.client("shield") as client:  # (1)
    paginator: ListProtectionsPaginator = client.get_paginator("list_protections")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ShieldClient](./client.md)
2. paginator: [ListProtectionsPaginator](./paginators.md#listprotectionspaginator)
3. item: [:material-code-braces: ListProtectionsResponseTypeDef](./type_defs.md#listprotectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProtectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProtectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProtectionsResponseTypeDef](./type_defs.md#listprotectionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProtectionsRequestListProtectionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectionsRequestListProtectionsPaginateTypeDef](./type_defs.md#listprotectionsrequestlistprotectionspaginatetypedef) 
