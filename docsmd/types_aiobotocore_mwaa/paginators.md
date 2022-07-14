# Paginators

> [Index](../README.md) > [MWAA](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
    type annotations stubs module [types-aiobotocore-mwaa](https://pypi.org/project/types-aiobotocore-mwaa/).

## ListEnvironmentsPaginator

Type annotations and code completion for `#!python session.client("mwaa").get_paginator("list_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_mwaa.paginator import ListEnvironmentsPaginator

session = Session()

session = get_session()
async with session.client("mwaa") as client:  # (1)
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsOutputTypeDef
        print(item)  # (3)
```

1. client: [MWAAClient](./client.md)
2. paginator: [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
3. item: [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEnvironmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListEnvironmentsInputListEnvironmentsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsInputListEnvironmentsPaginateTypeDef](./type_defs.md#listenvironmentsinputlistenvironmentspaginatetypedef) 
