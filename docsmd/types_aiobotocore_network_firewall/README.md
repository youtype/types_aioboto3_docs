# NetworkFirewall module

> [Index](../README.md) > NetworkFirewall


!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `NetworkFirewall` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[network-firewall]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[network-firewall]'


# standalone installation
python -m pip install types-aiobotocore-network-firewall
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-network-firewall
```

## Usage

Code samples can be found in [Examples](./usage.md).

## NetworkFirewallClient

Type annotations and code completion for  `#!python session.client("network-firewall")` as [NetworkFirewallClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_network_firewall.client import NetworkFirewallClient


session = Session()
async with session.client("network-firewall") as client:
    client: NetworkFirewallClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("network-firewall").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_network_firewall.paginator import ListFirewallPoliciesPaginator

def get_list_firewall_policies_paginator() -> ListFirewallPoliciesPaginator:
    return client.get_paginator("list_firewall_policies"))
```

- [ListFirewallPoliciesPaginator](./paginators.md#listfirewallpoliciespaginator)
- [ListFirewallsPaginator](./paginators.md#listfirewallspaginator)
- [ListRuleGroupsPaginator](./paginators.md#listrulegroupspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_network_firewall.literals import AttachmentStatusType

def get_value() -> AttachmentStatusType:
    return "CREATING"
```

