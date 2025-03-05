# Paginators

> [Index](../README.md) > [FreeTier](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).

## GetFreeTierUsagePaginator

Type annotations and code completion for `#!python session.client("freetier").get_paginator("get_free_tier_usage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier/paginator/GetFreeTierUsage.html#FreeTier.Paginator.GetFreeTierUsage)

```python
# GetFreeTierUsagePaginator usage example

from aioboto3.session import Session

from types_aiobotocore_freetier.paginator import GetFreeTierUsagePaginator

session = Session()

session = get_session()
async with session.client("freetier") as client:  # (1)
    paginator: GetFreeTierUsagePaginator = client.get_paginator("get_free_tier_usage")  # (2)
    async for item in paginator.paginate(...):
        item: GetFreeTierUsageResponseTypeDef
        print(item)  # (3)
```

1. client: [FreeTierClient](./client.md)
2. paginator: [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)
3. item: `AioPageIterator[GetFreeTierUsageResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetFreeTierUsagePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: ExpressionPaginatorTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetFreeTierUsageResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetFreeTierUsageResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetFreeTierUsageRequestPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFreeTierUsageRequestPaginateTypeDef](./type_defs.md#getfreetierusagerequestpaginatetypedef)
