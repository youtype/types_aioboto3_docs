# Examples

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#route53recoverycluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[route53-recovery-cluster]` package installed.

Write your `Route53RecoveryCluster` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# Route53RecoveryClusterClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53-recovery-cluster") as client:  # (1)
    result = await client.get_routing_control_state()  # (2)
```

1. client: [Route53RecoveryClusterClient](./client.md)
2. result: [:material-code-braces: GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef)



#### Paginator usage example

```python
# ListRoutingControlsPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53-recovery-cluster") as client:  # (1)
    paginator = client.get_paginator("list_routing_controls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53RecoveryClusterClient](./client.md)
2. paginator: [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)
3. item: [:material-code-braces: ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef)




### Explicit type annotations

With `types-aioboto3-lite[route53-recovery-cluster]`
or a standalone `types_aiobotocore_route53_recovery_cluster` package, you have to explicitly specify
`client: Route53RecoveryClusterClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# Route53RecoveryClusterClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient
from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateResponseTypeDef
from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateRequestTypeDef


session = Session()

client: Route53RecoveryClusterClient
async with session.client("route53-recovery-cluster") as client:  # (1)
    kwargs: GetRoutingControlStateRequestTypeDef = {...}  # (2)
    result: GetRoutingControlStateResponseTypeDef = await client.get_routing_control_state(**kwargs)  # (3)
```

1. client: [Route53RecoveryClusterClient](./client.md)
2. kwargs: [:material-code-braces: GetRoutingControlStateRequestTypeDef](./type_defs.md#getroutingcontrolstaterequesttypedef)
3. result: [:material-code-braces: GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef)



#### Paginator usage example

```python
# ListRoutingControlsPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient
from types_aiobotocore_route53_recovery_cluster.paginator import ListRoutingControlsPaginator
from types_aiobotocore_route53_recovery_cluster.type_defs import ListRoutingControlsResponseTypeDef


session = Session()

client: Route53RecoveryClusterClient
async with session.client("route53-recovery-cluster") as client:  # (1)
    paginator: ListRoutingControlsPaginator = client.get_paginator("list_routing_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryClusterClient](./client.md)
2. paginator: [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)
3. item: [:material-code-braces: ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef)




