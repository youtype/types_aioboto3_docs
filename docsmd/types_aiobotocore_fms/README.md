# FMS module

> [Index](../README.md) > FMS


!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `FMS`.

### From PyPI with pip

Install `types-aioboto3` for `FMS` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[fms]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[fms]'


# standalone installation
python -m pip install types-aiobotocore-fms
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-fms
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FMSClient

Type annotations and code completion for  `#!python session.client("fms")` as [FMSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_fms.client import FMSClient


session = Session()
async with session.client("fms") as client:
    client: FMSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("fms").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_fms.paginator import ListAppsListsPaginator

def get_list_apps_lists_paginator() -> ListAppsListsPaginator:
    return client.get_paginator("list_apps_lists"))
```

- [ListAppsListsPaginator](./paginators.md#listappslistspaginator)
- [ListComplianceStatusPaginator](./paginators.md#listcompliancestatuspaginator)
- [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
- [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- [ListProtocolsListsPaginator](./paginators.md#listprotocolslistspaginator)
- [ListThirdPartyFirewallFirewallPoliciesPaginator](./paginators.md#listthirdpartyfirewallfirewallpoliciespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_fms.literals import AccountRoleStatusType

def get_value() -> AccountRoleStatusType:
    return "CREATING"
```

- [AccountRoleStatusType](./literals.md#accountrolestatustype)
- [CustomerPolicyScopeIdTypeType](./literals.md#customerpolicyscopeidtypetype)
- [DependentServiceNameType](./literals.md#dependentservicenametype)
- [DestinationTypeType](./literals.md#destinationtypetype)
- [FirewallDeploymentModelType](./literals.md#firewalldeploymentmodeltype)
- [ListAppsListsPaginatorName](./literals.md#listappslistspaginatorname)
- [ListComplianceStatusPaginatorName](./literals.md#listcompliancestatuspaginatorname)
- [ListMemberAccountsPaginatorName](./literals.md#listmemberaccountspaginatorname)
- [ListPoliciesPaginatorName](./literals.md#listpoliciespaginatorname)
- [ListProtocolsListsPaginatorName](./literals.md#listprotocolslistspaginatorname)
- [ListThirdPartyFirewallFirewallPoliciesPaginatorName](./literals.md#listthirdpartyfirewallfirewallpoliciespaginatorname)
- [MarketplaceSubscriptionOnboardingStatusType](./literals.md#marketplacesubscriptiononboardingstatustype)
- [PolicyComplianceStatusTypeType](./literals.md#policycompliancestatustypetype)
- [RemediationActionTypeType](./literals.md#remediationactiontypetype)
- [SecurityServiceTypeType](./literals.md#securityservicetypetype)
- [TargetTypeType](./literals.md#targettypetype)
- [ThirdPartyFirewallAssociationStatusType](./literals.md#thirdpartyfirewallassociationstatustype)
- [ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype)
- [ViolationReasonType](./literals.md#violationreasontype)
- [FMSServiceName](./literals.md#fmsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_fms.type_defs import ActionTargetTypeDef

def get_value() -> ActionTargetTypeDef:
    return {
        "ResourceId": ...,
    }
```

- [ActionTargetTypeDef](./type_defs.md#actiontargettypedef)
- [AppTypeDef](./type_defs.md#apptypedef)
- [AssociateAdminAccountRequestRequestTypeDef](./type_defs.md#associateadminaccountrequestrequesttypedef)
- [AssociateThirdPartyFirewallRequestRequestTypeDef](./type_defs.md#associatethirdpartyfirewallrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AwsEc2NetworkInterfaceViolationTypeDef](./type_defs.md#awsec2networkinterfaceviolationtypedef)
- [PartialMatchTypeDef](./type_defs.md#partialmatchtypedef)
- [ComplianceViolatorTypeDef](./type_defs.md#complianceviolatortypedef)
- [DeleteAppsListRequestRequestTypeDef](./type_defs.md#deleteappslistrequestrequesttypedef)
- [DeletePolicyRequestRequestTypeDef](./type_defs.md#deletepolicyrequestrequesttypedef)
- [DeleteProtocolsListRequestRequestTypeDef](./type_defs.md#deleteprotocolslistrequestrequesttypedef)
- [DisassociateThirdPartyFirewallRequestRequestTypeDef](./type_defs.md#disassociatethirdpartyfirewallrequestrequesttypedef)
- [DnsDuplicateRuleGroupViolationTypeDef](./type_defs.md#dnsduplicaterulegroupviolationtypedef)
- [DnsRuleGroupLimitExceededViolationTypeDef](./type_defs.md#dnsrulegrouplimitexceededviolationtypedef)
- [DnsRuleGroupPriorityConflictViolationTypeDef](./type_defs.md#dnsrulegrouppriorityconflictviolationtypedef)
- [EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef)
- [ExpectedRouteTypeDef](./type_defs.md#expectedroutetypedef)
- [FMSPolicyUpdateFirewallCreationConfigActionTypeDef](./type_defs.md#fmspolicyupdatefirewallcreationconfigactiontypedef)
- [FirewallSubnetIsOutOfScopeViolationTypeDef](./type_defs.md#firewallsubnetisoutofscopeviolationtypedef)
- [FirewallSubnetMissingVPCEndpointViolationTypeDef](./type_defs.md#firewallsubnetmissingvpcendpointviolationtypedef)
- [GetAppsListRequestRequestTypeDef](./type_defs.md#getappslistrequestrequesttypedef)
- [GetComplianceDetailRequestRequestTypeDef](./type_defs.md#getcompliancedetailrequestrequesttypedef)
- [GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef)
- [GetProtectionStatusRequestRequestTypeDef](./type_defs.md#getprotectionstatusrequestrequesttypedef)
- [GetProtocolsListRequestRequestTypeDef](./type_defs.md#getprotocolslistrequestrequesttypedef)
- [ProtocolsListDataTypeDef](./type_defs.md#protocolslistdatatypedef)
- [GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef](./type_defs.md#getthirdpartyfirewallassociationstatusrequestrequesttypedef)
- [GetViolationDetailsRequestRequestTypeDef](./type_defs.md#getviolationdetailsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAppsListsRequestRequestTypeDef](./type_defs.md#listappslistsrequestrequesttypedef)
- [ListComplianceStatusRequestRequestTypeDef](./type_defs.md#listcompliancestatusrequestrequesttypedef)
- [ListMemberAccountsRequestRequestTypeDef](./type_defs.md#listmemberaccountsrequestrequesttypedef)
- [ListPoliciesRequestRequestTypeDef](./type_defs.md#listpoliciesrequestrequesttypedef)
- [PolicySummaryTypeDef](./type_defs.md#policysummarytypedef)
- [ListProtocolsListsRequestRequestTypeDef](./type_defs.md#listprotocolslistsrequestrequesttypedef)
- [ProtocolsListDataSummaryTypeDef](./type_defs.md#protocolslistdatasummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesrequestrequesttypedef)
- [ThirdPartyFirewallFirewallPolicyTypeDef](./type_defs.md#thirdpartyfirewallfirewallpolicytypedef)
- [RouteTypeDef](./type_defs.md#routetypedef)
- [NetworkFirewallMissingExpectedRTViolationTypeDef](./type_defs.md#networkfirewallmissingexpectedrtviolationtypedef)
- [NetworkFirewallMissingFirewallViolationTypeDef](./type_defs.md#networkfirewallmissingfirewallviolationtypedef)
- [NetworkFirewallMissingSubnetViolationTypeDef](./type_defs.md#networkfirewallmissingsubnetviolationtypedef)
- [StatefulRuleGroupTypeDef](./type_defs.md#statefulrulegrouptypedef)
- [StatelessRuleGroupTypeDef](./type_defs.md#statelessrulegrouptypedef)
- [NetworkFirewallPolicyTypeDef](./type_defs.md#networkfirewallpolicytypedef)
- [ThirdPartyFirewallPolicyTypeDef](./type_defs.md#thirdpartyfirewallpolicytypedef)
- [ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)
- [PutNotificationChannelRequestRequestTypeDef](./type_defs.md#putnotificationchannelrequestrequesttypedef)
- [ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef](./type_defs.md#thirdpartyfirewallmissingexpectedroutetableviolationtypedef)
- [ThirdPartyFirewallMissingFirewallViolationTypeDef](./type_defs.md#thirdpartyfirewallmissingfirewallviolationtypedef)
- [ThirdPartyFirewallMissingSubnetViolationTypeDef](./type_defs.md#thirdpartyfirewallmissingsubnetviolationtypedef)
- [SecurityGroupRuleDescriptionTypeDef](./type_defs.md#securitygroupruledescriptiontypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [EC2AssociateRouteTableActionTypeDef](./type_defs.md#ec2associateroutetableactiontypedef)
- [EC2CopyRouteTableActionTypeDef](./type_defs.md#ec2copyroutetableactiontypedef)
- [EC2CreateRouteActionTypeDef](./type_defs.md#ec2createrouteactiontypedef)
- [EC2CreateRouteTableActionTypeDef](./type_defs.md#ec2createroutetableactiontypedef)
- [EC2DeleteRouteActionTypeDef](./type_defs.md#ec2deleterouteactiontypedef)
- [EC2ReplaceRouteActionTypeDef](./type_defs.md#ec2replacerouteactiontypedef)
- [EC2ReplaceRouteTableAssociationActionTypeDef](./type_defs.md#ec2replaceroutetableassociationactiontypedef)
- [AppsListDataSummaryTypeDef](./type_defs.md#appslistdatasummarytypedef)
- [AppsListDataTypeDef](./type_defs.md#appslistdatatypedef)
- [AssociateThirdPartyFirewallResponseTypeDef](./type_defs.md#associatethirdpartyfirewallresponsetypedef)
- [DisassociateThirdPartyFirewallResponseTypeDef](./type_defs.md#disassociatethirdpartyfirewallresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAdminAccountResponseTypeDef](./type_defs.md#getadminaccountresponsetypedef)
- [GetNotificationChannelResponseTypeDef](./type_defs.md#getnotificationchannelresponsetypedef)
- [GetProtectionStatusResponseTypeDef](./type_defs.md#getprotectionstatusresponsetypedef)
- [GetThirdPartyFirewallAssociationStatusResponseTypeDef](./type_defs.md#getthirdpartyfirewallassociationstatusresponsetypedef)
- [ListMemberAccountsResponseTypeDef](./type_defs.md#listmemberaccountsresponsetypedef)
- [AwsEc2InstanceViolationTypeDef](./type_defs.md#awsec2instanceviolationtypedef)
- [PolicyComplianceDetailTypeDef](./type_defs.md#policycompliancedetailtypedef)
- [PolicyComplianceStatusTypeDef](./type_defs.md#policycompliancestatustypedef)
- [NetworkFirewallMissingExpectedRoutesViolationTypeDef](./type_defs.md#networkfirewallmissingexpectedroutesviolationtypedef)
- [GetProtocolsListResponseTypeDef](./type_defs.md#getprotocolslistresponsetypedef)
- [PutProtocolsListResponseTypeDef](./type_defs.md#putprotocolslistresponsetypedef)
- [ListAppsListsRequestListAppsListsPaginateTypeDef](./type_defs.md#listappslistsrequestlistappslistspaginatetypedef)
- [ListComplianceStatusRequestListComplianceStatusPaginateTypeDef](./type_defs.md#listcompliancestatusrequestlistcompliancestatuspaginatetypedef)
- [ListMemberAccountsRequestListMemberAccountsPaginateTypeDef](./type_defs.md#listmemberaccountsrequestlistmemberaccountspaginatetypedef)
- [ListPoliciesRequestListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesrequestlistpoliciespaginatetypedef)
- [ListProtocolsListsRequestListProtocolsListsPaginateTypeDef](./type_defs.md#listprotocolslistsrequestlistprotocolslistspaginatetypedef)
- [ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesrequestlistthirdpartyfirewallfirewallpoliciespaginatetypedef)
- [ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef)
- [ListProtocolsListsResponseTypeDef](./type_defs.md#listprotocolslistsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutProtocolsListRequestRequestTypeDef](./type_defs.md#putprotocolslistrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ListThirdPartyFirewallFirewallPoliciesResponseTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesresponsetypedef)
- [NetworkFirewallBlackHoleRouteDetectedViolationTypeDef](./type_defs.md#networkfirewallblackholeroutedetectedviolationtypedef)
- [NetworkFirewallInternetTrafficNotInspectedViolationTypeDef](./type_defs.md#networkfirewallinternettrafficnotinspectedviolationtypedef)
- [NetworkFirewallInvalidRouteConfigurationViolationTypeDef](./type_defs.md#networkfirewallinvalidrouteconfigurationviolationtypedef)
- [NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef](./type_defs.md#networkfirewallunexpectedfirewallroutesviolationtypedef)
- [NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef](./type_defs.md#networkfirewallunexpectedgatewayroutesviolationtypedef)
- [RouteHasOutOfScopeEndpointViolationTypeDef](./type_defs.md#routehasoutofscopeendpointviolationtypedef)
- [NetworkFirewallPolicyDescriptionTypeDef](./type_defs.md#networkfirewallpolicydescriptiontypedef)
- [PolicyOptionTypeDef](./type_defs.md#policyoptiontypedef)
- [SecurityGroupRemediationActionTypeDef](./type_defs.md#securitygroupremediationactiontypedef)
- [RemediationActionTypeDef](./type_defs.md#remediationactiontypedef)
- [ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef)
- [GetAppsListResponseTypeDef](./type_defs.md#getappslistresponsetypedef)
- [PutAppsListRequestRequestTypeDef](./type_defs.md#putappslistrequestrequesttypedef)
- [PutAppsListResponseTypeDef](./type_defs.md#putappslistresponsetypedef)
- [GetComplianceDetailResponseTypeDef](./type_defs.md#getcompliancedetailresponsetypedef)
- [ListComplianceStatusResponseTypeDef](./type_defs.md#listcompliancestatusresponsetypedef)
- [NetworkFirewallPolicyModifiedViolationTypeDef](./type_defs.md#networkfirewallpolicymodifiedviolationtypedef)
- [SecurityServicePolicyDataTypeDef](./type_defs.md#securityservicepolicydatatypedef)
- [AwsVPCSecurityGroupViolationTypeDef](./type_defs.md#awsvpcsecuritygroupviolationtypedef)
- [RemediationActionWithOrderTypeDef](./type_defs.md#remediationactionwithordertypedef)
- [PolicyTypeDef](./type_defs.md#policytypedef)
- [PossibleRemediationActionTypeDef](./type_defs.md#possibleremediationactiontypedef)
- [GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef)
- [PutPolicyRequestRequestTypeDef](./type_defs.md#putpolicyrequestrequesttypedef)
- [PutPolicyResponseTypeDef](./type_defs.md#putpolicyresponsetypedef)
- [PossibleRemediationActionsTypeDef](./type_defs.md#possibleremediationactionstypedef)
- [ResourceViolationTypeDef](./type_defs.md#resourceviolationtypedef)
- [ViolationDetailTypeDef](./type_defs.md#violationdetailtypedef)
- [GetViolationDetailsResponseTypeDef](./type_defs.md#getviolationdetailsresponsetypedef)

