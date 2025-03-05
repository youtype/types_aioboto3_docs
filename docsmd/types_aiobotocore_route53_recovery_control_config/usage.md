# Examples

> [Index](../README.md) > [Route53RecoveryControlConfig](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53RecoveryControlConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#route53recoverycontrolconfig)
    type annotations stubs module [types-aiobotocore-route53-recovery-control-config](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[route53-recovery-control-config]` package installed.

Write your `Route53RecoveryControlConfig` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# Route53RecoveryControlConfigClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53-recovery-control-config") as client:  # (1)
    result = await client.create_cluster()  # (2)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)



#### Paginator usage example

```python
# ListAssociatedRoute53HealthChecksPaginator usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53-recovery-control-config") as client:  # (1)
    paginator = client.get_paginator("list_associated_route53_health_checks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListAssociatedRoute53HealthChecksPaginator](./paginators.md#listassociatedroute53healthcheckspaginator)
3. item: [:material-code-braces: ListAssociatedRoute53HealthChecksResponseTypeDef](./type_defs.md#listassociatedroute53healthchecksresponsetypedef)



#### Waiter usage example

```python
# ClusterCreatedWaiter usage example

from aioboto3.session import Session


session = Session()

async with session.client("route53-recovery-control-config") as client:  # (1)
    waiter = client.get_waiter("cluster_created")  # (2)
    await waiter.wait(...)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. waiter: [ClusterCreatedWaiter](./waiters.md#clustercreatedwaiter)


### Explicit type annotations

With `types-aioboto3-lite[route53-recovery-control-config]`
or a standalone `types_aiobotocore_route53_recovery_control_config` package, you have to explicitly specify
`client: Route53RecoveryControlConfigClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# Route53RecoveryControlConfigClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53_recovery_control_config.client import Route53RecoveryControlConfigClient
from types_aiobotocore_route53_recovery_control_config.type_defs import CreateClusterResponseTypeDef
from types_aiobotocore_route53_recovery_control_config.type_defs import CreateClusterRequestTypeDef


session = Session()

client: Route53RecoveryControlConfigClient
async with session.client("route53-recovery-control-config") as client:  # (1)
    kwargs: CreateClusterRequestTypeDef = {...}  # (2)
    result: CreateClusterResponseTypeDef = await client.create_cluster(**kwargs)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. kwargs: [:material-code-braces: CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef)
3. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)



#### Paginator usage example

```python
# ListAssociatedRoute53HealthChecksPaginator usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53_recovery_control_config.client import Route53RecoveryControlConfigClient
from types_aiobotocore_route53_recovery_control_config.paginator import ListAssociatedRoute53HealthChecksPaginator
from types_aiobotocore_route53_recovery_control_config.type_defs import ListAssociatedRoute53HealthChecksResponseTypeDef


session = Session()

client: Route53RecoveryControlConfigClient
async with session.client("route53-recovery-control-config") as client:  # (1)
    paginator: ListAssociatedRoute53HealthChecksPaginator = client.get_paginator("list_associated_route53_health_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedRoute53HealthChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListAssociatedRoute53HealthChecksPaginator](./paginators.md#listassociatedroute53healthcheckspaginator)
3. item: [:material-code-braces: ListAssociatedRoute53HealthChecksResponseTypeDef](./type_defs.md#listassociatedroute53healthchecksresponsetypedef)



#### Waiter usage example

```python
# ClusterCreatedWaiter usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_route53_recovery_control_config.client import Route53RecoveryControlConfigClient
from types_aiobotocore_route53_recovery_control_config.waiter import ClusterCreatedWaiter


session = Session()

async with session.client("route53-recovery-control-config") as client:  # (1)
    waiter = client.get_waiter("cluster_created")  # (2)
    await waiter.wait(...)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. waiter: [ClusterCreatedWaiter](./waiters.md#clustercreatedwaiter)


