# Examples

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#codeguruprofiler)
    type annotations stubs module [types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[codeguruprofiler]` package installed.

Write your `CodeGuruProfiler` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# CodeGuruProfilerClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("codeguruprofiler") as client:  # (1)
    result = await client.add_notification_channels()  # (2)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. result: [:material-code-braces: AddNotificationChannelsResponseTypeDef](./type_defs.md#addnotificationchannelsresponsetypedef)



#### Paginator usage example

```python
# ListProfileTimesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("codeguruprofiler") as client:  # (1)
    paginator = client.get_paginator("list_profile_times")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. paginator: [ListProfileTimesPaginator](./paginators.md#listprofiletimespaginator)
3. item: [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[codeguruprofiler]`
or a standalone `types_aiobotocore_codeguruprofiler` package, you have to explicitly specify
`client: CodeGuruProfilerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# CodeGuruProfilerClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codeguruprofiler.client import CodeGuruProfilerClient
from types_aiobotocore_codeguruprofiler.type_defs import AddNotificationChannelsResponseTypeDef
from types_aiobotocore_codeguruprofiler.type_defs import AddNotificationChannelsRequestTypeDef


session = Session()

client: CodeGuruProfilerClient
async with session.client("codeguruprofiler") as client:  # (1)
    kwargs: AddNotificationChannelsRequestTypeDef = {...}  # (2)
    result: AddNotificationChannelsResponseTypeDef = await client.add_notification_channels(**kwargs)  # (3)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. kwargs: [:material-code-braces: AddNotificationChannelsRequestTypeDef](./type_defs.md#addnotificationchannelsrequesttypedef)
3. result: [:material-code-braces: AddNotificationChannelsResponseTypeDef](./type_defs.md#addnotificationchannelsresponsetypedef)



#### Paginator usage example

```python
# ListProfileTimesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_codeguruprofiler.client import CodeGuruProfilerClient
from types_aiobotocore_codeguruprofiler.paginator import ListProfileTimesPaginator
from types_aiobotocore_codeguruprofiler.type_defs import ListProfileTimesResponseTypeDef


session = Session()

client: CodeGuruProfilerClient
async with session.client("codeguruprofiler") as client:  # (1)
    paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfileTimesResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeGuruProfilerClient](./client.md)
2. paginator: [ListProfileTimesPaginator](./paginators.md#listprofiletimespaginator)
3. item: [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef)