- [AttachmentStatusType](./literals.md#attachmentstatustype)
- [ConfigurationSyncStateType](./literals.md#configurationsyncstatetype)
- [FirewallStatusValueType](./literals.md#firewallstatusvaluetype)
- [GeneratedRulesTypeType](./literals.md#generatedrulestypetype)
- [ListFirewallPoliciesPaginatorName](./literals.md#listfirewallpoliciespaginatorname)
- [ListFirewallsPaginatorName](./literals.md#listfirewallspaginatorname)
- [ListRuleGroupsPaginatorName](./literals.md#listrulegroupspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [LogDestinationTypeType](./literals.md#logdestinationtypetype)
- [LogTypeType](./literals.md#logtypetype)
- [OverrideActionType](./literals.md#overrideactiontype)
- [PerObjectSyncStatusType](./literals.md#perobjectsyncstatustype)
- [ResourceManagedStatusType](./literals.md#resourcemanagedstatustype)
- [ResourceStatusType](./literals.md#resourcestatustype)
- [RuleGroupTypeType](./literals.md#rulegrouptypetype)
- [RuleOrderType](./literals.md#ruleordertype)
- [StatefulActionType](./literals.md#statefulactiontype)
- [StatefulRuleDirectionType](./literals.md#statefulruledirectiontype)
- [StatefulRuleProtocolType](./literals.md#statefulruleprotocoltype)
- [TCPFlagType](./literals.md#tcpflagtype)
- [TargetTypeType](./literals.md#targettypetype)
- [NetworkFirewallServiceName](./literals.md#networkfirewallservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_network_firewall.type_defs import AddressTypeDef

def get_value() -> AddressTypeDef:
    return {
        "AddressDefinition": ...,
    }
```

- [AddressTypeDef](./type_defs.md#addresstypedef)
- [AssociateFirewallPolicyRequestRequestTypeDef](./type_defs.md#associatefirewallpolicyrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef)
- [AttachmentTypeDef](./type_defs.md#attachmenttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteFirewallPolicyRequestRequestTypeDef](./type_defs.md#deletefirewallpolicyrequestrequesttypedef)
- [DeleteFirewallRequestRequestTypeDef](./type_defs.md#deletefirewallrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRuleGroupRequestRequestTypeDef](./type_defs.md#deleterulegrouprequestrequesttypedef)
- [DescribeFirewallPolicyRequestRequestTypeDef](./type_defs.md#describefirewallpolicyrequestrequesttypedef)
- [DescribeFirewallRequestRequestTypeDef](./type_defs.md#describefirewallrequestrequesttypedef)
- [DescribeLoggingConfigurationRequestRequestTypeDef](./type_defs.md#describeloggingconfigurationrequestrequesttypedef)
- [DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef)
- [DescribeRuleGroupMetadataRequestRequestTypeDef](./type_defs.md#describerulegroupmetadatarequestrequesttypedef)
- [StatefulRuleOptionsTypeDef](./type_defs.md#statefulruleoptionstypedef)
- [DescribeRuleGroupRequestRequestTypeDef](./type_defs.md#describerulegrouprequestrequesttypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [DisassociateSubnetsRequestRequestTypeDef](./type_defs.md#disassociatesubnetsrequestrequesttypedef)
- [FirewallMetadataTypeDef](./type_defs.md#firewallmetadatatypedef)
- [FirewallPolicyMetadataTypeDef](./type_defs.md#firewallpolicymetadatatypedef)
- [StatefulEngineOptionsTypeDef](./type_defs.md#statefulengineoptionstypedef)
- [StatelessRuleGroupReferenceTypeDef](./type_defs.md#statelessrulegroupreferencetypedef)
- [HeaderTypeDef](./type_defs.md#headertypedef)
- [IPSetTypeDef](./type_defs.md#ipsettypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListFirewallPoliciesRequestRequestTypeDef](./type_defs.md#listfirewallpoliciesrequestrequesttypedef)
- [ListFirewallsRequestRequestTypeDef](./type_defs.md#listfirewallsrequestrequesttypedef)
- [ListRuleGroupsRequestRequestTypeDef](./type_defs.md#listrulegroupsrequestrequesttypedef)
- [RuleGroupMetadataTypeDef](./type_defs.md#rulegroupmetadatatypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LogDestinationConfigTypeDef](./type_defs.md#logdestinationconfigtypedef)
- [PortRangeTypeDef](./type_defs.md#portrangetypedef)
- [TCPFlagFieldTypeDef](./type_defs.md#tcpflagfieldtypedef)
- [PerObjectStatusTypeDef](./type_defs.md#perobjectstatustypedef)
- [PortSetTypeDef](./type_defs.md#portsettypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [RuleOptionTypeDef](./type_defs.md#ruleoptiontypedef)
- [RulesSourceListTypeDef](./type_defs.md#rulessourcelisttypedef)
- [StatefulRuleGroupOverrideTypeDef](./type_defs.md#statefulrulegroupoverridetypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFirewallDeleteProtectionRequestRequestTypeDef](./type_defs.md#updatefirewalldeleteprotectionrequestrequesttypedef)
- [UpdateFirewallDescriptionRequestRequestTypeDef](./type_defs.md#updatefirewalldescriptionrequestrequesttypedef)
- [UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef](./type_defs.md#updatefirewallpolicychangeprotectionrequestrequesttypedef)
- [UpdateSubnetChangeProtectionRequestRequestTypeDef](./type_defs.md#updatesubnetchangeprotectionrequestrequesttypedef)
- [AssociateFirewallPolicyResponseTypeDef](./type_defs.md#associatefirewallpolicyresponsetypedef)
- [DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef)
- [UpdateFirewallDeleteProtectionResponseTypeDef](./type_defs.md#updatefirewalldeleteprotectionresponsetypedef)
- [UpdateFirewallDescriptionResponseTypeDef](./type_defs.md#updatefirewalldescriptionresponsetypedef)
- [UpdateFirewallPolicyChangeProtectionResponseTypeDef](./type_defs.md#updatefirewallpolicychangeprotectionresponsetypedef)
- [UpdateSubnetChangeProtectionResponseTypeDef](./type_defs.md#updatesubnetchangeprotectionresponsetypedef)
- [AssociateSubnetsRequestRequestTypeDef](./type_defs.md#associatesubnetsrequestrequesttypedef)
- [AssociateSubnetsResponseTypeDef](./type_defs.md#associatesubnetsresponsetypedef)
- [DisassociateSubnetsResponseTypeDef](./type_defs.md#disassociatesubnetsresponsetypedef)
- [CreateFirewallRequestRequestTypeDef](./type_defs.md#createfirewallrequestrequesttypedef)
- [FirewallPolicyResponseTypeDef](./type_defs.md#firewallpolicyresponsetypedef)
- [FirewallTypeDef](./type_defs.md#firewalltypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RuleGroupResponseTypeDef](./type_defs.md#rulegroupresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [DescribeRuleGroupMetadataResponseTypeDef](./type_defs.md#describerulegroupmetadataresponsetypedef)
- [PublishMetricActionTypeDef](./type_defs.md#publishmetricactiontypedef)
- [ListFirewallsResponseTypeDef](./type_defs.md#listfirewallsresponsetypedef)
- [ListFirewallPoliciesResponseTypeDef](./type_defs.md#listfirewallpoliciesresponsetypedef)
- [ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef](./type_defs.md#listfirewallpoliciesrequestlistfirewallpoliciespaginatetypedef)
- [ListFirewallsRequestListFirewallsPaginateTypeDef](./type_defs.md#listfirewallsrequestlistfirewallspaginatetypedef)
- [ListRuleGroupsRequestListRuleGroupsPaginateTypeDef](./type_defs.md#listrulegroupsrequestlistrulegroupspaginatetypedef)
- [ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef)
- [ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef)
- [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- [MatchAttributesTypeDef](./type_defs.md#matchattributestypedef)
- [SyncStateTypeDef](./type_defs.md#syncstatetypedef)
- [RuleVariablesTypeDef](./type_defs.md#rulevariablestypedef)
- [StatefulRuleTypeDef](./type_defs.md#statefulruletypedef)
- [StatefulRuleGroupReferenceTypeDef](./type_defs.md#statefulrulegroupreferencetypedef)
- [CreateFirewallPolicyResponseTypeDef](./type_defs.md#createfirewallpolicyresponsetypedef)
- [DeleteFirewallPolicyResponseTypeDef](./type_defs.md#deletefirewallpolicyresponsetypedef)
- [UpdateFirewallPolicyResponseTypeDef](./type_defs.md#updatefirewallpolicyresponsetypedef)
- [CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef)
- [DeleteRuleGroupResponseTypeDef](./type_defs.md#deleterulegroupresponsetypedef)
- [UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef)
- [ActionDefinitionTypeDef](./type_defs.md#actiondefinitiontypedef)
- [DescribeLoggingConfigurationResponseTypeDef](./type_defs.md#describeloggingconfigurationresponsetypedef)
- [UpdateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#updateloggingconfigurationrequestrequesttypedef)
- [UpdateLoggingConfigurationResponseTypeDef](./type_defs.md#updateloggingconfigurationresponsetypedef)
- [RuleDefinitionTypeDef](./type_defs.md#ruledefinitiontypedef)
- [FirewallStatusTypeDef](./type_defs.md#firewallstatustypedef)
- [CustomActionTypeDef](./type_defs.md#customactiontypedef)
- [StatelessRuleTypeDef](./type_defs.md#statelessruletypedef)
- [CreateFirewallResponseTypeDef](./type_defs.md#createfirewallresponsetypedef)
- [DeleteFirewallResponseTypeDef](./type_defs.md#deletefirewallresponsetypedef)
- [DescribeFirewallResponseTypeDef](./type_defs.md#describefirewallresponsetypedef)
- [FirewallPolicyTypeDef](./type_defs.md#firewallpolicytypedef)
- [StatelessRulesAndCustomActionsTypeDef](./type_defs.md#statelessrulesandcustomactionstypedef)
- [CreateFirewallPolicyRequestRequestTypeDef](./type_defs.md#createfirewallpolicyrequestrequesttypedef)
- [DescribeFirewallPolicyResponseTypeDef](./type_defs.md#describefirewallpolicyresponsetypedef)
- [UpdateFirewallPolicyRequestRequestTypeDef](./type_defs.md#updatefirewallpolicyrequestrequesttypedef)
- [RulesSourceTypeDef](./type_defs.md#rulessourcetypedef)
- [RuleGroupTypeDef](./type_defs.md#rulegrouptypedef)
- [CreateRuleGroupRequestRequestTypeDef](./type_defs.md#createrulegrouprequestrequesttypedef)
- [DescribeRuleGroupResponseTypeDef](./type_defs.md#describerulegroupresponsetypedef)
- [UpdateRuleGroupRequestRequestTypeDef](./type_defs.md#updaterulegrouprequestrequesttypedef)

