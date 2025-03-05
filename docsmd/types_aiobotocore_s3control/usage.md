# Examples

> [Index](../README.md) > [S3Control](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#s3control)
    type annotations stubs module [types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[s3control]` package installed.

Write your `S3Control` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# S3ControlClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3control") as client:  # (1)
    result = await client.associate_access_grants_identity_center()  # (2)
```

1. client: [S3ControlClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListAccessPointsForObjectLambdaPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("s3control") as client:  # (1)
    paginator = client.get_paginator("list_access_points_for_object_lambda")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListAccessPointsForObjectLambdaPaginator](./paginators.md#listaccesspointsforobjectlambdapaginator)
3. item: [:material-code-braces: ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef)




### Explicit type annotations

With `types-aioboto3-lite[s3control]`
or a standalone `types_aiobotocore_s3control` package, you have to explicitly specify
`client: S3ControlClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# S3ControlClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3control.client import S3ControlClient
from types_aiobotocore_s3control.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_s3control.type_defs import AssociateAccessGrantsIdentityCenterRequestTypeDef


session = Session()

client: S3ControlClient
async with session.client("s3control") as client:  # (1)
    kwargs: AssociateAccessGrantsIdentityCenterRequestTypeDef = {...}  # (2)
    result: EmptyResponseMetadataTypeDef = await client.associate_access_grants_identity_center(**kwargs)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. kwargs: [:material-code-braces: AssociateAccessGrantsIdentityCenterRequestTypeDef](./type_defs.md#associateaccessgrantsidentitycenterrequesttypedef)
3. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListAccessPointsForObjectLambdaPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_s3control.client import S3ControlClient
from types_aiobotocore_s3control.paginator import ListAccessPointsForObjectLambdaPaginator
from types_aiobotocore_s3control.type_defs import ListAccessPointsForObjectLambdaResultTypeDef


session = Session()

client: S3ControlClient
async with session.client("s3control") as client:  # (1)
    paginator: ListAccessPointsForObjectLambdaPaginator = client.get_paginator("list_access_points_for_object_lambda")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPointsForObjectLambdaResultTypeDef
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListAccessPointsForObjectLambdaPaginator](./paginators.md#listaccesspointsforobjectlambdapaginator)
3. item: [:material-code-braces: ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef)




