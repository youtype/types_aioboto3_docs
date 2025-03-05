# Examples

> [Index](../README.md) > [SWF](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#swf)
    type annotations stubs module [types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[swf]` package installed.

Write your `SWF` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SWFClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("swf") as client:  # (1)
    result = await client.count_closed_workflow_executions()  # (2)
```

1. client: [SWFClient](./client.md)
2. result: [:material-code-braces: WorkflowExecutionCountTypeDef](./type_defs.md#workflowexecutioncounttypedef)



#### Paginator usage example

```python
# GetWorkflowExecutionHistoryPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("swf") as client:  # (1)
    paginator = client.get_paginator("get_workflow_execution_history")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [GetWorkflowExecutionHistoryPaginator](./paginators.md#getworkflowexecutionhistorypaginator)
3. item: [:material-code-braces: HistoryTypeDef](./type_defs.md#historytypedef)




### Explicit type annotations

With `types-aioboto3-lite[swf]`
or a standalone `types_aiobotocore_swf` package, you have to explicitly specify
`client: SWFClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SWFClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_swf.client import SWFClient
from types_aiobotocore_swf.type_defs import WorkflowExecutionCountTypeDef
from types_aiobotocore_swf.type_defs import CountClosedWorkflowExecutionsInputTypeDef


session = Session()

client: SWFClient
async with session.client("swf") as client:  # (1)
    kwargs: CountClosedWorkflowExecutionsInputTypeDef = {...}  # (2)
    result: WorkflowExecutionCountTypeDef = await client.count_closed_workflow_executions(**kwargs)  # (3)
```

1. client: [SWFClient](./client.md)
2. kwargs: [:material-code-braces: CountClosedWorkflowExecutionsInputTypeDef](./type_defs.md#countclosedworkflowexecutionsinputtypedef)
3. result: [:material-code-braces: WorkflowExecutionCountTypeDef](./type_defs.md#workflowexecutioncounttypedef)



#### Paginator usage example

```python
# GetWorkflowExecutionHistoryPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_swf.client import SWFClient
from types_aiobotocore_swf.paginator import GetWorkflowExecutionHistoryPaginator
from types_aiobotocore_swf.type_defs import HistoryTypeDef


session = Session()

client: SWFClient
async with session.client("swf") as client:  # (1)
    paginator: GetWorkflowExecutionHistoryPaginator = client.get_paginator("get_workflow_execution_history")  # (2)
    async for item in paginator.paginate(...):
        item: HistoryTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [GetWorkflowExecutionHistoryPaginator](./paginators.md#getworkflowexecutionhistorypaginator)
3. item: [:material-code-braces: HistoryTypeDef](./type_defs.md#historytypedef)




