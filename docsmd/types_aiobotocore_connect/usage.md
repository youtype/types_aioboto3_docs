# Examples

> [Index](../README.md) > [Connect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[connect]` package installed.

Write your `Connect` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ConnectClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("connect") as client:  # (1)
    result = await client.activate_evaluation_form()  # (2)
```

1. client: [ConnectClient](./client.md)
2. result: [:material-code-braces: ActivateEvaluationFormResponseTypeDef](./type_defs.md#activateevaluationformresponsetypedef)



#### Paginator usage example

```python
# GetMetricDataPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("connect") as client:  # (1)
    paginator = client.get_paginator("get_metric_data")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
3. item: [:material-code-braces: GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[connect]`
or a standalone `types_aiobotocore_connect` package, you have to explicitly specify
`client: ConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ConnectClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connect.client import ConnectClient
from types_aiobotocore_connect.type_defs import ActivateEvaluationFormResponseTypeDef
from types_aiobotocore_connect.type_defs import ActivateEvaluationFormRequestTypeDef


session = Session()

client: ConnectClient
async with session.client("connect") as client:  # (1)
    kwargs: ActivateEvaluationFormRequestTypeDef = {...}  # (2)
    result: ActivateEvaluationFormResponseTypeDef = await client.activate_evaluation_form(**kwargs)  # (3)
```

1. client: [ConnectClient](./client.md)
2. kwargs: [:material-code-braces: ActivateEvaluationFormRequestTypeDef](./type_defs.md#activateevaluationformrequesttypedef)
3. result: [:material-code-braces: ActivateEvaluationFormResponseTypeDef](./type_defs.md#activateevaluationformresponsetypedef)



#### Paginator usage example

```python
# GetMetricDataPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_connect.client import ConnectClient
from types_aiobotocore_connect.paginator import GetMetricDataPaginator
from types_aiobotocore_connect.type_defs import GetMetricDataResponseTypeDef


session = Session()

client: ConnectClient
async with session.client("connect") as client:  # (1)
    paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetMetricDataResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectClient](./client.md)
2. paginator: [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
3. item: [:material-code-braces: GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef)




