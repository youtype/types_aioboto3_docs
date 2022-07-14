# Paginators

> [Index](../README.md) > [S3Control](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
    type annotations stubs module [types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

## ListAccessPointsForObjectLambdaPaginator

Type annotations and code completion for `#!python session.client("s3control").get_paginator("list_access_points_for_object_lambda")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_s3control.paginator import ListAccessPointsForObjectLambdaPaginator

session = Session()

session = get_session()
async with session.client("s3control") as client:  # (1)
    paginator: ListAccessPointsForObjectLambdaPaginator = client.get_paginator("list_access_points_for_object_lambda")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPointsForObjectLambdaResultTypeDef
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListAccessPointsForObjectLambdaPaginator](./paginators.md#listaccesspointsforobjectlambdapaginator)
3. item: [:material-code-braces: ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessPointsForObjectLambdaPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccessPointsForObjectLambdaResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef](./type_defs.md#listaccesspointsforobjectlambdarequestlistaccesspointsforobjectlambdapaginatetypedef) 
