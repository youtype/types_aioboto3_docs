# Examples

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[route53-recovery-cluster]` package installed.

Write your `Route53RecoveryCluster` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("route53-recovery-cluster") as client:  # (1)
        result = await client.get_routing_control_state()  # (2)
    ```

    1. client: [Route53RecoveryClusterClient](./client.md)
    2. result: [:material-code-braces: GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[route53-recovery-cluster]`
or a standalone `types_aiobotocore_route53_recovery_cluster` package, you have to explicitly specify
`client: Route53RecoveryClusterClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient
    from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateResponseTypeDef
    from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateRequestRequestTypeDef


    session = Session()

    client: Route53RecoveryClusterClient
    async with session.client("route53-recovery-cluster") as client:  # (1)
        kwargs: GetRoutingControlStateRequestRequestTypeDef = {...}  # (2)
        result: GetRoutingControlStateResponseTypeDef = await client.get_routing_control_state(**kwargs)  # (3)
    ```

    1. client: [Route53RecoveryClusterClient](./client.md)
    2. kwargs: [:material-code-braces: GetRoutingControlStateRequestRequestTypeDef](./type_defs.md#getroutingcontrolstaterequestrequesttypedef) 
    3. result: [:material-code-braces: GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef) 






