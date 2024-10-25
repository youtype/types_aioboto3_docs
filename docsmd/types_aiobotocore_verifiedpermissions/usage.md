# Examples

> [Index](../README.md) > [VerifiedPermissions](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
    type annotations stubs module [types-aiobotocore-verifiedpermissions](https://pypi.org/project/types-aiobotocore-verifiedpermissions/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[verifiedpermissions]` package installed.

Write your `VerifiedPermissions` code as usual,
type checking and code completion should work out of the box.



```python
# VerifiedPermissionsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("verifiedpermissions") as client:  # (1)
    result = await client.batch_is_authorized()  # (2)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. result: [:material-code-braces: BatchIsAuthorizedOutputTypeDef](./type_defs.md#batchisauthorizedoutputtypedef) 



```python
# ListIdentitySourcesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("verifiedpermissions") as client:  # (1)
    paginator = client.get_paginator("list_identity_sources")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. paginator: [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
3. item: [:material-code-braces: ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[verifiedpermissions]`
or a standalone `types_aiobotocore_verifiedpermissions` package, you have to explicitly specify
`client: VerifiedPermissionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# VerifiedPermissionsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_verifiedpermissions.client import VerifiedPermissionsClient
from types_aiobotocore_verifiedpermissions.type_defs import BatchIsAuthorizedOutputTypeDef
from types_aiobotocore_verifiedpermissions.type_defs import BatchIsAuthorizedInputRequestTypeDef


session = Session()

client: VerifiedPermissionsClient
async with session.client("verifiedpermissions") as client:  # (1)
    kwargs: BatchIsAuthorizedInputRequestTypeDef = {...}  # (2)
    result: BatchIsAuthorizedOutputTypeDef = await client.batch_is_authorized(**kwargs)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. kwargs: [:material-code-braces: BatchIsAuthorizedInputRequestTypeDef](./type_defs.md#batchisauthorizedinputrequesttypedef) 
3. result: [:material-code-braces: BatchIsAuthorizedOutputTypeDef](./type_defs.md#batchisauthorizedoutputtypedef) 



```python
# ListIdentitySourcesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_verifiedpermissions.client import VerifiedPermissionsClient
from types_aiobotocore_verifiedpermissions.paginator import ListIdentitySourcesPaginator
from types_aiobotocore_verifiedpermissions.type_defs import ListIdentitySourcesOutputTypeDef


session = Session()

client: VerifiedPermissionsClient
async with session.client("verifiedpermissions") as client:  # (1)
    paginator: ListIdentitySourcesPaginator = client.get_paginator("list_identity_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentitySourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [VerifiedPermissionsClient](./client.md)
2. paginator: [ListIdentitySourcesPaginator](./paginators.md#listidentitysourcespaginator)
3. item: [:material-code-braces: ListIdentitySourcesOutputTypeDef](./type_defs.md#listidentitysourcesoutputtypedef) 




