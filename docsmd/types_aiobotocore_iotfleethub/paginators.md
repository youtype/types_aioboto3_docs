# Paginators

> [Index](../README.md) > [IoTFleetHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTFleetHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
    type annotations stubs module [types-aiobotocore-iotfleethub](https://pypi.org/project/types-aiobotocore-iotfleethub/).

## ListApplicationsPaginator

Type annotations and code completion for `#!python session.client("iotfleethub").get_paginator("list_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Paginator.ListApplications)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_iotfleethub.paginator import ListApplicationsPaginator

session = Session()

session = get_session()
async with session.client("iotfleethub") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetHubClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationsRequestListApplicationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef) 
