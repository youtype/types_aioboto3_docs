# Examples

> [Index](../README.md) > [NetworkFlowMonitor](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NetworkFlowMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#networkflowmonitor)
    type annotations stubs module [types-aiobotocore-networkflowmonitor](https://pypi.org/project/types-aiobotocore-networkflowmonitor/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[networkflowmonitor]` package installed.

Write your `NetworkFlowMonitor` code as usual,
type checking and code completion should work out of the box.



```python
# NetworkFlowMonitorClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("networkflowmonitor") as client:  # (1)
    result = await client.create_monitor()  # (2)
```

1. client: [NetworkFlowMonitorClient](./client.md)
2. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 



```python
# GetQueryResultsMonitorTopContributorsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("networkflowmonitor") as client:  # (1)
    paginator = client.get_paginator("get_query_results_monitor_top_contributors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NetworkFlowMonitorClient](./client.md)
2. paginator: [GetQueryResultsMonitorTopContributorsPaginator](./paginators.md#getqueryresultsmonitortopcontributorspaginator)
3. item: [:material-code-braces: GetQueryResultsMonitorTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsoutputtypedef) 




### Explicit type annotations

With `types-aioboto3-lite[networkflowmonitor]`
or a standalone `types_aiobotocore_networkflowmonitor` package, you have to explicitly specify
`client: NetworkFlowMonitorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NetworkFlowMonitorClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_networkflowmonitor.client import NetworkFlowMonitorClient
from types_aiobotocore_networkflowmonitor.type_defs import CreateMonitorOutputTypeDef
from types_aiobotocore_networkflowmonitor.type_defs import CreateMonitorInputRequestTypeDef


session = Session()

client: NetworkFlowMonitorClient
async with session.client("networkflowmonitor") as client:  # (1)
    kwargs: CreateMonitorInputRequestTypeDef = {...}  # (2)
    result: CreateMonitorOutputTypeDef = await client.create_monitor(**kwargs)  # (3)
```

1. client: [NetworkFlowMonitorClient](./client.md)
2. kwargs: [:material-code-braces: CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef) 
3. result: [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 



```python
# GetQueryResultsMonitorTopContributorsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_networkflowmonitor.client import NetworkFlowMonitorClient
from types_aiobotocore_networkflowmonitor.paginator import GetQueryResultsMonitorTopContributorsPaginator
from types_aiobotocore_networkflowmonitor.type_defs import GetQueryResultsMonitorTopContributorsOutputTypeDef


session = Session()

client: NetworkFlowMonitorClient
async with session.client("networkflowmonitor") as client:  # (1)
    paginator: GetQueryResultsMonitorTopContributorsPaginator = client.get_paginator("get_query_results_monitor_top_contributors")  # (2)
    async for item in paginator.paginate(...):
        item: GetQueryResultsMonitorTopContributorsOutputTypeDef
        print(item)  # (3)
```

1. client: [NetworkFlowMonitorClient](./client.md)
2. paginator: [GetQueryResultsMonitorTopContributorsPaginator](./paginators.md#getqueryresultsmonitortopcontributorspaginator)
3. item: [:material-code-braces: GetQueryResultsMonitorTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsoutputtypedef) 



