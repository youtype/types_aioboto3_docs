# Route53Resolver module

> [Index](../README.md) > Route53Resolver


!!! note ""

    Auto-generated documentation for [Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#route53resolver)
    type annotations stubs module [types-aiobotocore-route53resolver](https://pypi.org/project/types-aiobotocore-route53resolver/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `Route53Resolver` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `Route53Resolver` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[route53resolver]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[route53resolver]'

# standalone installation
python -m pip install types-aiobotocore-route53resolver
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-route53resolver
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Route53ResolverClient

Type annotations and code completion for  `#!python session.client("route53resolver")` as [Route53ResolverClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client)

```python
# Route53ResolverClient usage example

from aioboto3.session import Session

from types_aiobotocore_route53resolver.client import Route53ResolverClient


session = Session()
async with session.client("route53resolver") as client:
    client: Route53ResolverClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("route53resolver").get_paginator("...")`.

```python
# ListFirewallConfigsPaginator usage example

from types_aiobotocore_route53resolver.paginator import ListFirewallConfigsPaginator

def get_list_firewall_configs_paginator() -> ListFirewallConfigsPaginator:
    return client.get_paginator("list_firewall_configs"))
```

- [ListFirewallConfigsPaginator](./paginators.md#listfirewallconfigspaginator)
- [ListFirewallDomainListsPaginator](./paginators.md#listfirewalldomainlistspaginator)
- [ListFirewallDomainsPaginator](./paginators.md#listfirewalldomainspaginator)
- [ListFirewallRuleGroupAssociationsPaginator](./paginators.md#listfirewallrulegroupassociationspaginator)
- [ListFirewallRuleGroupsPaginator](./paginators.md#listfirewallrulegroupspaginator)
- [ListFirewallRulesPaginator](./paginators.md#listfirewallrulespaginator)
- [ListOutpostResolversPaginator](./paginators.md#listoutpostresolverspaginator)
- [ListResolverConfigsPaginator](./paginators.md#listresolverconfigspaginator)
- [ListResolverDnssecConfigsPaginator](./paginators.md#listresolverdnssecconfigspaginator)
- [ListResolverEndpointIpAddressesPaginator](./paginators.md#listresolverendpointipaddressespaginator)
- [ListResolverEndpointsPaginator](./paginators.md#listresolverendpointspaginator)
- [ListResolverQueryLogConfigAssociationsPaginator](./paginators.md#listresolverquerylogconfigassociationspaginator)
- [ListResolverQueryLogConfigsPaginator](./paginators.md#listresolverquerylogconfigspaginator)
- [ListResolverRuleAssociationsPaginator](./paginators.md#listresolverruleassociationspaginator)
- [ListResolverRulesPaginator](./paginators.md#listresolverrulespaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionType usage example

from types_aiobotocore_route53resolver.literals import ActionType

def get_value() -> ActionType:
    return "ALERT"
```

- [ActionType](./literals.md#actiontype)
- [AutodefinedReverseFlagType](./literals.md#autodefinedreverseflagtype)
- [BlockOverrideDnsTypeType](./literals.md#blockoverridednstypetype)
- [BlockResponseType](./literals.md#blockresponsetype)
- [ConfidenceThresholdType](./literals.md#confidencethresholdtype)
- [DnsThreatProtectionType](./literals.md#dnsthreatprotectiontype)
- [FirewallDomainImportOperationType](./literals.md#firewalldomainimportoperationtype)
- [FirewallDomainListStatusType](./literals.md#firewalldomainliststatustype)
- [FirewallDomainRedirectionActionType](./literals.md#firewalldomainredirectionactiontype)
- [FirewallDomainUpdateOperationType](./literals.md#firewalldomainupdateoperationtype)
- [FirewallFailOpenStatusType](./literals.md#firewallfailopenstatustype)
- [FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype)
- [FirewallRuleGroupStatusType](./literals.md#firewallrulegroupstatustype)
- [IpAddressStatusType](./literals.md#ipaddressstatustype)
- [ListFirewallConfigsPaginatorName](./literals.md#listfirewallconfigspaginatorname)
- [ListFirewallDomainListsPaginatorName](./literals.md#listfirewalldomainlistspaginatorname)
- [ListFirewallDomainsPaginatorName](./literals.md#listfirewalldomainspaginatorname)
- [ListFirewallRuleGroupAssociationsPaginatorName](./literals.md#listfirewallrulegroupassociationspaginatorname)
- [ListFirewallRuleGroupsPaginatorName](./literals.md#listfirewallrulegroupspaginatorname)
- [ListFirewallRulesPaginatorName](./literals.md#listfirewallrulespaginatorname)
- [ListOutpostResolversPaginatorName](./literals.md#listoutpostresolverspaginatorname)
- [ListResolverConfigsPaginatorName](./literals.md#listresolverconfigspaginatorname)
- [ListResolverDnssecConfigsPaginatorName](./literals.md#listresolverdnssecconfigspaginatorname)
- [ListResolverEndpointIpAddressesPaginatorName](./literals.md#listresolverendpointipaddressespaginatorname)
- [ListResolverEndpointsPaginatorName](./literals.md#listresolverendpointspaginatorname)
- [ListResolverQueryLogConfigAssociationsPaginatorName](./literals.md#listresolverquerylogconfigassociationspaginatorname)
- [ListResolverQueryLogConfigsPaginatorName](./literals.md#listresolverquerylogconfigspaginatorname)
- [ListResolverRuleAssociationsPaginatorName](./literals.md#listresolverruleassociationspaginatorname)
- [ListResolverRulesPaginatorName](./literals.md#listresolverrulespaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [MutationProtectionStatusType](./literals.md#mutationprotectionstatustype)
- [OutpostResolverStatusType](./literals.md#outpostresolverstatustype)
- [ProtocolType](./literals.md#protocoltype)
- [ResolverAutodefinedReverseStatusType](./literals.md#resolverautodefinedreversestatustype)
- [ResolverDNSSECValidationStatusType](./literals.md#resolverdnssecvalidationstatustype)
- [ResolverEndpointDirectionType](./literals.md#resolverendpointdirectiontype)
- [ResolverEndpointStatusType](./literals.md#resolverendpointstatustype)
- [ResolverEndpointTypeType](./literals.md#resolverendpointtypetype)
- [ResolverQueryLogConfigAssociationErrorType](./literals.md#resolverquerylogconfigassociationerrortype)
- [ResolverQueryLogConfigAssociationStatusType](./literals.md#resolverquerylogconfigassociationstatustype)
- [ResolverQueryLogConfigStatusType](./literals.md#resolverquerylogconfigstatustype)
- [ResolverRuleAssociationStatusType](./literals.md#resolverruleassociationstatustype)
- [ResolverRuleStatusType](./literals.md#resolverrulestatustype)
- [RuleTypeOptionType](./literals.md#ruletypeoptiontype)
- [ShareStatusType](./literals.md#sharestatustype)
- [SortOrderType](./literals.md#sortordertype)
- [ValidationType](./literals.md#validationtype)
- [Route53ResolverServiceName](./literals.md#route53resolverservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TagTypeDef](./type_defs.md#tagtypedef)
- [FirewallRuleGroupAssociationTypeDef](./type_defs.md#firewallrulegroupassociationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [IpAddressUpdateTypeDef](./type_defs.md#ipaddressupdatetypedef)
- [ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef)
- [AssociateResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#associateresolverquerylogconfigrequestrequesttypedef)
- [ResolverQueryLogConfigAssociationTypeDef](./type_defs.md#resolverquerylogconfigassociationtypedef)
- [AssociateResolverRuleRequestRequestTypeDef](./type_defs.md#associateresolverrulerequestrequesttypedef)
- [ResolverRuleAssociationTypeDef](./type_defs.md#resolverruleassociationtypedef)
- [FirewallDomainListTypeDef](./type_defs.md#firewalldomainlisttypedef)
- [FirewallRuleGroupTypeDef](./type_defs.md#firewallrulegrouptypedef)
- [CreateFirewallRuleRequestRequestTypeDef](./type_defs.md#createfirewallrulerequestrequesttypedef)
- [FirewallRuleTypeDef](./type_defs.md#firewallruletypedef)
- [OutpostResolverTypeDef](./type_defs.md#outpostresolvertypedef)
- [IpAddressRequestTypeDef](./type_defs.md#ipaddressrequesttypedef)
- [ResolverQueryLogConfigTypeDef](./type_defs.md#resolverquerylogconfigtypedef)
- [TargetAddressTypeDef](./type_defs.md#targetaddresstypedef)
- [DeleteFirewallDomainListRequestRequestTypeDef](./type_defs.md#deletefirewalldomainlistrequestrequesttypedef)
- [DeleteFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#deletefirewallrulegrouprequestrequesttypedef)
- [DeleteFirewallRuleRequestRequestTypeDef](./type_defs.md#deletefirewallrulerequestrequesttypedef)
- [DeleteOutpostResolverRequestRequestTypeDef](./type_defs.md#deleteoutpostresolverrequestrequesttypedef)
- [DeleteResolverEndpointRequestRequestTypeDef](./type_defs.md#deleteresolverendpointrequestrequesttypedef)
- [DeleteResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#deleteresolverquerylogconfigrequestrequesttypedef)
- [DeleteResolverRuleRequestRequestTypeDef](./type_defs.md#deleteresolverrulerequestrequesttypedef)
- [DisassociateFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#disassociatefirewallrulegrouprequestrequesttypedef)
- [DisassociateResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#disassociateresolverquerylogconfigrequestrequesttypedef)
- [DisassociateResolverRuleRequestRequestTypeDef](./type_defs.md#disassociateresolverrulerequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [FirewallConfigTypeDef](./type_defs.md#firewallconfigtypedef)
- [FirewallDomainListMetadataTypeDef](./type_defs.md#firewalldomainlistmetadatatypedef)
- [FirewallRuleGroupMetadataTypeDef](./type_defs.md#firewallrulegroupmetadatatypedef)
- [GetFirewallConfigRequestRequestTypeDef](./type_defs.md#getfirewallconfigrequestrequesttypedef)
- [GetFirewallDomainListRequestRequestTypeDef](./type_defs.md#getfirewalldomainlistrequestrequesttypedef)
- [GetFirewallRuleGroupAssociationRequestRequestTypeDef](./type_defs.md#getfirewallrulegroupassociationrequestrequesttypedef)
- [GetFirewallRuleGroupPolicyRequestRequestTypeDef](./type_defs.md#getfirewallrulegrouppolicyrequestrequesttypedef)
- [GetFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#getfirewallrulegrouprequestrequesttypedef)
- [GetOutpostResolverRequestRequestTypeDef](./type_defs.md#getoutpostresolverrequestrequesttypedef)
- [GetResolverConfigRequestRequestTypeDef](./type_defs.md#getresolverconfigrequestrequesttypedef)
- [ResolverConfigTypeDef](./type_defs.md#resolverconfigtypedef)
- [GetResolverDnssecConfigRequestRequestTypeDef](./type_defs.md#getresolverdnssecconfigrequestrequesttypedef)
- [ResolverDnssecConfigTypeDef](./type_defs.md#resolverdnssecconfigtypedef)
- [GetResolverEndpointRequestRequestTypeDef](./type_defs.md#getresolverendpointrequestrequesttypedef)
- [GetResolverQueryLogConfigAssociationRequestRequestTypeDef](./type_defs.md#getresolverquerylogconfigassociationrequestrequesttypedef)
- [GetResolverQueryLogConfigPolicyRequestRequestTypeDef](./type_defs.md#getresolverquerylogconfigpolicyrequestrequesttypedef)
- [GetResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#getresolverquerylogconfigrequestrequesttypedef)
- [GetResolverRuleAssociationRequestRequestTypeDef](./type_defs.md#getresolverruleassociationrequestrequesttypedef)
- [GetResolverRulePolicyRequestRequestTypeDef](./type_defs.md#getresolverrulepolicyrequestrequesttypedef)
- [GetResolverRuleRequestRequestTypeDef](./type_defs.md#getresolverrulerequestrequesttypedef)
- [ImportFirewallDomainsRequestRequestTypeDef](./type_defs.md#importfirewalldomainsrequestrequesttypedef)
- [IpAddressResponseTypeDef](./type_defs.md#ipaddressresponsetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListFirewallConfigsRequestRequestTypeDef](./type_defs.md#listfirewallconfigsrequestrequesttypedef)
- [ListFirewallDomainListsRequestRequestTypeDef](./type_defs.md#listfirewalldomainlistsrequestrequesttypedef)
- [ListFirewallDomainsRequestRequestTypeDef](./type_defs.md#listfirewalldomainsrequestrequesttypedef)
- [ListFirewallRuleGroupAssociationsRequestRequestTypeDef](./type_defs.md#listfirewallrulegroupassociationsrequestrequesttypedef)
- [ListFirewallRuleGroupsRequestRequestTypeDef](./type_defs.md#listfirewallrulegroupsrequestrequesttypedef)
- [ListFirewallRulesRequestRequestTypeDef](./type_defs.md#listfirewallrulesrequestrequesttypedef)
- [ListOutpostResolversRequestRequestTypeDef](./type_defs.md#listoutpostresolversrequestrequesttypedef)
- [ListResolverConfigsRequestRequestTypeDef](./type_defs.md#listresolverconfigsrequestrequesttypedef)
- [ListResolverEndpointIpAddressesRequestRequestTypeDef](./type_defs.md#listresolverendpointipaddressesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PutFirewallRuleGroupPolicyRequestRequestTypeDef](./type_defs.md#putfirewallrulegrouppolicyrequestrequesttypedef)
- [PutResolverQueryLogConfigPolicyRequestRequestTypeDef](./type_defs.md#putresolverquerylogconfigpolicyrequestrequesttypedef)
- [PutResolverRulePolicyRequestRequestTypeDef](./type_defs.md#putresolverrulepolicyrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFirewallConfigRequestRequestTypeDef](./type_defs.md#updatefirewallconfigrequestrequesttypedef)
- [UpdateFirewallDomainsRequestRequestTypeDef](./type_defs.md#updatefirewalldomainsrequestrequesttypedef)
- [UpdateFirewallRuleGroupAssociationRequestRequestTypeDef](./type_defs.md#updatefirewallrulegroupassociationrequestrequesttypedef)
- [UpdateFirewallRuleRequestRequestTypeDef](./type_defs.md#updatefirewallrulerequestrequesttypedef)
- [UpdateIpAddressTypeDef](./type_defs.md#updateipaddresstypedef)
- [UpdateOutpostResolverRequestRequestTypeDef](./type_defs.md#updateoutpostresolverrequestrequesttypedef)
- [UpdateResolverConfigRequestRequestTypeDef](./type_defs.md#updateresolverconfigrequestrequesttypedef)
- [UpdateResolverDnssecConfigRequestRequestTypeDef](./type_defs.md#updateresolverdnssecconfigrequestrequesttypedef)
- [AssociateFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#associatefirewallrulegrouprequestrequesttypedef)
- [CreateFirewallDomainListRequestRequestTypeDef](./type_defs.md#createfirewalldomainlistrequestrequesttypedef)
- [CreateFirewallRuleGroupRequestRequestTypeDef](./type_defs.md#createfirewallrulegrouprequestrequesttypedef)
- [CreateOutpostResolverRequestRequestTypeDef](./type_defs.md#createoutpostresolverrequestrequesttypedef)
- [CreateResolverQueryLogConfigRequestRequestTypeDef](./type_defs.md#createresolverquerylogconfigrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [AssociateFirewallRuleGroupResponseTypeDef](./type_defs.md#associatefirewallrulegroupresponsetypedef)
- [DisassociateFirewallRuleGroupResponseTypeDef](./type_defs.md#disassociatefirewallrulegroupresponsetypedef)
- [GetFirewallRuleGroupAssociationResponseTypeDef](./type_defs.md#getfirewallrulegroupassociationresponsetypedef)
- [GetFirewallRuleGroupPolicyResponseTypeDef](./type_defs.md#getfirewallrulegrouppolicyresponsetypedef)
- [GetResolverQueryLogConfigPolicyResponseTypeDef](./type_defs.md#getresolverquerylogconfigpolicyresponsetypedef)
- [GetResolverRulePolicyResponseTypeDef](./type_defs.md#getresolverrulepolicyresponsetypedef)
- [ImportFirewallDomainsResponseTypeDef](./type_defs.md#importfirewalldomainsresponsetypedef)
- [ListFirewallDomainsResponseTypeDef](./type_defs.md#listfirewalldomainsresponsetypedef)
- [ListFirewallRuleGroupAssociationsResponseTypeDef](./type_defs.md#listfirewallrulegroupassociationsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutFirewallRuleGroupPolicyResponseTypeDef](./type_defs.md#putfirewallrulegrouppolicyresponsetypedef)
- [PutResolverQueryLogConfigPolicyResponseTypeDef](./type_defs.md#putresolverquerylogconfigpolicyresponsetypedef)
- [PutResolverRulePolicyResponseTypeDef](./type_defs.md#putresolverrulepolicyresponsetypedef)
- [UpdateFirewallDomainsResponseTypeDef](./type_defs.md#updatefirewalldomainsresponsetypedef)
- [UpdateFirewallRuleGroupAssociationResponseTypeDef](./type_defs.md#updatefirewallrulegroupassociationresponsetypedef)
- [AssociateResolverEndpointIpAddressRequestRequestTypeDef](./type_defs.md#associateresolverendpointipaddressrequestrequesttypedef)
- [DisassociateResolverEndpointIpAddressRequestRequestTypeDef](./type_defs.md#disassociateresolverendpointipaddressrequestrequesttypedef)
- [AssociateResolverEndpointIpAddressResponseTypeDef](./type_defs.md#associateresolverendpointipaddressresponsetypedef)
- [CreateResolverEndpointResponseTypeDef](./type_defs.md#createresolverendpointresponsetypedef)
- [DeleteResolverEndpointResponseTypeDef](./type_defs.md#deleteresolverendpointresponsetypedef)
- [DisassociateResolverEndpointIpAddressResponseTypeDef](./type_defs.md#disassociateresolverendpointipaddressresponsetypedef)
- [GetResolverEndpointResponseTypeDef](./type_defs.md#getresolverendpointresponsetypedef)
- [ListResolverEndpointsResponseTypeDef](./type_defs.md#listresolverendpointsresponsetypedef)
- [UpdateResolverEndpointResponseTypeDef](./type_defs.md#updateresolverendpointresponsetypedef)
- [AssociateResolverQueryLogConfigResponseTypeDef](./type_defs.md#associateresolverquerylogconfigresponsetypedef)
- [DisassociateResolverQueryLogConfigResponseTypeDef](./type_defs.md#disassociateresolverquerylogconfigresponsetypedef)
- [GetResolverQueryLogConfigAssociationResponseTypeDef](./type_defs.md#getresolverquerylogconfigassociationresponsetypedef)
- [ListResolverQueryLogConfigAssociationsResponseTypeDef](./type_defs.md#listresolverquerylogconfigassociationsresponsetypedef)
- [AssociateResolverRuleResponseTypeDef](./type_defs.md#associateresolverruleresponsetypedef)
- [DisassociateResolverRuleResponseTypeDef](./type_defs.md#disassociateresolverruleresponsetypedef)
- [GetResolverRuleAssociationResponseTypeDef](./type_defs.md#getresolverruleassociationresponsetypedef)
- [ListResolverRuleAssociationsResponseTypeDef](./type_defs.md#listresolverruleassociationsresponsetypedef)
- [CreateFirewallDomainListResponseTypeDef](./type_defs.md#createfirewalldomainlistresponsetypedef)
- [DeleteFirewallDomainListResponseTypeDef](./type_defs.md#deletefirewalldomainlistresponsetypedef)
- [GetFirewallDomainListResponseTypeDef](./type_defs.md#getfirewalldomainlistresponsetypedef)
- [CreateFirewallRuleGroupResponseTypeDef](./type_defs.md#createfirewallrulegroupresponsetypedef)
- [DeleteFirewallRuleGroupResponseTypeDef](./type_defs.md#deletefirewallrulegroupresponsetypedef)
- [GetFirewallRuleGroupResponseTypeDef](./type_defs.md#getfirewallrulegroupresponsetypedef)
- [CreateFirewallRuleResponseTypeDef](./type_defs.md#createfirewallruleresponsetypedef)
- [DeleteFirewallRuleResponseTypeDef](./type_defs.md#deletefirewallruleresponsetypedef)
- [ListFirewallRulesResponseTypeDef](./type_defs.md#listfirewallrulesresponsetypedef)
- [UpdateFirewallRuleResponseTypeDef](./type_defs.md#updatefirewallruleresponsetypedef)
- [CreateOutpostResolverResponseTypeDef](./type_defs.md#createoutpostresolverresponsetypedef)
- [DeleteOutpostResolverResponseTypeDef](./type_defs.md#deleteoutpostresolverresponsetypedef)
- [GetOutpostResolverResponseTypeDef](./type_defs.md#getoutpostresolverresponsetypedef)
- [ListOutpostResolversResponseTypeDef](./type_defs.md#listoutpostresolversresponsetypedef)
- [UpdateOutpostResolverResponseTypeDef](./type_defs.md#updateoutpostresolverresponsetypedef)
- [CreateResolverEndpointRequestRequestTypeDef](./type_defs.md#createresolverendpointrequestrequesttypedef)
- [CreateResolverQueryLogConfigResponseTypeDef](./type_defs.md#createresolverquerylogconfigresponsetypedef)
- [DeleteResolverQueryLogConfigResponseTypeDef](./type_defs.md#deleteresolverquerylogconfigresponsetypedef)
- [GetResolverQueryLogConfigResponseTypeDef](./type_defs.md#getresolverquerylogconfigresponsetypedef)
- [ListResolverQueryLogConfigsResponseTypeDef](./type_defs.md#listresolverquerylogconfigsresponsetypedef)
- [CreateResolverRuleRequestRequestTypeDef](./type_defs.md#createresolverrulerequestrequesttypedef)
- [ResolverRuleConfigTypeDef](./type_defs.md#resolverruleconfigtypedef)
- [ResolverRuleTypeDef](./type_defs.md#resolverruletypedef)
- [ListResolverDnssecConfigsRequestRequestTypeDef](./type_defs.md#listresolverdnssecconfigsrequestrequesttypedef)
- [ListResolverEndpointsRequestRequestTypeDef](./type_defs.md#listresolverendpointsrequestrequesttypedef)
- [ListResolverQueryLogConfigAssociationsRequestRequestTypeDef](./type_defs.md#listresolverquerylogconfigassociationsrequestrequesttypedef)
- [ListResolverQueryLogConfigsRequestRequestTypeDef](./type_defs.md#listresolverquerylogconfigsrequestrequesttypedef)
- [ListResolverRuleAssociationsRequestRequestTypeDef](./type_defs.md#listresolverruleassociationsrequestrequesttypedef)
- [ListResolverRulesRequestRequestTypeDef](./type_defs.md#listresolverrulesrequestrequesttypedef)
- [GetFirewallConfigResponseTypeDef](./type_defs.md#getfirewallconfigresponsetypedef)
- [ListFirewallConfigsResponseTypeDef](./type_defs.md#listfirewallconfigsresponsetypedef)
- [UpdateFirewallConfigResponseTypeDef](./type_defs.md#updatefirewallconfigresponsetypedef)
- [ListFirewallDomainListsResponseTypeDef](./type_defs.md#listfirewalldomainlistsresponsetypedef)
- [ListFirewallRuleGroupsResponseTypeDef](./type_defs.md#listfirewallrulegroupsresponsetypedef)
- [GetResolverConfigResponseTypeDef](./type_defs.md#getresolverconfigresponsetypedef)
- [ListResolverConfigsResponseTypeDef](./type_defs.md#listresolverconfigsresponsetypedef)
- [UpdateResolverConfigResponseTypeDef](./type_defs.md#updateresolverconfigresponsetypedef)
- [GetResolverDnssecConfigResponseTypeDef](./type_defs.md#getresolverdnssecconfigresponsetypedef)
- [ListResolverDnssecConfigsResponseTypeDef](./type_defs.md#listresolverdnssecconfigsresponsetypedef)
- [UpdateResolverDnssecConfigResponseTypeDef](./type_defs.md#updateresolverdnssecconfigresponsetypedef)
- [ListResolverEndpointIpAddressesResponseTypeDef](./type_defs.md#listresolverendpointipaddressesresponsetypedef)
- [ListFirewallConfigsRequestPaginateTypeDef](./type_defs.md#listfirewallconfigsrequestpaginatetypedef)
- [ListFirewallDomainListsRequestPaginateTypeDef](./type_defs.md#listfirewalldomainlistsrequestpaginatetypedef)
- [ListFirewallDomainsRequestPaginateTypeDef](./type_defs.md#listfirewalldomainsrequestpaginatetypedef)
- [ListFirewallRuleGroupAssociationsRequestPaginateTypeDef](./type_defs.md#listfirewallrulegroupassociationsrequestpaginatetypedef)
- [ListFirewallRuleGroupsRequestPaginateTypeDef](./type_defs.md#listfirewallrulegroupsrequestpaginatetypedef)
- [ListFirewallRulesRequestPaginateTypeDef](./type_defs.md#listfirewallrulesrequestpaginatetypedef)
- [ListOutpostResolversRequestPaginateTypeDef](./type_defs.md#listoutpostresolversrequestpaginatetypedef)
- [ListResolverConfigsRequestPaginateTypeDef](./type_defs.md#listresolverconfigsrequestpaginatetypedef)
- [ListResolverDnssecConfigsRequestPaginateTypeDef](./type_defs.md#listresolverdnssecconfigsrequestpaginatetypedef)
- [ListResolverEndpointIpAddressesRequestPaginateTypeDef](./type_defs.md#listresolverendpointipaddressesrequestpaginatetypedef)
- [ListResolverEndpointsRequestPaginateTypeDef](./type_defs.md#listresolverendpointsrequestpaginatetypedef)
- [ListResolverQueryLogConfigAssociationsRequestPaginateTypeDef](./type_defs.md#listresolverquerylogconfigassociationsrequestpaginatetypedef)
- [ListResolverQueryLogConfigsRequestPaginateTypeDef](./type_defs.md#listresolverquerylogconfigsrequestpaginatetypedef)
- [ListResolverRuleAssociationsRequestPaginateTypeDef](./type_defs.md#listresolverruleassociationsrequestpaginatetypedef)
- [ListResolverRulesRequestPaginateTypeDef](./type_defs.md#listresolverrulesrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [UpdateResolverEndpointRequestRequestTypeDef](./type_defs.md#updateresolverendpointrequestrequesttypedef)
- [UpdateResolverRuleRequestRequestTypeDef](./type_defs.md#updateresolverrulerequestrequesttypedef)
- [CreateResolverRuleResponseTypeDef](./type_defs.md#createresolverruleresponsetypedef)
- [DeleteResolverRuleResponseTypeDef](./type_defs.md#deleteresolverruleresponsetypedef)
- [GetResolverRuleResponseTypeDef](./type_defs.md#getresolverruleresponsetypedef)
- [ListResolverRulesResponseTypeDef](./type_defs.md#listresolverrulesresponsetypedef)
- [UpdateResolverRuleResponseTypeDef](./type_defs.md#updateresolverruleresponsetypedef)
