# Examples

> [Index](../README.md) > [BackupSearch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BackupSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch.html#backupsearch)
    type annotations stubs module [types-aiobotocore-backupsearch](https://pypi.org/project/types-aiobotocore-backupsearch/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[backupsearch]` package installed.

Write your `BackupSearch` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BackupSearchClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("backupsearch") as client:  # (1)
    result = await client.get_search_job()  # (2)
```

1. client: [BackupSearchClient](./client.md)
2. result: [:material-code-braces: GetSearchJobOutputTypeDef](./type_defs.md#getsearchjoboutputtypedef)



#### Paginator usage example

```python
# ListSearchJobBackupsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("backupsearch") as client:  # (1)
    paginator = client.get_paginator("list_search_job_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchJobBackupsPaginator](./paginators.md#listsearchjobbackupspaginator)
3. item: [:material-code-braces: ListSearchJobBackupsOutputTypeDef](./type_defs.md#listsearchjobbackupsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[backupsearch]`
or a standalone `types_aiobotocore_backupsearch` package, you have to explicitly specify
`client: BackupSearchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BackupSearchClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_backupsearch.client import BackupSearchClient
from types_aiobotocore_backupsearch.type_defs import GetSearchJobOutputTypeDef
from types_aiobotocore_backupsearch.type_defs import GetSearchJobInputTypeDef


session = Session()

client: BackupSearchClient
async with session.client("backupsearch") as client:  # (1)
    kwargs: GetSearchJobInputTypeDef = {...}  # (2)
    result: GetSearchJobOutputTypeDef = await client.get_search_job(**kwargs)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. kwargs: [:material-code-braces: GetSearchJobInputTypeDef](./type_defs.md#getsearchjobinputtypedef)
3. result: [:material-code-braces: GetSearchJobOutputTypeDef](./type_defs.md#getsearchjoboutputtypedef)



#### Paginator usage example

```python
# ListSearchJobBackupsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_backupsearch.client import BackupSearchClient
from types_aiobotocore_backupsearch.paginator import ListSearchJobBackupsPaginator
from types_aiobotocore_backupsearch.type_defs import ListSearchJobBackupsOutputTypeDef


session = Session()

client: BackupSearchClient
async with session.client("backupsearch") as client:  # (1)
    paginator: ListSearchJobBackupsPaginator = client.get_paginator("list_search_job_backups")  # (2)
    async for item in paginator.paginate(...):
        item: ListSearchJobBackupsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchJobBackupsPaginator](./paginators.md#listsearchjobbackupspaginator)
3. item: [:material-code-braces: ListSearchJobBackupsOutputTypeDef](./type_defs.md#listsearchjobbackupsoutputtypedef)




