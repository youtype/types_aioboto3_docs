# Examples

> [Index](../README.md) > [TimestreamQuery](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#timestreamquery)
    type annotations stubs module [types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[timestream-query]` package installed.

Write your `TimestreamQuery` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# TimestreamQueryClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("timestream-query") as client:  # (1)
    result = await client.cancel_query()  # (2)
```

1. client: [TimestreamQueryClient](./client.md)
2. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef)



#### Paginator usage example

```python
# ListScheduledQueriesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("timestream-query") as client:  # (1)
    paginator = client.get_paginator("list_scheduled_queries")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TimestreamQueryClient](./client.md)
2. paginator: [ListScheduledQueriesPaginator](./paginators.md#listscheduledqueriespaginator)
3. item: [:material-code-braces: ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[timestream-query]`
or a standalone `types_aiobotocore_timestream_query` package, you have to explicitly specify
`client: TimestreamQueryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# TimestreamQueryClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_timestream_query.client import TimestreamQueryClient
from types_aiobotocore_timestream_query.type_defs import CancelQueryResponseTypeDef
from types_aiobotocore_timestream_query.type_defs import CancelQueryRequestTypeDef


session = Session()

client: TimestreamQueryClient
async with session.client("timestream-query") as client:  # (1)
    kwargs: CancelQueryRequestTypeDef = {...}  # (2)
    result: CancelQueryResponseTypeDef = await client.cancel_query(**kwargs)  # (3)
```

1. client: [TimestreamQueryClient](./client.md)
2. kwargs: [:material-code-braces: CancelQueryRequestTypeDef](./type_defs.md#cancelqueryrequesttypedef)
3. result: [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef)



#### Paginator usage example

```python
# ListScheduledQueriesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_timestream_query.client import TimestreamQueryClient
from types_aiobotocore_timestream_query.paginator import ListScheduledQueriesPaginator
from types_aiobotocore_timestream_query.type_defs import ListScheduledQueriesResponseTypeDef


session = Session()

client: TimestreamQueryClient
async with session.client("timestream-query") as client:  # (1)
    paginator: ListScheduledQueriesPaginator = client.get_paginator("list_scheduled_queries")  # (2)
    async for item in paginator.paginate(...):
        item: ListScheduledQueriesResponseTypeDef
        print(item)  # (3)
```

1. client: [TimestreamQueryClient](./client.md)
2. paginator: [ListScheduledQueriesPaginator](./paginators.md#listscheduledqueriespaginator)
3. item: [:material-code-braces: ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef)




