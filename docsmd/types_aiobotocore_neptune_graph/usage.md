# Examples

> [Index](../README.md) > [NeptuneGraph](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#neptunegraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[neptune-graph]` package installed.

Write your `NeptuneGraph` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# NeptuneGraphClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("neptune-graph") as client:  # (1)
    result = await client.cancel_export_task()  # (2)
```

1. client: [NeptuneGraphClient](./client.md)
2. result: [:material-code-braces: CancelExportTaskOutputTypeDef](./type_defs.md#cancelexporttaskoutputtypedef)



#### Paginator usage example

```python
# ListExportTasksPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("neptune-graph") as client:  # (1)
    paginator = client.get_paginator("list_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListExportTasksPaginator](./paginators.md#listexporttaskspaginator)
3. item: [:material-code-braces: ListExportTasksOutputTypeDef](./type_defs.md#listexporttasksoutputtypedef)



#### Waiter usage example

```python
# ExportTaskCancelledWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("neptune-graph") as client:  # (1)
    waiter = client.get_waiter("export_task_cancelled")  # (2)
    await waiter.wait(...)
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [ExportTaskCancelledWaiter](./waiters.md#exporttaskcancelledwaiter)


### Explicit type annotations

With `types-aioboto3-lite[neptune-graph]`
or a standalone `types_aiobotocore_neptune_graph` package, you have to explicitly specify
`client: NeptuneGraphClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# NeptuneGraphClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient
from types_aiobotocore_neptune_graph.type_defs import CancelExportTaskOutputTypeDef
from types_aiobotocore_neptune_graph.type_defs import CancelExportTaskInputTypeDef


session = Session()

client: NeptuneGraphClient
async with session.client("neptune-graph") as client:  # (1)
    kwargs: CancelExportTaskInputTypeDef = {...}  # (2)
    result: CancelExportTaskOutputTypeDef = await client.cancel_export_task(**kwargs)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. kwargs: [:material-code-braces: CancelExportTaskInputTypeDef](./type_defs.md#cancelexporttaskinputtypedef)
3. result: [:material-code-braces: CancelExportTaskOutputTypeDef](./type_defs.md#cancelexporttaskoutputtypedef)



#### Paginator usage example

```python
# ListExportTasksPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient
from types_aiobotocore_neptune_graph.paginator import ListExportTasksPaginator
from types_aiobotocore_neptune_graph.type_defs import ListExportTasksOutputTypeDef


session = Session()

client: NeptuneGraphClient
async with session.client("neptune-graph") as client:  # (1)
    paginator: ListExportTasksPaginator = client.get_paginator("list_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListExportTasksOutputTypeDef
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListExportTasksPaginator](./paginators.md#listexporttaskspaginator)
3. item: [:material-code-braces: ListExportTasksOutputTypeDef](./type_defs.md#listexporttasksoutputtypedef)



#### Waiter usage example

```python
# ExportTaskCancelledWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient
from types_aiobotocore_neptune_graph.waiter import ExportTaskCancelledWaiter


session = Session()

async with session.client("neptune-graph") as client:  # (1)
    waiter = client.get_waiter("export_task_cancelled")  # (2)
    await waiter.wait(...)
```

1. client: [NeptuneGraphClient](./client.md)
2. waiter: [ExportTaskCancelledWaiter](./waiters.md#exporttaskcancelledwaiter)


