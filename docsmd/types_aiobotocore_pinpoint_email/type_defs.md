# Type definitions

> [Index](../README.md) > [PinpointEmail](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#pinpointemail)
    type annotations stubs module [types-aiobotocore-pinpoint-email](https://pypi.org/project/types-aiobotocore-pinpoint-email/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## InboxPlacementTrackingOptionUnionTypeDef

```python
# InboxPlacementTrackingOptionUnionTypeDef definition

InboxPlacementTrackingOptionUnionTypeDef = Union[
    InboxPlacementTrackingOptionTypeDef,  # (1)
    InboxPlacementTrackingOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InboxPlacementTrackingOptionTypeDef](./type_defs.md#inboxplacementtrackingoptiontypedef) 
2. See [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 

## CloudWatchDestinationUnionTypeDef

```python
# CloudWatchDestinationUnionTypeDef definition

CloudWatchDestinationUnionTypeDef = Union[
    CloudWatchDestinationTypeDef,  # (1)
    CloudWatchDestinationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) 
2. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 

## DomainDeliverabilityTrackingOptionUnionTypeDef

```python
# DomainDeliverabilityTrackingOptionUnionTypeDef definition

DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
    DomainDeliverabilityTrackingOptionTypeDef,  # (1)
    DomainDeliverabilityTrackingOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) 
2. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 



## BlacklistEntryTypeDef

```python
# BlacklistEntryTypeDef definition

class BlacklistEntryTypeDef(TypedDict):
    RblName: NotRequired[str],
    ListingTime: NotRequired[datetime],
    Description: NotRequired[str],
```

## ContentTypeDef

```python
# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    Data: str,
    Charset: NotRequired[str],
```

## CloudWatchDimensionConfigurationTypeDef

```python
# CloudWatchDimensionConfigurationTypeDef definition

class CloudWatchDimensionConfigurationTypeDef(TypedDict):
    DimensionName: str,
    DimensionValueSource: DimensionValueSourceType,  # (1)
    DefaultDimensionValue: str,
```

1. See [:material-code-brackets: DimensionValueSourceType](./literals.md#dimensionvaluesourcetype) 
## DeliveryOptionsTypeDef

```python
# DeliveryOptionsTypeDef definition

class DeliveryOptionsTypeDef(TypedDict):
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    SendingPoolName: NotRequired[str],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## SendingOptionsTypeDef

```python
# SendingOptionsTypeDef definition

class SendingOptionsTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## TrackingOptionsTypeDef

```python
# TrackingOptionsTypeDef definition

class TrackingOptionsTypeDef(TypedDict):
    CustomRedirectDomain: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DkimAttributesTypeDef

```python
# DkimAttributesTypeDef definition

class DkimAttributesTypeDef(TypedDict):
    SigningEnabled: NotRequired[bool],
    Status: NotRequired[DkimStatusType],  # (1)
    Tokens: NotRequired[list[str]],
```

1. See [:material-code-brackets: DkimStatusType](./literals.md#dkimstatustype) 
## DomainIspPlacementTypeDef

```python
# DomainIspPlacementTypeDef definition

class DomainIspPlacementTypeDef(TypedDict):
    IspName: NotRequired[str],
    InboxRawCount: NotRequired[int],
    SpamRawCount: NotRequired[int],
    InboxPercentage: NotRequired[float],
    SpamPercentage: NotRequired[float],
```

## VolumeStatisticsTypeDef

```python
# VolumeStatisticsTypeDef definition

class VolumeStatisticsTypeDef(TypedDict):
    InboxRawCount: NotRequired[int],
    SpamRawCount: NotRequired[int],
    ProjectedInbox: NotRequired[int],
    ProjectedSpam: NotRequired[int],
```

## DedicatedIpTypeDef

```python
# DedicatedIpTypeDef definition

class DedicatedIpTypeDef(TypedDict):
    Ip: str,
    WarmupStatus: WarmupStatusType,  # (1)
    WarmupPercentage: int,
    PoolName: NotRequired[str],
```

1. See [:material-code-brackets: WarmupStatusType](./literals.md#warmupstatustype) 
## DeleteConfigurationSetEventDestinationRequestRequestTypeDef

```python
# DeleteConfigurationSetEventDestinationRequestRequestTypeDef definition

class DeleteConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
```

## DeleteConfigurationSetRequestRequestTypeDef

```python
# DeleteConfigurationSetRequestRequestTypeDef definition

class DeleteConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## DeleteDedicatedIpPoolRequestRequestTypeDef

```python
# DeleteDedicatedIpPoolRequestRequestTypeDef definition

class DeleteDedicatedIpPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
```

## DeleteEmailIdentityRequestRequestTypeDef

```python
# DeleteEmailIdentityRequestRequestTypeDef definition

class DeleteEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## DeliverabilityTestReportTypeDef

```python
# DeliverabilityTestReportTypeDef definition

class DeliverabilityTestReportTypeDef(TypedDict):
    ReportId: NotRequired[str],
    ReportName: NotRequired[str],
    Subject: NotRequired[str],
    FromEmailAddress: NotRequired[str],
    CreateDate: NotRequired[datetime],
    DeliverabilityTestStatus: NotRequired[DeliverabilityTestStatusType],  # (1)
```

1. See [:material-code-brackets: DeliverabilityTestStatusType](./literals.md#deliverabilityteststatustype) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    ToAddresses: NotRequired[Sequence[str]],
    CcAddresses: NotRequired[Sequence[str]],
    BccAddresses: NotRequired[Sequence[str]],
```

## DomainDeliverabilityCampaignTypeDef

```python
# DomainDeliverabilityCampaignTypeDef definition

class DomainDeliverabilityCampaignTypeDef(TypedDict):
    CampaignId: NotRequired[str],
    ImageUrl: NotRequired[str],
    Subject: NotRequired[str],
    FromAddress: NotRequired[str],
    SendingIps: NotRequired[list[str]],
    FirstSeenDateTime: NotRequired[datetime],
    LastSeenDateTime: NotRequired[datetime],
    InboxCount: NotRequired[int],
    SpamCount: NotRequired[int],
    ReadRate: NotRequired[float],
    DeleteRate: NotRequired[float],
    ReadDeleteRate: NotRequired[float],
    ProjectedVolume: NotRequired[int],
    Esps: NotRequired[list[str]],
```

## InboxPlacementTrackingOptionOutputTypeDef

```python
# InboxPlacementTrackingOptionOutputTypeDef definition

class InboxPlacementTrackingOptionOutputTypeDef(TypedDict):
    Global: NotRequired[bool],
    TrackedIsps: NotRequired[list[str]],
```

## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    TemplateArn: NotRequired[str],
    TemplateData: NotRequired[str],
```

## KinesisFirehoseDestinationTypeDef

```python
# KinesisFirehoseDestinationTypeDef definition

class KinesisFirehoseDestinationTypeDef(TypedDict):
    IamRoleArn: str,
    DeliveryStreamArn: str,
```

## PinpointDestinationTypeDef

```python
# PinpointDestinationTypeDef definition

class PinpointDestinationTypeDef(TypedDict):
    ApplicationArn: NotRequired[str],
```

## SnsDestinationTypeDef

```python
# SnsDestinationTypeDef definition

class SnsDestinationTypeDef(TypedDict):
    TopicArn: str,
```

## SendQuotaTypeDef

```python
# SendQuotaTypeDef definition

class SendQuotaTypeDef(TypedDict):
    Max24HourSend: NotRequired[float],
    MaxSendRate: NotRequired[float],
    SentLast24Hours: NotRequired[float],
```

## GetBlacklistReportsRequestRequestTypeDef

```python
# GetBlacklistReportsRequestRequestTypeDef definition

class GetBlacklistReportsRequestRequestTypeDef(TypedDict):
    BlacklistItemNames: Sequence[str],
```

## GetConfigurationSetEventDestinationsRequestRequestTypeDef

```python
# GetConfigurationSetEventDestinationsRequestRequestTypeDef definition

class GetConfigurationSetEventDestinationsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## GetConfigurationSetRequestRequestTypeDef

```python
# GetConfigurationSetRequestRequestTypeDef definition

class GetConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
```

## ReputationOptionsOutputTypeDef

```python
# ReputationOptionsOutputTypeDef definition

class ReputationOptionsOutputTypeDef(TypedDict):
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[datetime],
```

## GetDedicatedIpRequestRequestTypeDef

```python
# GetDedicatedIpRequestRequestTypeDef definition

class GetDedicatedIpRequestRequestTypeDef(TypedDict):
    Ip: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetDedicatedIpsRequestRequestTypeDef

```python
# GetDedicatedIpsRequestRequestTypeDef definition

class GetDedicatedIpsRequestRequestTypeDef(TypedDict):
    PoolName: NotRequired[str],
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## GetDeliverabilityTestReportRequestRequestTypeDef

```python
# GetDeliverabilityTestReportRequestRequestTypeDef definition

class GetDeliverabilityTestReportRequestRequestTypeDef(TypedDict):
    ReportId: str,
```

## PlacementStatisticsTypeDef

```python
# PlacementStatisticsTypeDef definition

class PlacementStatisticsTypeDef(TypedDict):
    InboxPercentage: NotRequired[float],
    SpamPercentage: NotRequired[float],
    MissingPercentage: NotRequired[float],
    SpfPercentage: NotRequired[float],
    DkimPercentage: NotRequired[float],
```

## GetDomainDeliverabilityCampaignRequestRequestTypeDef

```python
# GetDomainDeliverabilityCampaignRequestRequestTypeDef definition

class GetDomainDeliverabilityCampaignRequestRequestTypeDef(TypedDict):
    CampaignId: str,
```

## GetEmailIdentityRequestRequestTypeDef

```python
# GetEmailIdentityRequestRequestTypeDef definition

class GetEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
```

## MailFromAttributesTypeDef

```python
# MailFromAttributesTypeDef definition

class MailFromAttributesTypeDef(TypedDict):
    MailFromDomain: str,
    MailFromDomainStatus: MailFromDomainStatusType,  # (1)
    BehaviorOnMxFailure: BehaviorOnMxFailureType,  # (2)
```

1. See [:material-code-brackets: MailFromDomainStatusType](./literals.md#mailfromdomainstatustype) 
2. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 
## IdentityInfoTypeDef

```python
# IdentityInfoTypeDef definition

class IdentityInfoTypeDef(TypedDict):
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    IdentityName: NotRequired[str],
    SendingEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## InboxPlacementTrackingOptionTypeDef

```python
# InboxPlacementTrackingOptionTypeDef definition

class InboxPlacementTrackingOptionTypeDef(TypedDict):
    Global: NotRequired[bool],
    TrackedIsps: NotRequired[Sequence[str]],
```

## ListConfigurationSetsRequestRequestTypeDef

```python
# ListConfigurationSetsRequestRequestTypeDef definition

class ListConfigurationSetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListDedicatedIpPoolsRequestRequestTypeDef

```python
# ListDedicatedIpPoolsRequestRequestTypeDef definition

class ListDedicatedIpPoolsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListDeliverabilityTestReportsRequestRequestTypeDef

```python
# ListDeliverabilityTestReportsRequestRequestTypeDef definition

class ListDeliverabilityTestReportsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListEmailIdentitiesRequestRequestTypeDef

```python
# ListEmailIdentitiesRequestRequestTypeDef definition

class ListEmailIdentitiesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## MessageTagTypeDef

```python
# MessageTagTypeDef definition

class MessageTagTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef

```python
# PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef definition

class PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef(TypedDict):
    AutoWarmupEnabled: NotRequired[bool],
```

## PutAccountSendingAttributesRequestRequestTypeDef

```python
# PutAccountSendingAttributesRequestRequestTypeDef definition

class PutAccountSendingAttributesRequestRequestTypeDef(TypedDict):
    SendingEnabled: NotRequired[bool],
```

## PutConfigurationSetDeliveryOptionsRequestRequestTypeDef

```python
# PutConfigurationSetDeliveryOptionsRequestRequestTypeDef definition

class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TlsPolicy: NotRequired[TlsPolicyType],  # (1)
    SendingPoolName: NotRequired[str],
```

1. See [:material-code-brackets: TlsPolicyType](./literals.md#tlspolicytype) 
## PutConfigurationSetReputationOptionsRequestRequestTypeDef

```python
# PutConfigurationSetReputationOptionsRequestRequestTypeDef definition

class PutConfigurationSetReputationOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    ReputationMetricsEnabled: NotRequired[bool],
```

## PutConfigurationSetSendingOptionsRequestRequestTypeDef

```python
# PutConfigurationSetSendingOptionsRequestRequestTypeDef definition

class PutConfigurationSetSendingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    SendingEnabled: NotRequired[bool],
```

## PutConfigurationSetTrackingOptionsRequestRequestTypeDef

```python
# PutConfigurationSetTrackingOptionsRequestRequestTypeDef definition

class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    CustomRedirectDomain: NotRequired[str],
```

## PutDedicatedIpInPoolRequestRequestTypeDef

```python
# PutDedicatedIpInPoolRequestRequestTypeDef definition

class PutDedicatedIpInPoolRequestRequestTypeDef(TypedDict):
    Ip: str,
    DestinationPoolName: str,
```

## PutDedicatedIpWarmupAttributesRequestRequestTypeDef

```python
# PutDedicatedIpWarmupAttributesRequestRequestTypeDef definition

class PutDedicatedIpWarmupAttributesRequestRequestTypeDef(TypedDict):
    Ip: str,
    WarmupPercentage: int,
```

## PutEmailIdentityDkimAttributesRequestRequestTypeDef

```python
# PutEmailIdentityDkimAttributesRequestRequestTypeDef definition

class PutEmailIdentityDkimAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    SigningEnabled: NotRequired[bool],
```

## PutEmailIdentityFeedbackAttributesRequestRequestTypeDef

```python
# PutEmailIdentityFeedbackAttributesRequestRequestTypeDef definition

class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    EmailForwardingEnabled: NotRequired[bool],
```

## PutEmailIdentityMailFromAttributesRequestRequestTypeDef

```python
# PutEmailIdentityMailFromAttributesRequestRequestTypeDef definition

class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    MailFromDomain: NotRequired[str],
    BehaviorOnMxFailure: NotRequired[BehaviorOnMxFailureType],  # (1)
```

1. See [:material-code-brackets: BehaviorOnMxFailureType](./literals.md#behavioronmxfailuretype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## RawMessageTypeDef

```python
# RawMessageTypeDef definition

class RawMessageTypeDef(TypedDict):
    Data: BlobTypeDef,
```

## BodyTypeDef

```python
# BodyTypeDef definition

class BodyTypeDef(TypedDict):
    Text: NotRequired[ContentTypeDef],  # (1)
    Html: NotRequired[ContentTypeDef],  # (1)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
## CloudWatchDestinationOutputTypeDef

```python
# CloudWatchDestinationOutputTypeDef definition

class CloudWatchDestinationOutputTypeDef(TypedDict):
    DimensionConfigurations: list[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## CloudWatchDestinationTypeDef

```python
# CloudWatchDestinationTypeDef definition

class CloudWatchDestinationTypeDef(TypedDict):
    DimensionConfigurations: Sequence[CloudWatchDimensionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchDimensionConfigurationTypeDef](./type_defs.md#cloudwatchdimensionconfigurationtypedef) 
## CreateDedicatedIpPoolRequestRequestTypeDef

```python
# CreateDedicatedIpPoolRequestRequestTypeDef definition

class CreateDedicatedIpPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEmailIdentityRequestRequestTypeDef

```python
# CreateEmailIdentityRequestRequestTypeDef definition

class CreateEmailIdentityRequestRequestTypeDef(TypedDict):
    EmailIdentity: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDeliverabilityTestReportResponseTypeDef

```python
# CreateDeliverabilityTestReportResponseTypeDef definition

class CreateDeliverabilityTestReportResponseTypeDef(TypedDict):
    ReportId: str,
    DeliverabilityTestStatus: DeliverabilityTestStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeliverabilityTestStatusType](./literals.md#deliverabilityteststatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlacklistReportsResponseTypeDef

```python
# GetBlacklistReportsResponseTypeDef definition

class GetBlacklistReportsResponseTypeDef(TypedDict):
    BlacklistReport: dict[str, list[BlacklistEntryTypeDef]],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlacklistEntryTypeDef](./type_defs.md#blacklistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationSetsResponseTypeDef

```python
# ListConfigurationSetsResponseTypeDef definition

class ListConfigurationSetsResponseTypeDef(TypedDict):
    ConfigurationSets: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDedicatedIpPoolsResponseTypeDef

```python
# ListDedicatedIpPoolsResponseTypeDef definition

class ListDedicatedIpPoolsResponseTypeDef(TypedDict):
    DedicatedIpPools: list[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: list[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEmailResponseTypeDef

```python
# SendEmailResponseTypeDef definition

class SendEmailResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEmailIdentityResponseTypeDef

```python
# CreateEmailIdentityResponseTypeDef definition

class CreateEmailIdentityResponseTypeDef(TypedDict):
    IdentityType: IdentityTypeType,  # (1)
    VerifiedForSendingStatus: bool,
    DkimAttributes: DkimAttributesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: DkimAttributesTypeDef](./type_defs.md#dkimattributestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DailyVolumeTypeDef

```python
# DailyVolumeTypeDef definition

class DailyVolumeTypeDef(TypedDict):
    StartDate: NotRequired[datetime],
    VolumeStatistics: NotRequired[VolumeStatisticsTypeDef],  # (1)
    DomainIspPlacements: NotRequired[list[DomainIspPlacementTypeDef]],  # (2)
```

1. See [:material-code-braces: VolumeStatisticsTypeDef](./type_defs.md#volumestatisticstypedef) 
2. See [:material-code-braces: DomainIspPlacementTypeDef](./type_defs.md#domainispplacementtypedef) 
## OverallVolumeTypeDef

```python
# OverallVolumeTypeDef definition

class OverallVolumeTypeDef(TypedDict):
    VolumeStatistics: NotRequired[VolumeStatisticsTypeDef],  # (1)
    ReadRatePercent: NotRequired[float],
    DomainIspPlacements: NotRequired[list[DomainIspPlacementTypeDef]],  # (2)
```

1. See [:material-code-braces: VolumeStatisticsTypeDef](./type_defs.md#volumestatisticstypedef) 
2. See [:material-code-braces: DomainIspPlacementTypeDef](./type_defs.md#domainispplacementtypedef) 
## GetDedicatedIpResponseTypeDef

```python
# GetDedicatedIpResponseTypeDef definition

class GetDedicatedIpResponseTypeDef(TypedDict):
    DedicatedIp: DedicatedIpTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DedicatedIpTypeDef](./type_defs.md#dedicatediptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDedicatedIpsResponseTypeDef

```python
# GetDedicatedIpsResponseTypeDef definition

class GetDedicatedIpsResponseTypeDef(TypedDict):
    DedicatedIps: list[DedicatedIpTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DedicatedIpTypeDef](./type_defs.md#dedicatediptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeliverabilityTestReportsResponseTypeDef

```python
# ListDeliverabilityTestReportsResponseTypeDef definition

class ListDeliverabilityTestReportsResponseTypeDef(TypedDict):
    DeliverabilityTestReports: list[DeliverabilityTestReportTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeliverabilityTestReportTypeDef](./type_defs.md#deliverabilitytestreporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainDeliverabilityCampaignResponseTypeDef

```python
# GetDomainDeliverabilityCampaignResponseTypeDef definition

class GetDomainDeliverabilityCampaignResponseTypeDef(TypedDict):
    DomainDeliverabilityCampaign: DomainDeliverabilityCampaignTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDeliverabilityCampaignTypeDef](./type_defs.md#domaindeliverabilitycampaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainDeliverabilityCampaignsResponseTypeDef

```python
# ListDomainDeliverabilityCampaignsResponseTypeDef definition

class ListDomainDeliverabilityCampaignsResponseTypeDef(TypedDict):
    DomainDeliverabilityCampaigns: list[DomainDeliverabilityCampaignTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainDeliverabilityCampaignTypeDef](./type_defs.md#domaindeliverabilitycampaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainDeliverabilityTrackingOptionOutputTypeDef

```python
# DomainDeliverabilityTrackingOptionOutputTypeDef definition

class DomainDeliverabilityTrackingOptionOutputTypeDef(TypedDict):
    Domain: NotRequired[str],
    SubscriptionStartDate: NotRequired[datetime],
    InboxPlacementTrackingOption: NotRequired[InboxPlacementTrackingOptionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 
## GetDomainStatisticsReportRequestRequestTypeDef

```python
# GetDomainStatisticsReportRequestRequestTypeDef definition

class GetDomainStatisticsReportRequestRequestTypeDef(TypedDict):
    Domain: str,
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
```

## ListDomainDeliverabilityCampaignsRequestRequestTypeDef

```python
# ListDomainDeliverabilityCampaignsRequestRequestTypeDef definition

class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(TypedDict):
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
    SubscribedDomain: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ReputationOptionsTypeDef

```python
# ReputationOptionsTypeDef definition

class ReputationOptionsTypeDef(TypedDict):
    ReputationMetricsEnabled: NotRequired[bool],
    LastFreshStart: NotRequired[TimestampTypeDef],
```

## GetAccountResponseTypeDef

```python
# GetAccountResponseTypeDef definition

class GetAccountResponseTypeDef(TypedDict):
    SendQuota: SendQuotaTypeDef,  # (1)
    SendingEnabled: bool,
    DedicatedIpAutoWarmupEnabled: bool,
    EnforcementStatus: str,
    ProductionAccessEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SendQuotaTypeDef](./type_defs.md#sendquotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfigurationSetResponseTypeDef

```python
# GetConfigurationSetResponseTypeDef definition

class GetConfigurationSetResponseTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: TrackingOptionsTypeDef,  # (1)
    DeliveryOptions: DeliveryOptionsTypeDef,  # (2)
    ReputationOptions: ReputationOptionsOutputTypeDef,  # (3)
    SendingOptions: SendingOptionsTypeDef,  # (4)
    Tags: list[TagTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsOutputTypeDef](./type_defs.md#reputationoptionsoutputtypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDedicatedIpsRequestPaginateTypeDef

```python
# GetDedicatedIpsRequestPaginateTypeDef definition

class GetDedicatedIpsRequestPaginateTypeDef(TypedDict):
    PoolName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationSetsRequestPaginateTypeDef

```python
# ListConfigurationSetsRequestPaginateTypeDef definition

class ListConfigurationSetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDedicatedIpPoolsRequestPaginateTypeDef

```python
# ListDedicatedIpPoolsRequestPaginateTypeDef definition

class ListDedicatedIpPoolsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeliverabilityTestReportsRequestPaginateTypeDef

```python
# ListDeliverabilityTestReportsRequestPaginateTypeDef definition

class ListDeliverabilityTestReportsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEmailIdentitiesRequestPaginateTypeDef

```python
# ListEmailIdentitiesRequestPaginateTypeDef definition

class ListEmailIdentitiesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## IspPlacementTypeDef

```python
# IspPlacementTypeDef definition

class IspPlacementTypeDef(TypedDict):
    IspName: NotRequired[str],
    PlacementStatistics: NotRequired[PlacementStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: PlacementStatisticsTypeDef](./type_defs.md#placementstatisticstypedef) 
## GetEmailIdentityResponseTypeDef

```python
# GetEmailIdentityResponseTypeDef definition

class GetEmailIdentityResponseTypeDef(TypedDict):
    IdentityType: IdentityTypeType,  # (1)
    FeedbackForwardingStatus: bool,
    VerifiedForSendingStatus: bool,
    DkimAttributes: DkimAttributesTypeDef,  # (2)
    MailFromAttributes: MailFromAttributesTypeDef,  # (3)
    Tags: list[TagTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: DkimAttributesTypeDef](./type_defs.md#dkimattributestypedef) 
3. See [:material-code-braces: MailFromAttributesTypeDef](./type_defs.md#mailfromattributestypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEmailIdentitiesResponseTypeDef

```python
# ListEmailIdentitiesResponseTypeDef definition

class ListEmailIdentitiesResponseTypeDef(TypedDict):
    EmailIdentities: list[IdentityInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityInfoTypeDef](./type_defs.md#identityinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    Subject: ContentTypeDef,  # (1)
    Body: BodyTypeDef,  # (2)
```

1. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
2. See [:material-code-braces: BodyTypeDef](./type_defs.md#bodytypedef) 
## EventDestinationTypeDef

```python
# EventDestinationTypeDef definition

class EventDestinationTypeDef(TypedDict):
    Name: str,
    MatchingEventTypes: list[EventTypeType],  # (1)
    Enabled: NotRequired[bool],
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    CloudWatchDestination: NotRequired[CloudWatchDestinationOutputTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
    PinpointDestination: NotRequired[PinpointDestinationTypeDef],  # (5)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
5. See [:material-code-braces: PinpointDestinationTypeDef](./type_defs.md#pinpointdestinationtypedef) 
## GetDomainStatisticsReportResponseTypeDef

```python
# GetDomainStatisticsReportResponseTypeDef definition

class GetDomainStatisticsReportResponseTypeDef(TypedDict):
    OverallVolume: OverallVolumeTypeDef,  # (1)
    DailyVolumes: list[DailyVolumeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: OverallVolumeTypeDef](./type_defs.md#overallvolumetypedef) 
2. See [:material-code-braces: DailyVolumeTypeDef](./type_defs.md#dailyvolumetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeliverabilityDashboardOptionsResponseTypeDef

```python
# GetDeliverabilityDashboardOptionsResponseTypeDef definition

class GetDeliverabilityDashboardOptionsResponseTypeDef(TypedDict):
    DashboardEnabled: bool,
    SubscriptionExpiryDate: datetime,
    AccountStatus: DeliverabilityDashboardAccountStatusType,  # (1)
    ActiveSubscribedDomains: list[DomainDeliverabilityTrackingOptionOutputTypeDef],  # (2)
    PendingExpirationSubscribedDomains: list[DomainDeliverabilityTrackingOptionOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DeliverabilityDashboardAccountStatusType](./literals.md#deliverabilitydashboardaccountstatustype) 
2. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 
3. See [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationSetRequestRequestTypeDef

```python
# CreateConfigurationSetRequestRequestTypeDef definition

class CreateConfigurationSetRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    TrackingOptions: NotRequired[TrackingOptionsTypeDef],  # (1)
    DeliveryOptions: NotRequired[DeliveryOptionsTypeDef],  # (2)
    ReputationOptions: NotRequired[ReputationOptionsTypeDef],  # (3)
    SendingOptions: NotRequired[SendingOptionsTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: TrackingOptionsTypeDef](./type_defs.md#trackingoptionstypedef) 
2. See [:material-code-braces: DeliveryOptionsTypeDef](./type_defs.md#deliveryoptionstypedef) 
3. See [:material-code-braces: ReputationOptionsTypeDef](./type_defs.md#reputationoptionstypedef) 
4. See [:material-code-braces: SendingOptionsTypeDef](./type_defs.md#sendingoptionstypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetDeliverabilityTestReportResponseTypeDef

```python
# GetDeliverabilityTestReportResponseTypeDef definition

class GetDeliverabilityTestReportResponseTypeDef(TypedDict):
    DeliverabilityTestReport: DeliverabilityTestReportTypeDef,  # (1)
    OverallPlacement: PlacementStatisticsTypeDef,  # (2)
    IspPlacements: list[IspPlacementTypeDef],  # (3)
    Message: str,
    Tags: list[TagTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DeliverabilityTestReportTypeDef](./type_defs.md#deliverabilitytestreporttypedef) 
2. See [:material-code-braces: PlacementStatisticsTypeDef](./type_defs.md#placementstatisticstypedef) 
3. See [:material-code-braces: IspPlacementTypeDef](./type_defs.md#ispplacementtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainDeliverabilityTrackingOptionTypeDef

```python
# DomainDeliverabilityTrackingOptionTypeDef definition

class DomainDeliverabilityTrackingOptionTypeDef(TypedDict):
    Domain: NotRequired[str],
    SubscriptionStartDate: NotRequired[TimestampTypeDef],
    InboxPlacementTrackingOption: NotRequired[InboxPlacementTrackingOptionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InboxPlacementTrackingOptionTypeDef](./type_defs.md#inboxplacementtrackingoptiontypedef) [:material-code-braces: InboxPlacementTrackingOptionOutputTypeDef](./type_defs.md#inboxplacementtrackingoptionoutputtypedef) 
## EmailContentTypeDef

```python
# EmailContentTypeDef definition

class EmailContentTypeDef(TypedDict):
    Simple: NotRequired[MessageTypeDef],  # (1)
    Raw: NotRequired[RawMessageTypeDef],  # (2)
    Template: NotRequired[TemplateTypeDef],  # (3)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: RawMessageTypeDef](./type_defs.md#rawmessagetypedef) 
3. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## GetConfigurationSetEventDestinationsResponseTypeDef

```python
# GetConfigurationSetEventDestinationsResponseTypeDef definition

class GetConfigurationSetEventDestinationsResponseTypeDef(TypedDict):
    EventDestinations: list[EventDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDestinationTypeDef](./type_defs.md#eventdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventDestinationDefinitionTypeDef

```python
# EventDestinationDefinitionTypeDef definition

class EventDestinationDefinitionTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    MatchingEventTypes: NotRequired[Sequence[EventTypeType]],  # (1)
    KinesisFirehoseDestination: NotRequired[KinesisFirehoseDestinationTypeDef],  # (2)
    CloudWatchDestination: NotRequired[CloudWatchDestinationUnionTypeDef],  # (3)
    SnsDestination: NotRequired[SnsDestinationTypeDef],  # (4)
    PinpointDestination: NotRequired[PinpointDestinationTypeDef],  # (5)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
2. See [:material-code-braces: KinesisFirehoseDestinationTypeDef](./type_defs.md#kinesisfirehosedestinationtypedef) 
3. See [:material-code-braces: CloudWatchDestinationTypeDef](./type_defs.md#cloudwatchdestinationtypedef) [:material-code-braces: CloudWatchDestinationOutputTypeDef](./type_defs.md#cloudwatchdestinationoutputtypedef) 
4. See [:material-code-braces: SnsDestinationTypeDef](./type_defs.md#snsdestinationtypedef) 
5. See [:material-code-braces: PinpointDestinationTypeDef](./type_defs.md#pinpointdestinationtypedef) 
## CreateDeliverabilityTestReportRequestRequestTypeDef

```python
# CreateDeliverabilityTestReportRequestRequestTypeDef definition

class CreateDeliverabilityTestReportRequestRequestTypeDef(TypedDict):
    FromEmailAddress: str,
    Content: EmailContentTypeDef,  # (1)
    ReportName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SendEmailRequestRequestTypeDef

```python
# SendEmailRequestRequestTypeDef definition

class SendEmailRequestRequestTypeDef(TypedDict):
    Destination: DestinationTypeDef,  # (1)
    Content: EmailContentTypeDef,  # (2)
    FromEmailAddress: NotRequired[str],
    ReplyToAddresses: NotRequired[Sequence[str]],
    FeedbackForwardingEmailAddress: NotRequired[str],
    EmailTags: NotRequired[Sequence[MessageTagTypeDef]],  # (3)
    ConfigurationSetName: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: EmailContentTypeDef](./type_defs.md#emailcontenttypedef) 
3. See [:material-code-braces: MessageTagTypeDef](./type_defs.md#messagetagtypedef) 
## CreateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# CreateConfigurationSetEventDestinationRequestRequestTypeDef definition

class CreateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## UpdateConfigurationSetEventDestinationRequestRequestTypeDef

```python
# UpdateConfigurationSetEventDestinationRequestRequestTypeDef definition

class UpdateConfigurationSetEventDestinationRequestRequestTypeDef(TypedDict):
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 
## PutDeliverabilityDashboardOptionRequestRequestTypeDef

```python
# PutDeliverabilityDashboardOptionRequestRequestTypeDef definition

class PutDeliverabilityDashboardOptionRequestRequestTypeDef(TypedDict):
    DashboardEnabled: bool,
    SubscribedDomains: NotRequired[Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DomainDeliverabilityTrackingOptionTypeDef](./type_defs.md#domaindeliverabilitytrackingoptiontypedef) [:material-code-braces: DomainDeliverabilityTrackingOptionOutputTypeDef](./type_defs.md#domaindeliverabilitytrackingoptionoutputtypedef) 