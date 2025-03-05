# Examples

> [Index](../README.md) > [SSMIncidents](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#ssmincidents)
    type annotations stubs module [types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[ssm-incidents]` package installed.

Write your `SSMIncidents` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SSMIncidentsClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-incidents") as client:  # (1)
    result = await client.batch_get_incident_findings()  # (2)
```

1. client: [SSMIncidentsClient](./client.md)
2. result: [:material-code-braces: BatchGetIncidentFindingsOutputTypeDef](./type_defs.md#batchgetincidentfindingsoutputtypedef)



#### Paginator usage example

```python
# GetResourcePoliciesPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-incidents") as client:  # (1)
    paginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: [:material-code-braces: GetResourcePoliciesOutputTypeDef](./type_defs.md#getresourcepoliciesoutputtypedef)



#### Waiter usage example

```python
# WaitForReplicationSetActiveWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("ssm-incidents") as client:  # (1)
    waiter = client.get_waiter("wait_for_replication_set_active")  # (2)
    await waiter.wait(...)
```

1. client: [SSMIncidentsClient](./client.md)
2. waiter: [WaitForReplicationSetActiveWaiter](./waiters.md#waitforreplicationsetactivewaiter)


### Explicit type annotations

With `types-aioboto3-lite[ssm-incidents]`
or a standalone `types_aiobotocore_ssm_incidents` package, you have to explicitly specify
`client: SSMIncidentsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SSMIncidentsClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.type_defs import BatchGetIncidentFindingsOutputTypeDef
from types_aiobotocore_ssm_incidents.type_defs import BatchGetIncidentFindingsInputTypeDef


session = Session()

client: SSMIncidentsClient
async with session.client("ssm-incidents") as client:  # (1)
    kwargs: BatchGetIncidentFindingsInputTypeDef = {...}  # (2)
    result: BatchGetIncidentFindingsOutputTypeDef = await client.batch_get_incident_findings(**kwargs)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. kwargs: [:material-code-braces: BatchGetIncidentFindingsInputTypeDef](./type_defs.md#batchgetincidentfindingsinputtypedef)
3. result: [:material-code-braces: BatchGetIncidentFindingsOutputTypeDef](./type_defs.md#batchgetincidentfindingsoutputtypedef)



#### Paginator usage example

```python
# GetResourcePoliciesPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.paginator import GetResourcePoliciesPaginator
from types_aiobotocore_ssm_incidents.type_defs import GetResourcePoliciesOutputTypeDef


session = Session()

client: SSMIncidentsClient
async with session.client("ssm-incidents") as client:  # (1)
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: [:material-code-braces: GetResourcePoliciesOutputTypeDef](./type_defs.md#getresourcepoliciesoutputtypedef)



#### Waiter usage example

```python
# WaitForReplicationSetActiveWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.waiter import WaitForReplicationSetActiveWaiter


session = Session()

async with session.client("ssm-incidents") as client:  # (1)
    waiter = client.get_waiter("wait_for_replication_set_active")  # (2)
    await waiter.wait(...)
```

1. client: [SSMIncidentsClient](./client.md)
2. waiter: [WaitForReplicationSetActiveWaiter](./waiters.md#waitforreplicationsetactivewaiter)


