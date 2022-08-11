# Route53RecoveryClusterClient

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Route53RecoveryClusterClient

!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

## Route53RecoveryClusterClient

Type annotations and code completion for `#!python session.client("route53-recovery-cluster")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient

session = Session()
async with session.client("route53-recovery-cluster") as client:
    client: Route53RecoveryClusterClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("route53-recovery-cluster").exceptions` structure.

```python title="Usage example"
async with session.client("route53-recovery-cluster") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.EndpointTemporarilyUnavailableException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_route53_recovery_cluster.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_routing\_control\_state

Get the state for a routing control.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").get_routing_control_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.get_routing_control_state)

```python title="Method definition"
await def get_routing_control_state(
    self,
    *,
    RoutingControlArn: str,
) -> GetRoutingControlStateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetRoutingControlStateRequestRequestTypeDef = {  # (1)
    "RoutingControlArn": ...,
}

parent.get_routing_control_state(**kwargs)
```

1. See [:material-code-braces: GetRoutingControlStateRequestRequestTypeDef](./type_defs.md#getroutingcontrolstaterequestrequesttypedef) 

### update\_routing\_control\_state

Set the state of the routing control to reroute traffic.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").update_routing_control_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_state)

```python title="Method definition"
await def update_routing_control_state(
    self,
    *,
    RoutingControlArn: str,
    RoutingControlState: RoutingControlStateType,  # (1)
    SafetyRulesToOverride: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: RoutingControlStateType](./literals.md#routingcontrolstatetype) 


```python title="Usage example with kwargs"
kwargs: UpdateRoutingControlStateRequestRequestTypeDef = {  # (1)
    "RoutingControlArn": ...,
    "RoutingControlState": ...,
}

parent.update_routing_control_state(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingControlStateRequestRequestTypeDef](./type_defs.md#updateroutingcontrolstaterequestrequesttypedef) 

### update\_routing\_control\_states

Set multiple routing control states.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").update_routing_control_states` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.update_routing_control_states)

```python title="Method definition"
await def update_routing_control_states(
    self,
    *,
    UpdateRoutingControlStateEntries: Sequence[UpdateRoutingControlStateEntryTypeDef],  # (1)
    SafetyRulesToOverride: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: UpdateRoutingControlStateEntryTypeDef](./type_defs.md#updateroutingcontrolstateentrytypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateRoutingControlStatesRequestRequestTypeDef = {  # (1)
    "UpdateRoutingControlStateEntries": ...,
}

parent.update_routing_control_states(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingControlStatesRequestRequestTypeDef](./type_defs.md#updateroutingcontrolstatesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("route53-recovery-cluster").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> Route53RecoveryClusterClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("route53-recovery-cluster").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





