# Route53RecoveryClusterClient

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Route53RecoveryClusterClient

!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#route53recoverycluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

## Route53RecoveryClusterClient

Type annotations and code completion for `#!python session.client("route53-recovery-cluster")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# Route53RecoveryClusterClient usage example

from aioboto3.session import Session
from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient

session = Session()
async with session.client("route53-recovery-cluster") as client:
    client: Route53RecoveryClusterClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("route53-recovery-cluster").exceptions` structure.

```python
# Route53RecoveryClusterClient.exceptions usage example

async with session.client("route53-recovery-cluster") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.EndpointTemporarilyUnavailableException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceLimitExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# Route53RecoveryClusterClient.exceptions type checking example

from types_aiobotocore_route53_recovery_cluster.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("route53-recovery-cluster").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("route53-recovery-cluster").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# generate_presigned_url method definition

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# get_routing_control_state method definition

await def get_routing_control_state(
    self,
    *,
    RoutingControlArn: str,
) -> GetRoutingControlStateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef) 


```python
# get_routing_control_state method usage example with argument unpacking

kwargs: GetRoutingControlStateRequestRequestTypeDef = {  # (1)
    "RoutingControlArn": ...,
}

parent.get_routing_control_state(**kwargs)
```

1. See [:material-code-braces: GetRoutingControlStateRequestRequestTypeDef](./type_defs.md#getroutingcontrolstaterequestrequesttypedef) 

### list\_routing\_controls

List routing control names and Amazon Resource Names (ARNs), as well as the
routing control state for each routing control, along with the control panel
name and control panel ARN for the routing controls.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").list_routing_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# list_routing_controls method definition

await def list_routing_controls(
    self,
    *,
    ControlPanelArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRoutingControlsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef) 


```python
# list_routing_controls method usage example with argument unpacking

kwargs: ListRoutingControlsRequestRequestTypeDef = {  # (1)
    "ControlPanelArn": ...,
}

parent.list_routing_controls(**kwargs)
```

1. See [:material-code-braces: ListRoutingControlsRequestRequestTypeDef](./type_defs.md#listroutingcontrolsrequestrequesttypedef) 

### update\_routing\_control\_state

Set the state of the routing control to reroute traffic.

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").update_routing_control_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# update_routing_control_state method definition

await def update_routing_control_state(
    self,
    *,
    RoutingControlArn: str,
    RoutingControlState: RoutingControlStateType,  # (1)
    SafetyRulesToOverride: Sequence[str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: RoutingControlStateType](./literals.md#routingcontrolstatetype) 


```python
# update_routing_control_state method usage example with argument unpacking

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# update_routing_control_states method definition

await def update_routing_control_states(
    self,
    *,
    UpdateRoutingControlStateEntries: Sequence[UpdateRoutingControlStateEntryTypeDef],  # (1)
    SafetyRulesToOverride: Sequence[str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: UpdateRoutingControlStateEntryTypeDef](./type_defs.md#updateroutingcontrolstateentrytypedef) 


```python
# update_routing_control_states method usage example with argument unpacking

kwargs: UpdateRoutingControlStatesRequestRequestTypeDef = {  # (1)
    "UpdateRoutingControlStateEntries": ...,
}

parent.update_routing_control_states(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingControlStatesRequestRequestTypeDef](./type_defs.md#updateroutingcontrolstatesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("route53-recovery-cluster").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("route53-recovery-cluster").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("route53-recovery-cluster").get_paginator` method with overloads.

- `client.get_paginator("list_routing_controls")` -> [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)


