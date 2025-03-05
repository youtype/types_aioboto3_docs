# Examples

> [Index](../README.md) > [CloudHSMV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#cloudhsmv2)
    type annotations stubs module [types-aiobotocore-cloudhsmv2](https://pypi.org/project/types-aiobotocore-cloudhsmv2/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[cloudhsmv2]` package installed.

Write your `CloudHSMV2` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CloudHSMV2Client usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudhsmv2") as client:  # (1)
    result = await client.copy_backup_to_region()  # (2)
```

1. client: [CloudHSMV2Client](./client.md)
2. result: [:material-code-braces: CopyBackupToRegionResponseTypeDef](./type_defs.md#copybackuptoregionresponsetypedef)



#### Paginator usage example

```python
# DescribeBackupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("cloudhsmv2") as client:  # (1)
    paginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudHSMV2Client](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[cloudhsmv2]`
or a standalone `types_aiobotocore_cloudhsmv2` package, you have to explicitly specify
`client: CloudHSMV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CloudHSMV2Client usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudhsmv2.client import CloudHSMV2Client
from types_aiobotocore_cloudhsmv2.type_defs import CopyBackupToRegionResponseTypeDef
from types_aiobotocore_cloudhsmv2.type_defs import CopyBackupToRegionRequestTypeDef


session = Session()

client: CloudHSMV2Client
async with session.client("cloudhsmv2") as client:  # (1)
    kwargs: CopyBackupToRegionRequestTypeDef = {...}  # (2)
    result: CopyBackupToRegionResponseTypeDef = await client.copy_backup_to_region(**kwargs)  # (3)
```

1. client: [CloudHSMV2Client](./client.md)
2. kwargs: [:material-code-braces: CopyBackupToRegionRequestTypeDef](./type_defs.md#copybackuptoregionrequesttypedef)
3. result: [:material-code-braces: CopyBackupToRegionResponseTypeDef](./type_defs.md#copybackuptoregionresponsetypedef)



#### Paginator usage example

```python
# DescribeBackupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_cloudhsmv2.client import CloudHSMV2Client
from types_aiobotocore_cloudhsmv2.paginator import DescribeBackupsPaginator
from types_aiobotocore_cloudhsmv2.type_defs import DescribeBackupsResponseTypeDef


session = Session()

client: CloudHSMV2Client
async with session.client("cloudhsmv2") as client:  # (1)
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudHSMV2Client](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)




