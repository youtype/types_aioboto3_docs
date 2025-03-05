# Examples

> [Index](../README.md) > [DocDBElastic](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[docdb-elastic]` package installed.

Write your `DocDBElastic` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DocDBElasticClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("docdb-elastic") as client:  # (1)
    result = await client.apply_pending_maintenance_action()  # (2)
```

1. client: [DocDBElasticClient](./client.md)
2. result: [:material-code-braces: ApplyPendingMaintenanceActionOutputTypeDef](./type_defs.md#applypendingmaintenanceactionoutputtypedef)



#### Paginator usage example

```python
# ListClusterSnapshotsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("docdb-elastic") as client:  # (1)
    paginator = client.get_paginator("list_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. paginator: [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
3. item: [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef)




### Explicit type annotations

With `types-aioboto3-lite[docdb-elastic]`
or a standalone `types_aiobotocore_docdb_elastic` package, you have to explicitly specify
`client: DocDBElasticClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DocDBElasticClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_docdb_elastic.client import DocDBElasticClient
from types_aiobotocore_docdb_elastic.type_defs import ApplyPendingMaintenanceActionOutputTypeDef
from types_aiobotocore_docdb_elastic.type_defs import ApplyPendingMaintenanceActionInputTypeDef


session = Session()

client: DocDBElasticClient
async with session.client("docdb-elastic") as client:  # (1)
    kwargs: ApplyPendingMaintenanceActionInputTypeDef = {...}  # (2)
    result: ApplyPendingMaintenanceActionOutputTypeDef = await client.apply_pending_maintenance_action(**kwargs)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. kwargs: [:material-code-braces: ApplyPendingMaintenanceActionInputTypeDef](./type_defs.md#applypendingmaintenanceactioninputtypedef)
3. result: [:material-code-braces: ApplyPendingMaintenanceActionOutputTypeDef](./type_defs.md#applypendingmaintenanceactionoutputtypedef)



#### Paginator usage example

```python
# ListClusterSnapshotsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_docdb_elastic.client import DocDBElasticClient
from types_aiobotocore_docdb_elastic.paginator import ListClusterSnapshotsPaginator
from types_aiobotocore_docdb_elastic.type_defs import ListClusterSnapshotsOutputTypeDef


session = Session()

client: DocDBElasticClient
async with session.client("docdb-elastic") as client:  # (1)
    paginator: ListClusterSnapshotsPaginator = client.get_paginator("list_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: ListClusterSnapshotsOutputTypeDef
        print(item)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. paginator: [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
3. item: [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef)




