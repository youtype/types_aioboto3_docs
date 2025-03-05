# Examples

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#applicationdiscoveryservice)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[discovery]` package installed.

Write your `ApplicationDiscoveryService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ApplicationDiscoveryServiceClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("discovery") as client:  # (1)
    result = await client.batch_delete_agents()  # (2)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. result: [:material-code-braces: BatchDeleteAgentsResponseTypeDef](./type_defs.md#batchdeleteagentsresponsetypedef)



#### Paginator usage example

```python
# DescribeAgentsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("discovery") as client:  # (1)
    paginator = client.get_paginator("describe_agents")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
3. item: [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[discovery]`
or a standalone `types_aiobotocore_discovery` package, you have to explicitly specify
`client: ApplicationDiscoveryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ApplicationDiscoveryServiceClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient
from types_aiobotocore_discovery.type_defs import BatchDeleteAgentsResponseTypeDef
from types_aiobotocore_discovery.type_defs import BatchDeleteAgentsRequestTypeDef


session = Session()

client: ApplicationDiscoveryServiceClient
async with session.client("discovery") as client:  # (1)
    kwargs: BatchDeleteAgentsRequestTypeDef = {...}  # (2)
    result: BatchDeleteAgentsResponseTypeDef = await client.batch_delete_agents(**kwargs)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. kwargs: [:material-code-braces: BatchDeleteAgentsRequestTypeDef](./type_defs.md#batchdeleteagentsrequesttypedef)
3. result: [:material-code-braces: BatchDeleteAgentsResponseTypeDef](./type_defs.md#batchdeleteagentsresponsetypedef)



#### Paginator usage example

```python
# DescribeAgentsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient
from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator
from types_aiobotocore_discovery.type_defs import DescribeAgentsResponseTypeDef


session = Session()

client: ApplicationDiscoveryServiceClient
async with session.client("discovery") as client:  # (1)
    paginator: DescribeAgentsPaginator = client.get_paginator("describe_agents")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApplicationDiscoveryServiceClient](./client.md)
2. paginator: [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
3. item: [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef)




