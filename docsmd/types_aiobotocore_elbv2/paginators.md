# Paginators

> [Index](../README.md) > [ElasticLoadBalancingv2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
    type annotations stubs module [types-aiobotocore-elbv2](https://pypi.org/project/types-aiobotocore-elbv2/).

## DescribeAccountLimitsPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_account_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef](./type_defs.md#describeaccountlimitsinputdescribeaccountlimitspaginatetypedef) 
## DescribeListenerCertificatesPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_listener_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeListenerCertificatesOutputTypeDef](./type_defs.md#describelistenercertificatesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeListenerCertificatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ListenerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeListenerCertificatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeListenerCertificatesOutputTypeDef](./type_defs.md#describelistenercertificatesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef](./type_defs.md#describelistenercertificatesinputdescribelistenercertificatespaginatetypedef) 
## DescribeListenersPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeListenersOutputTypeDef](./type_defs.md#describelistenersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeListenersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerArn: str = ...,
    ListenerArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeListenersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeListenersOutputTypeDef](./type_defs.md#describelistenersoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeListenersInputDescribeListenersPaginateTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeListenersInputDescribeListenersPaginateTypeDef](./type_defs.md#describelistenersinputdescribelistenerspaginatetypedef) 
## DescribeLoadBalancersPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLoadBalancersOutputTypeDef](./type_defs.md#describeloadbalancersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLoadBalancersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeLoadBalancersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLoadBalancersOutputTypeDef](./type_defs.md#describeloadbalancersoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = {  # (1)
    "LoadBalancerArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef](./type_defs.md#describeloadbalancersinputdescribeloadbalancerspaginatetypedef) 
## DescribeRulesPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeRulesOutputTypeDef](./type_defs.md#describerulesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ListenerArn: str = ...,
    RuleArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeRulesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRulesOutputTypeDef](./type_defs.md#describerulesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRulesInputDescribeRulesPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRulesInputDescribeRulesPaginateTypeDef](./type_defs.md#describerulesinputdescriberulespaginatetypedef) 
## DescribeSSLPoliciesPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_ssl_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSSLPoliciesOutputTypeDef](./type_defs.md#describesslpoliciesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSSLPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    LoadBalancerType: LoadBalancerTypeEnumType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSSLPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LoadBalancerTypeEnumType](./literals.md#loadbalancertypeenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSSLPoliciesOutputTypeDef](./type_defs.md#describesslpoliciesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef](./type_defs.md#describesslpoliciesinputdescribesslpoliciespaginatetypedef) 
## DescribeTargetGroupsPaginator

Type annotations and code completion for `#!python session.client("elbv2").get_paginator("describe_target_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTargetGroupsOutputTypeDef](./type_defs.md#describetargetgroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTargetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LoadBalancerArn: str = ...,
    TargetGroupArns: Sequence[str] = ...,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeTargetGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTargetGroupsOutputTypeDef](./type_defs.md#describetargetgroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = {  # (1)
    "LoadBalancerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef](./type_defs.md#describetargetgroupsinputdescribetargetgroupspaginatetypedef) 
