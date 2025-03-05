# Paginators

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#elasticloadbalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## DescribeAccountLimitsPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_account_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeAccountLimits.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)

```python
# DescribeAccountLimitsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeAccountLimitsPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: `AioPageIterator[DescribeAccountLimitsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeAccountLimitsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeAccountLimitsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountLimitsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsInputPaginateTypeDef](./type_defs.md#describeaccountlimitsinputpaginatetypedef)
## DescribeListenerCertificatesPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_listener_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeListenerCertificates.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)

```python
# DescribeListenerCertificatesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeListenerCertificatesPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeListenerCertificatesPaginator = client.get_paginator("describe_listener_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeListenerCertificatesOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeListenerCertificatesPaginator](./paginators.md#describelistenercertificatespaginator)
3. item: `AioPageIterator[DescribeListenerCertificatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeListenerCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ListenerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeListenerCertificatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeListenerCertificatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeListenerCertificatesInputPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeListenerCertificatesInputPaginateTypeDef](./type_defs.md#describelistenercertificatesinputpaginatetypedef)
## DescribeListenersPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeListeners.html#ElasticLoadBalancingv2.Paginator.DescribeListeners)

```python
# DescribeListenersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeListenersPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeListenersPaginator = client.get_paginator("describe_listeners")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeListenersOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeListenersPaginator](./paginators.md#describelistenerspaginator)
3. item: `AioPageIterator[DescribeListenersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeListenersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LoadBalancerArn: str = ...,
    ListenerArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeListenersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeListenersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeListenersInputPaginateTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeListenersInputPaginateTypeDef](./type_defs.md#describelistenersinputpaginatetypedef)
## DescribeLoadBalancersPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeLoadBalancers.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers)

```python
# DescribeLoadBalancersPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeLoadBalancersPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLoadBalancersOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)
3. item: `AioPageIterator[DescribeLoadBalancersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLoadBalancersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LoadBalancerArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeLoadBalancersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeLoadBalancersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLoadBalancersInputPaginateTypeDef = {  # (1)
    "LoadBalancerArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancersInputPaginateTypeDef](./type_defs.md#describeloadbalancersinputpaginatetypedef)
## DescribeRulesPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeRules.html#ElasticLoadBalancingv2.Paginator.DescribeRules)

```python
# DescribeRulesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeRulesPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeRulesPaginator = client.get_paginator("describe_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRulesOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeRulesPaginator](./paginators.md#describerulespaginator)
3. item: `AioPageIterator[DescribeRulesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ListenerArn: str = ...,
    RuleArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeRulesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeRulesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRulesInputPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRulesInputPaginateTypeDef](./type_defs.md#describerulesinputpaginatetypedef)
## DescribeSSLPoliciesPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_ssl_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeSSLPolicies.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies)

```python
# DescribeSSLPoliciesPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeSSLPoliciesPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeSSLPoliciesPaginator = client.get_paginator("describe_ssl_policies")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSSLPoliciesOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeSSLPoliciesPaginator](./paginators.md#describesslpoliciespaginator)
3. item: `AioPageIterator[DescribeSSLPoliciesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSSLPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    LoadBalancerType: LoadBalancerTypeEnumType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSSLPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSSLPoliciesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSSLPoliciesInputPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSSLPoliciesInputPaginateTypeDef](./type_defs.md#describesslpoliciesinputpaginatetypedef)
## DescribeTargetGroupsPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_target_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2/paginator/DescribeTargetGroups.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups)

```python
# DescribeTargetGroupsPaginator usage example

from aioboto3.session import Session

from types_aiobotocore_elbv2.paginator import DescribeTargetGroupsPaginator

session = Session()

session = get_session()
async with session.client("elbv2") as client:  # (1)
    paginator: DescribeTargetGroupsPaginator = client.get_paginator("describe_target_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTargetGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [ElasticLoadBalancingv2Client](./client.md)
2. paginator: [DescribeTargetGroupsPaginator](./paginators.md#describetargetgroupspaginator)
3. item: `AioPageIterator[DescribeTargetGroupsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTargetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LoadBalancerArn: str = ...,
    TargetGroupArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeTargetGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeTargetGroupsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTargetGroupsInputPaginateTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTargetGroupsInputPaginateTypeDef](./type_defs.md#describetargetgroupsinputpaginatetypedef)
