# ElasticLoadBalancing module

> [Index](../README.md) > ElasticLoadBalancing


!!! note ""

    Auto-generated documentation for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#elasticloadbalancing)
    type annotations stubs module [types-aiobotocore-elb](https://pypi.org/project/types-aiobotocore-elb/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `ElasticLoadBalancing` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `ElasticLoadBalancing` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[elb]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[elb]'

# standalone installation
python -m pip install types-aiobotocore-elb
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-elb
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ElasticLoadBalancingClient

Type annotations and code completion for  `#!python session.client("elb")` as [ElasticLoadBalancingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client)

```python
# ElasticLoadBalancingClient usage example

from aioboto3.session import Session

from types_aiobotocore_elb.client import ElasticLoadBalancingClient


session = Session()
async with session.client("elb") as client:
    client: ElasticLoadBalancingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("elb").get_paginator("...")`.

```python
# DescribeAccountLimitsPaginator usage example

from types_aiobotocore_elb.paginator import DescribeAccountLimitsPaginator

def get_describe_account_limits_paginator() -> DescribeAccountLimitsPaginator:
    return client.get_paginator("describe_account_limits"))
```

- [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
- [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.client("elb").get_waiter("...")`.

```python
# AnyInstanceInServiceWaiter usage example

from types_aiobotocore_elb.waiter import AnyInstanceInServiceWaiter

def get_any_instance_in_service_waiter() -> AnyInstanceInServiceWaiter:
    return Session().client("elb").get_waiter("any_instance_in_service")
```

- [AnyInstanceInServiceWaiter](./waiters.md#anyinstanceinservicewaiter)
- [InstanceDeregisteredWaiter](./waiters.md#instancederegisteredwaiter)
- [InstanceInServiceWaiter](./waiters.md#instanceinservicewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AnyInstanceInServiceWaiterName usage example

from types_aiobotocore_elb.literals import AnyInstanceInServiceWaiterName

def get_value() -> AnyInstanceInServiceWaiterName:
    return "any_instance_in_service"
```

- [AnyInstanceInServiceWaiterName](./literals.md#anyinstanceinservicewaitername)
- [DescribeAccountLimitsPaginatorName](./literals.md#describeaccountlimitspaginatorname)
- [DescribeLoadBalancersPaginatorName](./literals.md#describeloadbalancerspaginatorname)
- [InstanceDeregisteredWaiterName](./literals.md#instancederegisteredwaitername)
- [InstanceInServiceWaiterName](./literals.md#instanceinservicewaitername)
- [ElasticLoadBalancingServiceName](./literals.md#elasticloadbalancingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessLogTypeDef](./type_defs.md#accesslogtypedef)
- [AddAvailabilityZonesInputRequestTypeDef](./type_defs.md#addavailabilityzonesinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [AdditionalAttributeTypeDef](./type_defs.md#additionalattributetypedef)
- [AppCookieStickinessPolicyTypeDef](./type_defs.md#appcookiestickinesspolicytypedef)
- [ApplySecurityGroupsToLoadBalancerInputRequestTypeDef](./type_defs.md#applysecuritygroupstoloadbalancerinputrequesttypedef)
- [AttachLoadBalancerToSubnetsInputRequestTypeDef](./type_defs.md#attachloadbalancertosubnetsinputrequesttypedef)
- [BackendServerDescriptionTypeDef](./type_defs.md#backendserverdescriptiontypedef)
- [HealthCheckTypeDef](./type_defs.md#healthchecktypedef)
- [ConnectionDrainingTypeDef](./type_defs.md#connectiondrainingtypedef)
- [ConnectionSettingsTypeDef](./type_defs.md#connectionsettingstypedef)
- [ListenerTypeDef](./type_defs.md#listenertypedef)
- [CreateAppCookieStickinessPolicyInputRequestTypeDef](./type_defs.md#createappcookiestickinesspolicyinputrequesttypedef)
- [CreateLBCookieStickinessPolicyInputRequestTypeDef](./type_defs.md#createlbcookiestickinesspolicyinputrequesttypedef)
- [PolicyAttributeTypeDef](./type_defs.md#policyattributetypedef)
- [CrossZoneLoadBalancingTypeDef](./type_defs.md#crosszoneloadbalancingtypedef)
- [DeleteAccessPointInputRequestTypeDef](./type_defs.md#deleteaccesspointinputrequesttypedef)
- [DeleteLoadBalancerListenerInputRequestTypeDef](./type_defs.md#deleteloadbalancerlistenerinputrequesttypedef)
- [DeleteLoadBalancerPolicyInputRequestTypeDef](./type_defs.md#deleteloadbalancerpolicyinputrequesttypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAccessPointsInputRequestTypeDef](./type_defs.md#describeaccesspointsinputrequesttypedef)
- [DescribeAccountLimitsInputRequestTypeDef](./type_defs.md#describeaccountlimitsinputrequesttypedef)
- [LimitTypeDef](./type_defs.md#limittypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [InstanceStateTypeDef](./type_defs.md#instancestatetypedef)
- [DescribeLoadBalancerAttributesInputRequestTypeDef](./type_defs.md#describeloadbalancerattributesinputrequesttypedef)
- [DescribeLoadBalancerPoliciesInputRequestTypeDef](./type_defs.md#describeloadbalancerpoliciesinputrequesttypedef)
- [DescribeLoadBalancerPolicyTypesInputRequestTypeDef](./type_defs.md#describeloadbalancerpolicytypesinputrequesttypedef)
- [DescribeTagsInputRequestTypeDef](./type_defs.md#describetagsinputrequesttypedef)
- [DetachLoadBalancerFromSubnetsInputRequestTypeDef](./type_defs.md#detachloadbalancerfromsubnetsinputrequesttypedef)
- [LBCookieStickinessPolicyTypeDef](./type_defs.md#lbcookiestickinesspolicytypedef)
- [SourceSecurityGroupTypeDef](./type_defs.md#sourcesecuritygrouptypedef)
- [PolicyAttributeDescriptionTypeDef](./type_defs.md#policyattributedescriptiontypedef)
- [PolicyAttributeTypeDescriptionTypeDef](./type_defs.md#policyattributetypedescriptiontypedef)
- [RemoveAvailabilityZonesInputRequestTypeDef](./type_defs.md#removeavailabilityzonesinputrequesttypedef)
- [TagKeyOnlyTypeDef](./type_defs.md#tagkeyonlytypedef)
- [SetLoadBalancerListenerSSLCertificateInputRequestTypeDef](./type_defs.md#setloadbalancerlistenersslcertificateinputrequesttypedef)
- [SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef](./type_defs.md#setloadbalancerpoliciesforbackendserverinputrequesttypedef)
- [SetLoadBalancerPoliciesOfListenerInputRequestTypeDef](./type_defs.md#setloadbalancerpoliciesoflistenerinputrequesttypedef)
- [AddAvailabilityZonesOutputTypeDef](./type_defs.md#addavailabilityzonesoutputtypedef)
- [ApplySecurityGroupsToLoadBalancerOutputTypeDef](./type_defs.md#applysecuritygroupstoloadbalanceroutputtypedef)
- [AttachLoadBalancerToSubnetsOutputTypeDef](./type_defs.md#attachloadbalancertosubnetsoutputtypedef)
- [CreateAccessPointOutputTypeDef](./type_defs.md#createaccesspointoutputtypedef)
- [DetachLoadBalancerFromSubnetsOutputTypeDef](./type_defs.md#detachloadbalancerfromsubnetsoutputtypedef)
- [RemoveAvailabilityZonesOutputTypeDef](./type_defs.md#removeavailabilityzonesoutputtypedef)
- [AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef)
- [TagDescriptionTypeDef](./type_defs.md#tagdescriptiontypedef)
- [ConfigureHealthCheckInputRequestTypeDef](./type_defs.md#configurehealthcheckinputrequesttypedef)
- [ConfigureHealthCheckOutputTypeDef](./type_defs.md#configurehealthcheckoutputtypedef)
- [CreateAccessPointInputRequestTypeDef](./type_defs.md#createaccesspointinputrequesttypedef)
- [CreateLoadBalancerListenerInputRequestTypeDef](./type_defs.md#createloadbalancerlistenerinputrequesttypedef)
- [ListenerDescriptionTypeDef](./type_defs.md#listenerdescriptiontypedef)
- [CreateLoadBalancerPolicyInputRequestTypeDef](./type_defs.md#createloadbalancerpolicyinputrequesttypedef)
- [LoadBalancerAttributesOutputTypeDef](./type_defs.md#loadbalancerattributesoutputtypedef)
- [LoadBalancerAttributesTypeDef](./type_defs.md#loadbalancerattributestypedef)
- [DeregisterEndPointsInputRequestTypeDef](./type_defs.md#deregisterendpointsinputrequesttypedef)
- [DeregisterEndPointsOutputTypeDef](./type_defs.md#deregisterendpointsoutputtypedef)
- [DescribeEndPointStateInputRequestTypeDef](./type_defs.md#describeendpointstateinputrequesttypedef)
- [RegisterEndPointsInputRequestTypeDef](./type_defs.md#registerendpointsinputrequesttypedef)
- [RegisterEndPointsOutputTypeDef](./type_defs.md#registerendpointsoutputtypedef)
- [DescribeAccessPointsInputPaginateTypeDef](./type_defs.md#describeaccesspointsinputpaginatetypedef)
- [DescribeAccountLimitsInputPaginateTypeDef](./type_defs.md#describeaccountlimitsinputpaginatetypedef)
- [DescribeAccountLimitsOutputTypeDef](./type_defs.md#describeaccountlimitsoutputtypedef)
- [DescribeEndPointStateInputWaitTypeDef](./type_defs.md#describeendpointstateinputwaittypedef)
- [DescribeEndPointStateOutputTypeDef](./type_defs.md#describeendpointstateoutputtypedef)
- [PoliciesTypeDef](./type_defs.md#policiestypedef)
- [PolicyDescriptionTypeDef](./type_defs.md#policydescriptiontypedef)
- [PolicyTypeDescriptionTypeDef](./type_defs.md#policytypedescriptiontypedef)
- [RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef)
- [DescribeTagsOutputTypeDef](./type_defs.md#describetagsoutputtypedef)
- [DescribeLoadBalancerAttributesOutputTypeDef](./type_defs.md#describeloadbalancerattributesoutputtypedef)
- [ModifyLoadBalancerAttributesOutputTypeDef](./type_defs.md#modifyloadbalancerattributesoutputtypedef)
- [ModifyLoadBalancerAttributesInputRequestTypeDef](./type_defs.md#modifyloadbalancerattributesinputrequesttypedef)
- [LoadBalancerDescriptionTypeDef](./type_defs.md#loadbalancerdescriptiontypedef)
- [DescribeLoadBalancerPoliciesOutputTypeDef](./type_defs.md#describeloadbalancerpoliciesoutputtypedef)
- [DescribeLoadBalancerPolicyTypesOutputTypeDef](./type_defs.md#describeloadbalancerpolicytypesoutputtypedef)
- [DescribeAccessPointsOutputTypeDef](./type_defs.md#describeaccesspointsoutputtypedef)
