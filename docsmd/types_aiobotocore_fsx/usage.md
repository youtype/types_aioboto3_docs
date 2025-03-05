# Examples

> [Index](../README.md) > [FSx](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx)
    type annotations stubs module [types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[fsx]` package installed.

Write your `FSx` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# FSxClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("fsx") as client:  # (1)
    result = await client.associate_file_system_aliases()  # (2)
```

1. client: [FSxClient](./client.md)
2. result: [:material-code-braces: AssociateFileSystemAliasesResponseTypeDef](./type_defs.md#associatefilesystemaliasesresponsetypedef)



#### Paginator usage example

```python
# DescribeBackupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("fsx") as client:  # (1)
    paginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[fsx]`
or a standalone `types_aiobotocore_fsx` package, you have to explicitly specify
`client: FSxClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# FSxClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_fsx.client import FSxClient
from types_aiobotocore_fsx.type_defs import AssociateFileSystemAliasesResponseTypeDef
from types_aiobotocore_fsx.type_defs import AssociateFileSystemAliasesRequestTypeDef


session = Session()

client: FSxClient
async with session.client("fsx") as client:  # (1)
    kwargs: AssociateFileSystemAliasesRequestTypeDef = {...}  # (2)
    result: AssociateFileSystemAliasesResponseTypeDef = await client.associate_file_system_aliases(**kwargs)  # (3)
```

1. client: [FSxClient](./client.md)
2. kwargs: [:material-code-braces: AssociateFileSystemAliasesRequestTypeDef](./type_defs.md#associatefilesystemaliasesrequesttypedef)
3. result: [:material-code-braces: AssociateFileSystemAliasesResponseTypeDef](./type_defs.md#associatefilesystemaliasesresponsetypedef)



#### Paginator usage example

```python
# DescribeBackupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_fsx.client import FSxClient
from types_aiobotocore_fsx.paginator import DescribeBackupsPaginator
from types_aiobotocore_fsx.type_defs import DescribeBackupsResponseTypeDef


session = Session()

client: FSxClient
async with session.client("fsx") as client:  # (1)
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)




