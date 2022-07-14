# Paginators

> [Index](../README.md) > [Translate](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

## ListTerminologiesPaginator

Type annotations and code completion for `#!python session.client("translate").get_paginator("list_terminologies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_translate.paginator import ListTerminologiesPaginator

session = Session()

session = get_session()
async with session.client("translate") as client:  # (1)
    paginator: ListTerminologiesPaginator = client.get_paginator("list_terminologies")  # (2)
    async for item in paginator.paginate(...):
        item: ListTerminologiesResponseTypeDef
        print(item)  # (3)
```

1. client: [TranslateClient](./client.md)
2. paginator: [ListTerminologiesPaginator](./paginators.md#listterminologiespaginator)
3. item: [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTerminologiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTerminologiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTerminologiesRequestListTerminologiesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTerminologiesRequestListTerminologiesPaginateTypeDef](./type_defs.md#listterminologiesrequestlistterminologiespaginatetypedef) 
