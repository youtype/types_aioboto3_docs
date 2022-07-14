# Examples

> [Index](../README.md) > [ElasticLoadBalancing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
    type annotations stubs module [types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[elb]` package installed.

Write your `ElasticLoadBalancing` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elb") as client:  # (1)
        result = await client.apply_security_groups_to_load_balancer()  # (2)
    ```

    1. client: [ElasticLoadBalancingClient](./client.md)
    2. result: [:material-code-braces: ApplySecurityGroupsToLoadBalancerOutputTypeDef](./type_defs.md#applysecuritygroupstoloadbalanceroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elb") as client:  # (1)
        paginator = client.get_paginator("describe_account_limits")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ElasticLoadBalancingClient](./client.md)
    2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
    3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("elb") as client:  # (1)
        waiter = client.get_waiter("any_instance_in_service")  # (2)
        await waiter.wait()
    ```

    1. client: [ElasticLoadBalancingClient](./client.md)
    2. waiter: [AnyInstanceInServiceWaiter](./waiters.md#anyinstanceinservicewaiter)


### Explicit type annotations

With `types-aioboto3-lite[elb]`
or a standalone `types_aiobotocore_elb` package, you have to explicitly specify
`client: ElasticLoadBalancingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elb.client import ElasticLoadBalancingClient
    from types_aiobotocore_elb.type_defs import ApplySecurityGroupsToLoadBalancerOutputTypeDef
    from types_aiobotocore_elb.type_defs import ApplySecurityGroupsToLoadBalancerInputRequestTypeDef


    session = Session()

    client: ElasticLoadBalancingClient
    async with session.client("elb") as client:  # (1)
        kwargs: ApplySecurityGroupsToLoadBalancerInputRequestTypeDef = {...}  # (2)
        result: ApplySecurityGroupsToLoadBalancerOutputTypeDef = await client.apply_security_groups_to_load_balancer(**kwargs)  # (3)
    ```

    1. client: [ElasticLoadBalancingClient](./client.md)
    2. kwargs: [:material-code-braces: ApplySecurityGroupsToLoadBalancerInputRequestTypeDef](./type_defs.md#applysecuritygroupstoloadbalancerinputrequesttypedef) 
    3. result: [:material-code-braces: ApplySecurityGroupsToLoadBalancerOutputTypeDef](./type_defs.md#applysecuritygroupstoloadbalanceroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elb.client import ElasticLoadBalancingClient
    from types_aiobotocore_elb.paginator import DescribeAccountLimitsPaginator
    from types_aiobotocore_elb.type_defs import DescribeAccountLimitsOutputTypeDef


    session = Session()

    client: ElasticLoadBalancingClient
    async with session.client("elb") as client:  # (1)
        paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")  # (2)
        async for item in paginator.paginate(...):
            item: DescribeAccountLimitsOutputTypeDef
            print(item)  # (3)
    ```

    1. client: [ElasticLoadBalancingClient](./client.md)
    2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
    3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aioboto3.session import Session

    from types_aiobotocore_elb.client import ElasticLoadBalancingClient
    from types_aiobotocore_elb.waiter import AnyInstanceInServiceWaiter


    session = Session()

    async with session.client("elb") as client:  # (1)
        waiter = client.get_waiter("any_instance_in_service")  # (2)
        await waiter.wait()
    ```

    1. client: [ElasticLoadBalancingClient](./client.md)
    2. waiter: [AnyInstanceInServiceWaiter](./waiters.md#anyinstanceinservicewaiter)


