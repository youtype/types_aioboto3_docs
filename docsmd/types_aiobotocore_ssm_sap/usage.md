# Examples

> [Index](../README.md) > [SsmSap](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#ssmsap)
    type annotations stubs module [types-aiobotocore-ssm-sap](https://pypi.org/project/types-aiobotocore-ssm-sap/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ssm-sap]` package installed.

Write your `SsmSap` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SsmSapClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-sap") as client:  # (1)
    result = await client.delete_resource_permission()  # (2)
```

1. client: [SsmSapClient](./client.md)
2. result: [:material-code-braces: DeleteResourcePermissionOutputTypeDef](./type_defs.md#deleteresourcepermissionoutputtypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-sap") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SsmSapClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[ssm-sap]`
or a standalone `types_aiobotocore_ssm_sap` package, you have to explicitly specify
`client: SsmSapClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SsmSapClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_sap.client import SsmSapClient
from types_aiobotocore_ssm_sap.type_defs import DeleteResourcePermissionOutputTypeDef
from types_aiobotocore_ssm_sap.type_defs import DeleteResourcePermissionInputTypeDef


session = Session()

client: SsmSapClient
async with session.client("ssm-sap") as client:  # (1)
    kwargs: DeleteResourcePermissionInputTypeDef = {...}  # (2)
    result: DeleteResourcePermissionOutputTypeDef = await client.delete_resource_permission(**kwargs)  # (3)
```

1. client: [SsmSapClient](./client.md)
2. kwargs: [:material-code-braces: DeleteResourcePermissionInputTypeDef](./type_defs.md#deleteresourcepermissioninputtypedef)
3. result: [:material-code-braces: DeleteResourcePermissionOutputTypeDef](./type_defs.md#deleteresourcepermissionoutputtypedef)



#### Paginator usage example

```python
# ListApplicationsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_sap.client import SsmSapClient
from types_aiobotocore_ssm_sap.paginator import ListApplicationsPaginator
from types_aiobotocore_ssm_sap.type_defs import ListApplicationsOutputTypeDef


session = Session()

client: SsmSapClient
async with session.client("ssm-sap") as client:  # (1)
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationsOutputTypeDef
        print(item)  # (3)
```

1. client: [SsmSapClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsOutputTypeDef](./type_defs.md#listapplicationsoutputtypedef)




