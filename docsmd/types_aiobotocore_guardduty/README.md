# GuardDuty module

> [Index](../README.md) > GuardDuty


!!! note ""

    Auto-generated documentation for [GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
    type annotations stubs module [types-aiobotocore-guardduty](https://pypi.org/project/types-aiobotocore-guardduty/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `GuardDuty` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[guardduty]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[guardduty]'


# standalone installation
python -m pip install types-aiobotocore-guardduty
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-guardduty
```

## Usage

Code samples can be found in [Examples](./usage.md).

## GuardDutyClient

Type annotations and code completion for  `#!python session.client("guardduty")` as [GuardDutyClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_guardduty.client import GuardDutyClient


session = Session()
async with session.client("guardduty") as client:
    client: GuardDutyClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("guardduty").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_guardduty.paginator import DescribeMalwareScansPaginator

def get_describe_malware_scans_paginator() -> DescribeMalwareScansPaginator:
    return client.get_paginator("describe_malware_scans"))
```

- [DescribeMalwareScansPaginator](./paginators.md#describemalwarescanspaginator)
- [ListDetectorsPaginator](./paginators.md#listdetectorspaginator)
- [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
- [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
- [ListMembersPaginator](./paginators.md#listmemberspaginator)
- [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
- [ListThreatIntelSetsPaginator](./paginators.md#listthreatintelsetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_guardduty.literals import AdminStatusType

def get_value() -> AdminStatusType:
    return "DISABLE_IN_PROGRESS"
```

- [AdminStatusType](./literals.md#adminstatustype)
- [CriterionKeyType](./literals.md#criterionkeytype)
- [DataSourceStatusType](./literals.md#datasourcestatustype)
- [DataSourceType](./literals.md#datasourcetype)
- [DescribeMalwareScansPaginatorName](./literals.md#describemalwarescanspaginatorname)
- [DestinationTypeType](./literals.md#destinationtypetype)
- [DetectorStatusType](./literals.md#detectorstatustype)
- [EbsSnapshotPreservationType](./literals.md#ebssnapshotpreservationtype)
- [FeedbackType](./literals.md#feedbacktype)
- [FilterActionType](./literals.md#filteractiontype)
- [FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype)
- [FindingStatisticTypeType](./literals.md#findingstatistictypetype)
- [IpSetFormatType](./literals.md#ipsetformattype)
- [IpSetStatusType](./literals.md#ipsetstatustype)
- [ListDetectorsPaginatorName](./literals.md#listdetectorspaginatorname)
- [ListFiltersPaginatorName](./literals.md#listfilterspaginatorname)
- [ListFindingsPaginatorName](./literals.md#listfindingspaginatorname)
- [ListIPSetsPaginatorName](./literals.md#listipsetspaginatorname)
- [ListInvitationsPaginatorName](./literals.md#listinvitationspaginatorname)
- [ListMembersPaginatorName](./literals.md#listmemberspaginatorname)
- [ListOrganizationAdminAccountsPaginatorName](./literals.md#listorganizationadminaccountspaginatorname)
- [ListThreatIntelSetsPaginatorName](./literals.md#listthreatintelsetspaginatorname)
- [OrderByType](./literals.md#orderbytype)
- [PublishingStatusType](./literals.md#publishingstatustype)
- [ScanCriterionKeyType](./literals.md#scancriterionkeytype)
- [ScanResultType](./literals.md#scanresulttype)
- [ScanStatusType](./literals.md#scanstatustype)
- [ThreatIntelSetFormatType](./literals.md#threatintelsetformattype)
- [ThreatIntelSetStatusType](./literals.md#threatintelsetstatustype)
- [UsageStatisticTypeType](./literals.md#usagestatistictypetype)
- [GuardDutyServiceName](./literals.md#guarddutyservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef

def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
    return {
        "DetectorId": ...,
        "AdministratorId": ...,
        "InvitationId": ...,
    }
```

- [AcceptAdministratorInvitationRequestRequestTypeDef](./type_defs.md#acceptadministratorinvitationrequestrequesttypedef)
- [AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef)
- [AccessControlListTypeDef](./type_defs.md#accesscontrollisttypedef)
- [AccessKeyDetailsTypeDef](./type_defs.md#accesskeydetailstypedef)
- [AccountDetailTypeDef](./type_defs.md#accountdetailtypedef)
- [BlockPublicAccessTypeDef](./type_defs.md#blockpublicaccesstypedef)
- [DnsRequestActionTypeDef](./type_defs.md#dnsrequestactiontypedef)
- [AdminAccountTypeDef](./type_defs.md#adminaccounttypedef)
- [AdministratorTypeDef](./type_defs.md#administratortypedef)
- [ArchiveFindingsRequestRequestTypeDef](./type_defs.md#archivefindingsrequestrequesttypedef)
- [DomainDetailsTypeDef](./type_defs.md#domaindetailstypedef)
- [RemoteAccountDetailsTypeDef](./type_defs.md#remoteaccountdetailstypedef)
- [BucketPolicyTypeDef](./type_defs.md#bucketpolicytypedef)
- [CityTypeDef](./type_defs.md#citytypedef)
- [CloudTrailConfigurationResultTypeDef](./type_defs.md#cloudtrailconfigurationresulttypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [SecurityContextTypeDef](./type_defs.md#securitycontexttypedef)
- [VolumeMountTypeDef](./type_defs.md#volumemounttypedef)
- [CountryTypeDef](./type_defs.md#countrytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateIPSetRequestRequestTypeDef](./type_defs.md#createipsetrequestrequesttypedef)
- [UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef)
- [DestinationPropertiesTypeDef](./type_defs.md#destinationpropertiestypedef)
- [CreateSampleFindingsRequestRequestTypeDef](./type_defs.md#createsamplefindingsrequestrequesttypedef)
- [CreateThreatIntelSetRequestRequestTypeDef](./type_defs.md#createthreatintelsetrequestrequesttypedef)
- [DNSLogsConfigurationResultTypeDef](./type_defs.md#dnslogsconfigurationresulttypedef)
- [FlowLogsConfigurationResultTypeDef](./type_defs.md#flowlogsconfigurationresulttypedef)
- [S3LogsConfigurationResultTypeDef](./type_defs.md#s3logsconfigurationresulttypedef)
- [S3LogsConfigurationTypeDef](./type_defs.md#s3logsconfigurationtypedef)
- [DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef)
- [DeclineInvitationsRequestRequestTypeDef](./type_defs.md#declineinvitationsrequestrequesttypedef)
- [DefaultServerSideEncryptionTypeDef](./type_defs.md#defaultserversideencryptiontypedef)
- [DeleteDetectorRequestRequestTypeDef](./type_defs.md#deletedetectorrequestrequesttypedef)
- [DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef)
- [DeleteIPSetRequestRequestTypeDef](./type_defs.md#deleteipsetrequestrequesttypedef)
- [DeleteInvitationsRequestRequestTypeDef](./type_defs.md#deleteinvitationsrequestrequesttypedef)
- [DeleteMembersRequestRequestTypeDef](./type_defs.md#deletemembersrequestrequesttypedef)
- [DeletePublishingDestinationRequestRequestTypeDef](./type_defs.md#deletepublishingdestinationrequestrequesttypedef)
- [DeleteThreatIntelSetRequestRequestTypeDef](./type_defs.md#deletethreatintelsetrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- [DescribeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#describeorganizationconfigurationrequestrequesttypedef)
- [DescribePublishingDestinationRequestRequestTypeDef](./type_defs.md#describepublishingdestinationrequestrequesttypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [DisableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#disableorganizationadminaccountrequestrequesttypedef)
- [DisassociateFromAdministratorAccountRequestRequestTypeDef](./type_defs.md#disassociatefromadministratoraccountrequestrequesttypedef)
- [DisassociateFromMasterAccountRequestRequestTypeDef](./type_defs.md#disassociatefrommasteraccountrequestrequesttypedef)
- [DisassociateMembersRequestRequestTypeDef](./type_defs.md#disassociatemembersrequestrequesttypedef)
- [VolumeDetailTypeDef](./type_defs.md#volumedetailtypedef)
- [EbsVolumesResultTypeDef](./type_defs.md#ebsvolumesresulttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [EnableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#enableorganizationadminaccountrequestrequesttypedef)
- [ThreatIntelligenceDetailTypeDef](./type_defs.md#threatintelligencedetailtypedef)
- [FilterConditionTypeDef](./type_defs.md#filterconditiontypedef)
- [FindingStatisticsTypeDef](./type_defs.md#findingstatisticstypedef)
- [GeoLocationTypeDef](./type_defs.md#geolocationtypedef)
- [GetAdministratorAccountRequestRequestTypeDef](./type_defs.md#getadministratoraccountrequestrequesttypedef)
- [GetDetectorRequestRequestTypeDef](./type_defs.md#getdetectorrequestrequesttypedef)
- [GetFilterRequestRequestTypeDef](./type_defs.md#getfilterrequestrequesttypedef)
- [GetIPSetRequestRequestTypeDef](./type_defs.md#getipsetrequestrequesttypedef)
- [GetMalwareScanSettingsRequestRequestTypeDef](./type_defs.md#getmalwarescansettingsrequestrequesttypedef)
- [GetMasterAccountRequestRequestTypeDef](./type_defs.md#getmasteraccountrequestrequesttypedef)
- [MasterTypeDef](./type_defs.md#mastertypedef)
- [GetMemberDetectorsRequestRequestTypeDef](./type_defs.md#getmemberdetectorsrequestrequesttypedef)
- [GetMembersRequestRequestTypeDef](./type_defs.md#getmembersrequestrequesttypedef)
- [MemberTypeDef](./type_defs.md#membertypedef)
- [GetRemainingFreeTrialDaysRequestRequestTypeDef](./type_defs.md#getremainingfreetrialdaysrequestrequesttypedef)
- [GetThreatIntelSetRequestRequestTypeDef](./type_defs.md#getthreatintelsetrequestrequesttypedef)
- [UsageCriteriaTypeDef](./type_defs.md#usagecriteriatypedef)
- [HighestSeverityThreatDetailsTypeDef](./type_defs.md#highestseveritythreatdetailstypedef)
- [HostPathTypeDef](./type_defs.md#hostpathtypedef)
- [IamInstanceProfileTypeDef](./type_defs.md#iaminstanceprofiletypedef)
- [ProductCodeTypeDef](./type_defs.md#productcodetypedef)
- [InvitationTypeDef](./type_defs.md#invitationtypedef)
- [InviteMembersRequestRequestTypeDef](./type_defs.md#invitemembersrequestrequesttypedef)
- [KubernetesAuditLogsConfigurationResultTypeDef](./type_defs.md#kubernetesauditlogsconfigurationresulttypedef)
- [KubernetesAuditLogsConfigurationTypeDef](./type_defs.md#kubernetesauditlogsconfigurationtypedef)
- [KubernetesUserDetailsTypeDef](./type_defs.md#kubernetesuserdetailstypedef)
- [ListDetectorsRequestRequestTypeDef](./type_defs.md#listdetectorsrequestrequesttypedef)
- [ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef)
- [ListIPSetsRequestRequestTypeDef](./type_defs.md#listipsetsrequestrequesttypedef)
- [ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef)
- [ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef)
- [ListOrganizationAdminAccountsRequestRequestTypeDef](./type_defs.md#listorganizationadminaccountsrequestrequesttypedef)
- [ListPublishingDestinationsRequestRequestTypeDef](./type_defs.md#listpublishingdestinationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListThreatIntelSetsRequestRequestTypeDef](./type_defs.md#listthreatintelsetsrequestrequesttypedef)
- [LocalIpDetailsTypeDef](./type_defs.md#localipdetailstypedef)
- [LocalPortDetailsTypeDef](./type_defs.md#localportdetailstypedef)
- [ScanEc2InstanceWithFindingsTypeDef](./type_defs.md#scanec2instancewithfindingstypedef)
- [RemotePortDetailsTypeDef](./type_defs.md#remoteportdetailstypedef)
- [PrivateIpAddressDetailsTypeDef](./type_defs.md#privateipaddressdetailstypedef)
- [SecurityGroupTypeDef](./type_defs.md#securitygrouptypedef)
- [OrganizationS3LogsConfigurationResultTypeDef](./type_defs.md#organizations3logsconfigurationresulttypedef)
- [OrganizationS3LogsConfigurationTypeDef](./type_defs.md#organizations3logsconfigurationtypedef)
- [OrganizationEbsVolumesResultTypeDef](./type_defs.md#organizationebsvolumesresulttypedef)
- [OrganizationEbsVolumesTypeDef](./type_defs.md#organizationebsvolumestypedef)
- [OrganizationKubernetesAuditLogsConfigurationResultTypeDef](./type_defs.md#organizationkubernetesauditlogsconfigurationresulttypedef)
- [OrganizationKubernetesAuditLogsConfigurationTypeDef](./type_defs.md#organizationkubernetesauditlogsconfigurationtypedef)
- [OrganizationTypeDef](./type_defs.md#organizationtypedef)
- [OwnerTypeDef](./type_defs.md#ownertypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [ScanConditionPairTypeDef](./type_defs.md#scanconditionpairtypedef)
- [ScannedItemCountTypeDef](./type_defs.md#scanneditemcounttypedef)
- [ThreatsDetectedItemCountTypeDef](./type_defs.md#threatsdetecteditemcounttypedef)
- [ScanFilePathTypeDef](./type_defs.md#scanfilepathtypedef)
- [ScanResultDetailsTypeDef](./type_defs.md#scanresultdetailstypedef)
- [TriggerDetailsTypeDef](./type_defs.md#triggerdetailstypedef)
- [ServiceAdditionalInfoTypeDef](./type_defs.md#serviceadditionalinfotypedef)
- [StartMonitoringMembersRequestRequestTypeDef](./type_defs.md#startmonitoringmembersrequestrequesttypedef)
- [StopMonitoringMembersRequestRequestTypeDef](./type_defs.md#stopmonitoringmembersrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TotalTypeDef](./type_defs.md#totaltypedef)
- [UnarchiveFindingsRequestRequestTypeDef](./type_defs.md#unarchivefindingsrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFindingsFeedbackRequestRequestTypeDef](./type_defs.md#updatefindingsfeedbackrequestrequesttypedef)
- [UpdateIPSetRequestRequestTypeDef](./type_defs.md#updateipsetrequestrequesttypedef)
- [UpdateThreatIntelSetRequestRequestTypeDef](./type_defs.md#updatethreatintelsetrequestrequesttypedef)
- [CreateMembersRequestRequestTypeDef](./type_defs.md#createmembersrequestrequesttypedef)
- [AccountLevelPermissionsTypeDef](./type_defs.md#accountlevelpermissionstypedef)
- [BucketLevelPermissionsTypeDef](./type_defs.md#bucketlevelpermissionstypedef)
- [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef)
- [ContainerTypeDef](./type_defs.md#containertypedef)
- [CreateDetectorResponseTypeDef](./type_defs.md#createdetectorresponsetypedef)
- [CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef)
- [CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef)
- [CreatePublishingDestinationResponseTypeDef](./type_defs.md#createpublishingdestinationresponsetypedef)
- [CreateThreatIntelSetResponseTypeDef](./type_defs.md#createthreatintelsetresponsetypedef)
- [GetAdministratorAccountResponseTypeDef](./type_defs.md#getadministratoraccountresponsetypedef)
- [GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef)
- [GetInvitationsCountResponseTypeDef](./type_defs.md#getinvitationscountresponsetypedef)
- [GetThreatIntelSetResponseTypeDef](./type_defs.md#getthreatintelsetresponsetypedef)
- [ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef)
- [ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)
- [ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)
- [ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef)
- [ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListThreatIntelSetsResponseTypeDef](./type_defs.md#listthreatintelsetsresponsetypedef)
- [UpdateFilterResponseTypeDef](./type_defs.md#updatefilterresponsetypedef)
- [CreateMembersResponseTypeDef](./type_defs.md#createmembersresponsetypedef)
- [DeclineInvitationsResponseTypeDef](./type_defs.md#declineinvitationsresponsetypedef)
- [DeleteInvitationsResponseTypeDef](./type_defs.md#deleteinvitationsresponsetypedef)
- [DeleteMembersResponseTypeDef](./type_defs.md#deletemembersresponsetypedef)
- [DisassociateMembersResponseTypeDef](./type_defs.md#disassociatemembersresponsetypedef)
- [InviteMembersResponseTypeDef](./type_defs.md#invitemembersresponsetypedef)
- [StartMonitoringMembersResponseTypeDef](./type_defs.md#startmonitoringmembersresponsetypedef)
- [StopMonitoringMembersResponseTypeDef](./type_defs.md#stopmonitoringmembersresponsetypedef)
- [UpdateMemberDetectorsResponseTypeDef](./type_defs.md#updatememberdetectorsresponsetypedef)
- [CreatePublishingDestinationRequestRequestTypeDef](./type_defs.md#createpublishingdestinationrequestrequesttypedef)
- [DescribePublishingDestinationResponseTypeDef](./type_defs.md#describepublishingdestinationresponsetypedef)
- [UpdatePublishingDestinationRequestRequestTypeDef](./type_defs.md#updatepublishingdestinationrequestrequesttypedef)
- [KubernetesDataSourceFreeTrialTypeDef](./type_defs.md#kubernetesdatasourcefreetrialtypedef)
- [MalwareProtectionDataSourceFreeTrialTypeDef](./type_defs.md#malwareprotectiondatasourcefreetrialtypedef)
- [ListDetectorsRequestListDetectorsPaginateTypeDef](./type_defs.md#listdetectorsrequestlistdetectorspaginatetypedef)
- [ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef)
- [ListIPSetsRequestListIPSetsPaginateTypeDef](./type_defs.md#listipsetsrequestlistipsetspaginatetypedef)
- [ListInvitationsRequestListInvitationsPaginateTypeDef](./type_defs.md#listinvitationsrequestlistinvitationspaginatetypedef)
- [ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef)
- [ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef](./type_defs.md#listorganizationadminaccountsrequestlistorganizationadminaccountspaginatetypedef)
- [ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef](./type_defs.md#listthreatintelsetsrequestlistthreatintelsetspaginatetypedef)
- [GetFindingsRequestRequestTypeDef](./type_defs.md#getfindingsrequestrequesttypedef)
- [ListPublishingDestinationsResponseTypeDef](./type_defs.md#listpublishingdestinationsresponsetypedef)
- [EbsVolumeDetailsTypeDef](./type_defs.md#ebsvolumedetailstypedef)
- [ScanEc2InstanceWithFindingsResultTypeDef](./type_defs.md#scanec2instancewithfindingsresulttypedef)
- [EksClusterDetailsTypeDef](./type_defs.md#eksclusterdetailstypedef)
- [EvidenceTypeDef](./type_defs.md#evidencetypedef)
- [FilterCriterionTypeDef](./type_defs.md#filtercriteriontypedef)
- [GetFindingsStatisticsResponseTypeDef](./type_defs.md#getfindingsstatisticsresponsetypedef)
- [GetMasterAccountResponseTypeDef](./type_defs.md#getmasteraccountresponsetypedef)
- [GetMembersResponseTypeDef](./type_defs.md#getmembersresponsetypedef)
- [ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)
- [GetUsageStatisticsRequestRequestTypeDef](./type_defs.md#getusagestatisticsrequestrequesttypedef)
- [VolumeTypeDef](./type_defs.md#volumetypedef)
- [ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef)
- [KubernetesConfigurationResultTypeDef](./type_defs.md#kubernetesconfigurationresulttypedef)
- [KubernetesConfigurationTypeDef](./type_defs.md#kubernetesconfigurationtypedef)
- [MalwareProtectionConfigurationTypeDef](./type_defs.md#malwareprotectionconfigurationtypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [OrganizationScanEc2InstanceWithFindingsResultTypeDef](./type_defs.md#organizationscanec2instancewithfindingsresulttypedef)
- [OrganizationScanEc2InstanceWithFindingsTypeDef](./type_defs.md#organizationscanec2instancewithfindingstypedef)
- [OrganizationKubernetesConfigurationResultTypeDef](./type_defs.md#organizationkubernetesconfigurationresulttypedef)
- [OrganizationKubernetesConfigurationTypeDef](./type_defs.md#organizationkubernetesconfigurationtypedef)
- [RemoteIpDetailsTypeDef](./type_defs.md#remoteipdetailstypedef)
- [ScanConditionTypeDef](./type_defs.md#scanconditiontypedef)
- [ScanThreatNameTypeDef](./type_defs.md#scanthreatnametypedef)
- [ScanTypeDef](./type_defs.md#scantypedef)
- [UsageAccountResultTypeDef](./type_defs.md#usageaccountresulttypedef)
- [UsageDataSourceResultTypeDef](./type_defs.md#usagedatasourceresulttypedef)
- [UsageResourceResultTypeDef](./type_defs.md#usageresourceresulttypedef)
- [PermissionConfigurationTypeDef](./type_defs.md#permissionconfigurationtypedef)
- [CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef)
- [GetFilterResponseTypeDef](./type_defs.md#getfilterresponsetypedef)
- [GetFindingsStatisticsRequestRequestTypeDef](./type_defs.md#getfindingsstatisticsrequestrequesttypedef)
- [ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef)
- [ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef)
- [UpdateFilterRequestRequestTypeDef](./type_defs.md#updatefilterrequestrequesttypedef)
- [DataSourcesFreeTrialTypeDef](./type_defs.md#datasourcesfreetrialtypedef)
- [MalwareProtectionConfigurationResultTypeDef](./type_defs.md#malwareprotectionconfigurationresulttypedef)
- [FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
- [EcsTaskDetailsTypeDef](./type_defs.md#ecstaskdetailstypedef)
- [KubernetesWorkloadDetailsTypeDef](./type_defs.md#kubernetesworkloaddetailstypedef)
- [DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef)
- [InstanceDetailsTypeDef](./type_defs.md#instancedetailstypedef)
- [OrganizationMalwareProtectionConfigurationResultTypeDef](./type_defs.md#organizationmalwareprotectionconfigurationresulttypedef)
- [OrganizationMalwareProtectionConfigurationTypeDef](./type_defs.md#organizationmalwareprotectionconfigurationtypedef)
- [AwsApiCallActionTypeDef](./type_defs.md#awsapicallactiontypedef)
- [KubernetesApiCallActionTypeDef](./type_defs.md#kubernetesapicallactiontypedef)
- [NetworkConnectionActionTypeDef](./type_defs.md#networkconnectionactiontypedef)
- [PortProbeDetailTypeDef](./type_defs.md#portprobedetailtypedef)
- [ScanResourceCriteriaTypeDef](./type_defs.md#scanresourcecriteriatypedef)
- [ThreatDetectedByNameTypeDef](./type_defs.md#threatdetectedbynametypedef)
- [DescribeMalwareScansResponseTypeDef](./type_defs.md#describemalwarescansresponsetypedef)
- [UsageStatisticsTypeDef](./type_defs.md#usagestatisticstypedef)
- [PublicAccessTypeDef](./type_defs.md#publicaccesstypedef)
- [AccountFreeTrialInfoTypeDef](./type_defs.md#accountfreetrialinfotypedef)
- [DataSourceConfigurationsResultTypeDef](./type_defs.md#datasourceconfigurationsresulttypedef)
- [DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef](./type_defs.md#describemalwarescansrequestdescribemalwarescanspaginatetypedef)
- [DescribeMalwareScansRequestRequestTypeDef](./type_defs.md#describemalwarescansrequestrequesttypedef)
- [EcsClusterDetailsTypeDef](./type_defs.md#ecsclusterdetailstypedef)
- [KubernetesDetailsTypeDef](./type_defs.md#kubernetesdetailstypedef)
- [CreateDetectorRequestRequestTypeDef](./type_defs.md#createdetectorrequestrequesttypedef)
- [UpdateDetectorRequestRequestTypeDef](./type_defs.md#updatedetectorrequestrequesttypedef)
- [UpdateMemberDetectorsRequestRequestTypeDef](./type_defs.md#updatememberdetectorsrequestrequesttypedef)
- [OrganizationDataSourceConfigurationsResultTypeDef](./type_defs.md#organizationdatasourceconfigurationsresulttypedef)
- [OrganizationDataSourceConfigurationsTypeDef](./type_defs.md#organizationdatasourceconfigurationstypedef)
- [PortProbeActionTypeDef](./type_defs.md#portprobeactiontypedef)
- [GetMalwareScanSettingsResponseTypeDef](./type_defs.md#getmalwarescansettingsresponsetypedef)
- [UpdateMalwareScanSettingsRequestRequestTypeDef](./type_defs.md#updatemalwarescansettingsrequestrequesttypedef)
- [ScanDetectionsTypeDef](./type_defs.md#scandetectionstypedef)
- [GetUsageStatisticsResponseTypeDef](./type_defs.md#getusagestatisticsresponsetypedef)
- [S3BucketDetailTypeDef](./type_defs.md#s3bucketdetailtypedef)
- [GetRemainingFreeTrialDaysResponseTypeDef](./type_defs.md#getremainingfreetrialdaysresponsetypedef)
- [GetDetectorResponseTypeDef](./type_defs.md#getdetectorresponsetypedef)
- [MemberDataSourceConfigurationTypeDef](./type_defs.md#memberdatasourceconfigurationtypedef)
- [DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef)
- [UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [EbsVolumeScanDetailsTypeDef](./type_defs.md#ebsvolumescandetailstypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [GetMemberDetectorsResponseTypeDef](./type_defs.md#getmemberdetectorsresponsetypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef)

