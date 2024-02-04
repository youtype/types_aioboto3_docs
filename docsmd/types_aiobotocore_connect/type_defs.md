# Type definitions

> [Index](../README.md) > [Connect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
## ActivateEvaluationFormRequestRequestTypeDef

```python
# ActivateEvaluationFormRequestRequestTypeDef definition

class ActivateEvaluationFormRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DistributionTypeDef

```python
# DistributionTypeDef definition

class DistributionTypeDef(TypedDict):
    Region: str,
    Percentage: int,
```

## QueueReferenceTypeDef

```python
# QueueReferenceTypeDef definition

class QueueReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## AgentHierarchyGroupsTypeDef

```python
# AgentHierarchyGroupsTypeDef definition

class AgentHierarchyGroupsTypeDef(TypedDict):
    L1Ids: NotRequired[Sequence[str]],
    L2Ids: NotRequired[Sequence[str]],
    L3Ids: NotRequired[Sequence[str]],
    L4Ids: NotRequired[Sequence[str]],
    L5Ids: NotRequired[Sequence[str]],
```

## AgentInfoTypeDef

```python
# AgentInfoTypeDef definition

class AgentInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    ConnectedToAgentTimestamp: NotRequired[datetime],
    AgentPauseDurationInSeconds: NotRequired[int],
```

## AgentStatusReferenceTypeDef

```python
# AgentStatusReferenceTypeDef definition

class AgentStatusReferenceTypeDef(TypedDict):
    StatusStartTimestamp: NotRequired[datetime],
    StatusArn: NotRequired[str],
    StatusName: NotRequired[str],
```

## AgentStatusSummaryTypeDef

```python
# AgentStatusSummaryTypeDef definition

class AgentStatusSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[AgentStatusTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
## AgentStatusTypeDef

```python
# AgentStatusTypeDef definition

class AgentStatusTypeDef(TypedDict):
    AgentStatusARN: NotRequired[str],
    AgentStatusId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Type: NotRequired[AgentStatusTypeType],  # (1)
    DisplayOrder: NotRequired[int],
    State: NotRequired[AgentStatusStateType],  # (2)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
2. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
## ParticipantCapabilitiesTypeDef

```python
# ParticipantCapabilitiesTypeDef definition

class ParticipantCapabilitiesTypeDef(TypedDict):
    Video: NotRequired[VideoCapabilityType],  # (1)
```

1. See [:material-code-brackets: VideoCapabilityType](./literals.md#videocapabilitytype) 
## AnalyticsDataAssociationResultTypeDef

```python
# AnalyticsDataAssociationResultTypeDef definition

class AnalyticsDataAssociationResultTypeDef(TypedDict):
    DataSetId: NotRequired[str],
    TargetAccountId: NotRequired[str],
    ResourceShareId: NotRequired[str],
    ResourceShareArn: NotRequired[str],
```

## AnswerMachineDetectionConfigTypeDef

```python
# AnswerMachineDetectionConfigTypeDef definition

class AnswerMachineDetectionConfigTypeDef(TypedDict):
    EnableAnswerMachineDetection: NotRequired[bool],
    AwaitAnswerMachinePrompt: NotRequired[bool],
```

## ApplicationPaginatorTypeDef

```python
# ApplicationPaginatorTypeDef definition

class ApplicationPaginatorTypeDef(TypedDict):
    Namespace: NotRequired[str],
    ApplicationPermissions: NotRequired[List[str]],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Namespace: NotRequired[str],
    ApplicationPermissions: NotRequired[Sequence[str]],
```

## AssociateAnalyticsDataSetRequestRequestTypeDef

```python
# AssociateAnalyticsDataSetRequestRequestTypeDef definition

class AssociateAnalyticsDataSetRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetId: str,
    TargetAccountId: NotRequired[str],
```

## AssociateApprovedOriginRequestRequestTypeDef

```python
# AssociateApprovedOriginRequestRequestTypeDef definition

class AssociateApprovedOriginRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Origin: str,
```

## LexBotTypeDef

```python
# LexBotTypeDef definition

class LexBotTypeDef(TypedDict):
    Name: str,
    LexRegion: str,
```

## LexV2BotTypeDef

```python
# LexV2BotTypeDef definition

class LexV2BotTypeDef(TypedDict):
    AliasArn: NotRequired[str],
```

## AssociateDefaultVocabularyRequestRequestTypeDef

```python
# AssociateDefaultVocabularyRequestRequestTypeDef definition

class AssociateDefaultVocabularyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    VocabularyId: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## AssociateFlowRequestRequestTypeDef

```python
# AssociateFlowRequestRequestTypeDef definition

class AssociateFlowRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceId: str,
    FlowId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
## AssociateLambdaFunctionRequestRequestTypeDef

```python
# AssociateLambdaFunctionRequestRequestTypeDef definition

class AssociateLambdaFunctionRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    FunctionArn: str,
```

## AssociatePhoneNumberContactFlowRequestRequestTypeDef

```python
# AssociatePhoneNumberContactFlowRequestRequestTypeDef definition

class AssociatePhoneNumberContactFlowRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    InstanceId: str,
    ContactFlowId: str,
```

## AssociateQueueQuickConnectsRequestRequestTypeDef

```python
# AssociateQueueQuickConnectsRequestRequestTypeDef definition

class AssociateQueueQuickConnectsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    QuickConnectIds: Sequence[str],
```

## AssociateSecurityKeyRequestRequestTypeDef

```python
# AssociateSecurityKeyRequestRequestTypeDef definition

class AssociateSecurityKeyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Key: str,
```

## AssociateTrafficDistributionGroupUserRequestRequestTypeDef

```python
# AssociateTrafficDistributionGroupUserRequestRequestTypeDef definition

class AssociateTrafficDistributionGroupUserRequestRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    UserId: str,
    InstanceId: str,
```

## UserProficiencyTypeDef

```python
# UserProficiencyTypeDef definition

class UserProficiencyTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: str,
    Level: float,
```

## AttachmentReferenceTypeDef

```python
# AttachmentReferenceTypeDef definition

class AttachmentReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    Status: NotRequired[ReferenceStatusType],  # (1)
```

1. See [:material-code-brackets: ReferenceStatusType](./literals.md#referencestatustype) 
## AttendeeTypeDef

```python
# AttendeeTypeDef definition

class AttendeeTypeDef(TypedDict):
    AttendeeId: NotRequired[str],
    JoinToken: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    AttributeType: NotRequired[InstanceAttributeTypeType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
## AudioFeaturesTypeDef

```python
# AudioFeaturesTypeDef definition

class AudioFeaturesTypeDef(TypedDict):
    EchoReduction: NotRequired[MeetingFeatureStatusType],  # (1)
```

1. See [:material-code-brackets: MeetingFeatureStatusType](./literals.md#meetingfeaturestatustype) 
## AvailableNumberSummaryTypeDef

```python
# AvailableNumberSummaryTypeDef definition

class AvailableNumberSummaryTypeDef(TypedDict):
    PhoneNumber: NotRequired[str],
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (1)
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (2)
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## BatchAssociateAnalyticsDataSetRequestRequestTypeDef

```python
# BatchAssociateAnalyticsDataSetRequestRequestTypeDef definition

class BatchAssociateAnalyticsDataSetRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetIds: Sequence[str],
    TargetAccountId: NotRequired[str],
```

## ErrorResultTypeDef

```python
# ErrorResultTypeDef definition

class ErrorResultTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchDisassociateAnalyticsDataSetRequestRequestTypeDef

```python
# BatchDisassociateAnalyticsDataSetRequestRequestTypeDef definition

class BatchDisassociateAnalyticsDataSetRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetIds: Sequence[str],
    TargetAccountId: NotRequired[str],
```

## BatchGetFlowAssociationRequestRequestTypeDef

```python
# BatchGetFlowAssociationRequestRequestTypeDef definition

class BatchGetFlowAssociationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceIds: Sequence[str],
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
## FlowAssociationSummaryTypeDef

```python
# FlowAssociationSummaryTypeDef definition

class FlowAssociationSummaryTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    FlowId: NotRequired[str],
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
## FailedRequestTypeDef

```python
# FailedRequestTypeDef definition

class FailedRequestTypeDef(TypedDict):
    RequestIdentifier: NotRequired[str],
    FailureReasonCode: NotRequired[FailureReasonCodeType],  # (1)
    FailureReasonMessage: NotRequired[str],
```

1. See [:material-code-brackets: FailureReasonCodeType](./literals.md#failurereasoncodetype) 
## SuccessfulRequestTypeDef

```python
# SuccessfulRequestTypeDef definition

class SuccessfulRequestTypeDef(TypedDict):
    RequestIdentifier: NotRequired[str],
    ContactId: NotRequired[str],
```

## CampaignTypeDef

```python
# CampaignTypeDef definition

class CampaignTypeDef(TypedDict):
    CampaignId: NotRequired[str],
```

## ChatEventTypeDef

```python
# ChatEventTypeDef definition

class ChatEventTypeDef(TypedDict):
    Type: ChatEventTypeType,  # (1)
    ContentType: NotRequired[str],
    Content: NotRequired[str],
```

1. See [:material-code-brackets: ChatEventTypeType](./literals.md#chateventtypetype) 
## ChatMessageTypeDef

```python
# ChatMessageTypeDef definition

class ChatMessageTypeDef(TypedDict):
    ContentType: str,
    Content: str,
```

## ChatStreamingConfigurationTypeDef

```python
# ChatStreamingConfigurationTypeDef definition

class ChatStreamingConfigurationTypeDef(TypedDict):
    StreamingEndpointArn: str,
```

## ClaimPhoneNumberRequestRequestTypeDef

```python
# ClaimPhoneNumberRequestRequestTypeDef definition

class ClaimPhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumber: str,
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberDescription: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## PhoneNumberStatusTypeDef

```python
# PhoneNumberStatusTypeDef definition

class PhoneNumberStatusTypeDef(TypedDict):
    Status: NotRequired[PhoneNumberWorkflowStatusType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberWorkflowStatusType](./literals.md#phonenumberworkflowstatustype) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Type: NotRequired[EndpointTypeType],  # (1)
    Address: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## ContactFilterTypeDef

```python
# ContactFilterTypeDef definition

class ContactFilterTypeDef(TypedDict):
    ContactStates: NotRequired[Sequence[ContactStateType]],  # (1)
```

1. See [:material-code-brackets: ContactStateType](./literals.md#contactstatetype) 
## ContactFlowModuleSummaryTypeDef

```python
# ContactFlowModuleSummaryTypeDef definition

class ContactFlowModuleSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[ContactFlowModuleStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
## ContactFlowModuleTypeDef

```python
# ContactFlowModuleTypeDef definition

class ContactFlowModuleTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Content: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[ContactFlowModuleStateType],  # (1)
    Status: NotRequired[ContactFlowModuleStatusType],  # (2)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
2. See [:material-code-brackets: ContactFlowModuleStatusType](./literals.md#contactflowmodulestatustype) 
## ContactFlowSummaryTypeDef

```python
# ContactFlowSummaryTypeDef definition

class ContactFlowSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    ContactFlowType: NotRequired[ContactFlowTypeType],  # (1)
    ContactFlowState: NotRequired[ContactFlowStateType],  # (2)
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
## ContactFlowTypeDef

```python
# ContactFlowTypeDef definition

class ContactFlowTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ContactFlowTypeType],  # (1)
    State: NotRequired[ContactFlowStateType],  # (2)
    Description: NotRequired[str],
    Content: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
## ContactSearchSummaryAgentInfoTypeDef

```python
# ContactSearchSummaryAgentInfoTypeDef definition

class ContactSearchSummaryAgentInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    ConnectedToAgentTimestamp: NotRequired[datetime],
```

## ContactSearchSummaryQueueInfoTypeDef

```python
# ContactSearchSummaryQueueInfoTypeDef definition

class ContactSearchSummaryQueueInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    EnqueueTimestamp: NotRequired[datetime],
```

## QueueInfoTypeDef

```python
# QueueInfoTypeDef definition

class QueueInfoTypeDef(TypedDict):
    Id: NotRequired[str],
    EnqueueTimestamp: NotRequired[datetime],
```

## WisdomInfoTypeDef

```python
# WisdomInfoTypeDef definition

class WisdomInfoTypeDef(TypedDict):
    SessionArn: NotRequired[str],
```

## TagConditionTypeDef

```python
# TagConditionTypeDef definition

class TagConditionTypeDef(TypedDict):
    TagKey: NotRequired[str],
    TagValue: NotRequired[str],
```

## CreateAgentStatusRequestRequestTypeDef

```python
# CreateAgentStatusRequestRequestTypeDef definition

class CreateAgentStatusRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    State: AgentStatusStateType,  # (1)
    Description: NotRequired[str],
    DisplayOrder: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
## CreateContactFlowModuleRequestRequestTypeDef

```python
# CreateContactFlowModuleRequestRequestTypeDef definition

class CreateContactFlowModuleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Content: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## CreateContactFlowRequestRequestTypeDef

```python
# CreateContactFlowRequestRequestTypeDef definition

class CreateContactFlowRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Type: ContactFlowTypeType,  # (1)
    Content: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
## EvaluationFormScoringStrategyTypeDef

```python
# EvaluationFormScoringStrategyTypeDef definition

class EvaluationFormScoringStrategyTypeDef(TypedDict):
    Mode: EvaluationFormScoringModeType,  # (1)
    Status: EvaluationFormScoringStatusType,  # (2)
```

1. See [:material-code-brackets: EvaluationFormScoringModeType](./literals.md#evaluationformscoringmodetype) 
2. See [:material-code-brackets: EvaluationFormScoringStatusType](./literals.md#evaluationformscoringstatustype) 
## CreateInstanceRequestRequestTypeDef

```python
# CreateInstanceRequestRequestTypeDef definition

class CreateInstanceRequestRequestTypeDef(TypedDict):
    IdentityManagementType: DirectoryTypeType,  # (1)
    InboundCallsEnabled: bool,
    OutboundCallsEnabled: bool,
    ClientToken: NotRequired[str],
    InstanceAlias: NotRequired[str],
    DirectoryId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
## CreateIntegrationAssociationRequestRequestTypeDef

```python
# CreateIntegrationAssociationRequestRequestTypeDef definition

class CreateIntegrationAssociationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationType: IntegrationTypeType,  # (1)
    IntegrationArn: str,
    SourceApplicationUrl: NotRequired[str],
    SourceApplicationName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## ParticipantDetailsToAddTypeDef

```python
# ParticipantDetailsToAddTypeDef definition

class ParticipantDetailsToAddTypeDef(TypedDict):
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
## ParticipantTokenCredentialsTypeDef

```python
# ParticipantTokenCredentialsTypeDef definition

class ParticipantTokenCredentialsTypeDef(TypedDict):
    ParticipantToken: NotRequired[str],
    Expiry: NotRequired[str],
```

## CreatePersistentContactAssociationRequestRequestTypeDef

```python
# CreatePersistentContactAssociationRequestRequestTypeDef definition

class CreatePersistentContactAssociationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    InitialContactId: str,
    RehydrationType: RehydrationTypeType,  # (1)
    SourceContactId: str,
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: RehydrationTypeType](./literals.md#rehydrationtypetype) 
## PredefinedAttributeValuesTypeDef

```python
# PredefinedAttributeValuesTypeDef definition

class PredefinedAttributeValuesTypeDef(TypedDict):
    StringList: NotRequired[Sequence[str]],
```

## CreatePromptRequestRequestTypeDef

```python
# CreatePromptRequestRequestTypeDef definition

class CreatePromptRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    S3Uri: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## OutboundCallerConfigTypeDef

```python
# OutboundCallerConfigTypeDef definition

class OutboundCallerConfigTypeDef(TypedDict):
    OutboundCallerIdName: NotRequired[str],
    OutboundCallerIdNumberId: NotRequired[str],
    OutboundFlowId: NotRequired[str],
```

## RuleTriggerEventSourceTypeDef

```python
# RuleTriggerEventSourceTypeDef definition

class RuleTriggerEventSourceTypeDef(TypedDict):
    EventSourceName: EventSourceNameType,  # (1)
    IntegrationAssociationId: NotRequired[str],
```

1. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
## CreateTrafficDistributionGroupRequestRequestTypeDef

```python
# CreateTrafficDistributionGroupRequestRequestTypeDef definition

class CreateTrafficDistributionGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    InstanceId: str,
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateUseCaseRequestRequestTypeDef

```python
# CreateUseCaseRequestRequestTypeDef definition

class CreateUseCaseRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    UseCaseType: UseCaseTypeType,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: UseCaseTypeType](./literals.md#usecasetypetype) 
## CreateUserHierarchyGroupRequestRequestTypeDef

```python
# CreateUserHierarchyGroupRequestRequestTypeDef definition

class CreateUserHierarchyGroupRequestRequestTypeDef(TypedDict):
    Name: str,
    InstanceId: str,
    ParentGroupId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## UserIdentityInfoTypeDef

```python
# UserIdentityInfoTypeDef definition

class UserIdentityInfoTypeDef(TypedDict):
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    Email: NotRequired[str],
    SecondaryEmail: NotRequired[str],
    Mobile: NotRequired[str],
```

## UserPhoneConfigTypeDef

```python
# UserPhoneConfigTypeDef definition

class UserPhoneConfigTypeDef(TypedDict):
    PhoneType: PhoneTypeType,  # (1)
    AutoAccept: NotRequired[bool],
    AfterContactWorkTimeLimit: NotRequired[int],
    DeskPhoneNumber: NotRequired[str],
```

1. See [:material-code-brackets: PhoneTypeType](./literals.md#phonetypetype) 
## ViewInputContentTypeDef

```python
# ViewInputContentTypeDef definition

class ViewInputContentTypeDef(TypedDict):
    Template: NotRequired[str],
    Actions: NotRequired[Sequence[str]],
```

## CreateViewVersionRequestRequestTypeDef

```python
# CreateViewVersionRequestRequestTypeDef definition

class CreateViewVersionRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    VersionDescription: NotRequired[str],
    ViewContentSha256: NotRequired[str],
```

## CreateVocabularyRequestRequestTypeDef

```python
# CreateVocabularyRequestRequestTypeDef definition

class CreateVocabularyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    VocabularyName: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    Content: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    AccessToken: NotRequired[str],
    AccessTokenExpiration: NotRequired[datetime],
    RefreshToken: NotRequired[str],
    RefreshTokenExpiration: NotRequired[datetime],
```

## CrossChannelBehaviorTypeDef

```python
# CrossChannelBehaviorTypeDef definition

class CrossChannelBehaviorTypeDef(TypedDict):
    BehaviorType: BehaviorTypeType,  # (1)
```

1. See [:material-code-brackets: BehaviorTypeType](./literals.md#behaviortypetype) 
## CurrentMetricTypeDef

```python
# CurrentMetricTypeDef definition

class CurrentMetricTypeDef(TypedDict):
    Name: NotRequired[CurrentMetricNameType],  # (1)
    Unit: NotRequired[UnitType],  # (2)
```

1. See [:material-code-brackets: CurrentMetricNameType](./literals.md#currentmetricnametype) 
2. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## CurrentMetricSortCriteriaTypeDef

```python
# CurrentMetricSortCriteriaTypeDef definition

class CurrentMetricSortCriteriaTypeDef(TypedDict):
    SortByMetric: NotRequired[CurrentMetricNameType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: CurrentMetricNameType](./literals.md#currentmetricnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DateReferenceTypeDef

```python
# DateReferenceTypeDef definition

class DateReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## DeactivateEvaluationFormRequestRequestTypeDef

```python
# DeactivateEvaluationFormRequestRequestTypeDef definition

class DeactivateEvaluationFormRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
```

## DefaultVocabularyTypeDef

```python
# DefaultVocabularyTypeDef definition

class DefaultVocabularyTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    VocabularyId: str,
    VocabularyName: str,
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## DeleteContactEvaluationRequestRequestTypeDef

```python
# DeleteContactEvaluationRequestRequestTypeDef definition

class DeleteContactEvaluationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
```

## DeleteContactFlowModuleRequestRequestTypeDef

```python
# DeleteContactFlowModuleRequestRequestTypeDef definition

class DeleteContactFlowModuleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
```

## DeleteContactFlowRequestRequestTypeDef

```python
# DeleteContactFlowRequestRequestTypeDef definition

class DeleteContactFlowRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
```

## DeleteEvaluationFormRequestRequestTypeDef

```python
# DeleteEvaluationFormRequestRequestTypeDef definition

class DeleteEvaluationFormRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: NotRequired[int],
```

## DeleteHoursOfOperationRequestRequestTypeDef

```python
# DeleteHoursOfOperationRequestRequestTypeDef definition

class DeleteHoursOfOperationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
```

## DeleteInstanceRequestRequestTypeDef

```python
# DeleteInstanceRequestRequestTypeDef definition

class DeleteInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DeleteIntegrationAssociationRequestRequestTypeDef

```python
# DeleteIntegrationAssociationRequestRequestTypeDef definition

class DeleteIntegrationAssociationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
```

## DeletePredefinedAttributeRequestRequestTypeDef

```python
# DeletePredefinedAttributeRequestRequestTypeDef definition

class DeletePredefinedAttributeRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
```

## DeletePromptRequestRequestTypeDef

```python
# DeletePromptRequestRequestTypeDef definition

class DeletePromptRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
```

## DeleteQueueRequestRequestTypeDef

```python
# DeleteQueueRequestRequestTypeDef definition

class DeleteQueueRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
```

## DeleteQuickConnectRequestRequestTypeDef

```python
# DeleteQuickConnectRequestRequestTypeDef definition

class DeleteQuickConnectRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
```

## DeleteRoutingProfileRequestRequestTypeDef

```python
# DeleteRoutingProfileRequestRequestTypeDef definition

class DeleteRoutingProfileRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
```

## DeleteRuleRequestRequestTypeDef

```python
# DeleteRuleRequestRequestTypeDef definition

class DeleteRuleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RuleId: str,
```

## DeleteSecurityProfileRequestRequestTypeDef

```python
# DeleteSecurityProfileRequestRequestTypeDef definition

class DeleteSecurityProfileRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    SecurityProfileId: str,
```

## DeleteTaskTemplateRequestRequestTypeDef

```python
# DeleteTaskTemplateRequestRequestTypeDef definition

class DeleteTaskTemplateRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    TaskTemplateId: str,
```

## DeleteTrafficDistributionGroupRequestRequestTypeDef

```python
# DeleteTrafficDistributionGroupRequestRequestTypeDef definition

class DeleteTrafficDistributionGroupRequestRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
```

## DeleteUseCaseRequestRequestTypeDef

```python
# DeleteUseCaseRequestRequestTypeDef definition

class DeleteUseCaseRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    UseCaseId: str,
```

## DeleteUserHierarchyGroupRequestRequestTypeDef

```python
# DeleteUserHierarchyGroupRequestRequestTypeDef definition

class DeleteUserHierarchyGroupRequestRequestTypeDef(TypedDict):
    HierarchyGroupId: str,
    InstanceId: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
```

## DeleteViewRequestRequestTypeDef

```python
# DeleteViewRequestRequestTypeDef definition

class DeleteViewRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
```

## DeleteViewVersionRequestRequestTypeDef

```python
# DeleteViewVersionRequestRequestTypeDef definition

class DeleteViewVersionRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    ViewVersion: int,
```

## DeleteVocabularyRequestRequestTypeDef

```python
# DeleteVocabularyRequestRequestTypeDef definition

class DeleteVocabularyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    VocabularyId: str,
```

## DescribeAgentStatusRequestRequestTypeDef

```python
# DescribeAgentStatusRequestRequestTypeDef definition

class DescribeAgentStatusRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AgentStatusId: str,
```

## DescribeContactEvaluationRequestRequestTypeDef

```python
# DescribeContactEvaluationRequestRequestTypeDef definition

class DescribeContactEvaluationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
```

## DescribeContactFlowModuleRequestRequestTypeDef

```python
# DescribeContactFlowModuleRequestRequestTypeDef definition

class DescribeContactFlowModuleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
```

## DescribeContactFlowRequestRequestTypeDef

```python
# DescribeContactFlowRequestRequestTypeDef definition

class DescribeContactFlowRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
```

## DescribeContactRequestRequestTypeDef

```python
# DescribeContactRequestRequestTypeDef definition

class DescribeContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
```

## DescribeEvaluationFormRequestRequestTypeDef

```python
# DescribeEvaluationFormRequestRequestTypeDef definition

class DescribeEvaluationFormRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: NotRequired[int],
```

## DescribeHoursOfOperationRequestRequestTypeDef

```python
# DescribeHoursOfOperationRequestRequestTypeDef definition

class DescribeHoursOfOperationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
```

## DescribeInstanceAttributeRequestRequestTypeDef

```python
# DescribeInstanceAttributeRequestRequestTypeDef definition

class DescribeInstanceAttributeRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AttributeType: InstanceAttributeTypeType,  # (1)
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
## DescribeInstanceRequestRequestTypeDef

```python
# DescribeInstanceRequestRequestTypeDef definition

class DescribeInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DescribeInstanceStorageConfigRequestRequestTypeDef

```python
# DescribeInstanceStorageConfigRequestRequestTypeDef definition

class DescribeInstanceStorageConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
## DescribePhoneNumberRequestRequestTypeDef

```python
# DescribePhoneNumberRequestRequestTypeDef definition

class DescribePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
```

## DescribePredefinedAttributeRequestRequestTypeDef

```python
# DescribePredefinedAttributeRequestRequestTypeDef definition

class DescribePredefinedAttributeRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
```

## DescribePromptRequestRequestTypeDef

```python
# DescribePromptRequestRequestTypeDef definition

class DescribePromptRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
```

## PromptTypeDef

```python
# PromptTypeDef definition

class PromptTypeDef(TypedDict):
    PromptARN: NotRequired[str],
    PromptId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## DescribeQueueRequestRequestTypeDef

```python
# DescribeQueueRequestRequestTypeDef definition

class DescribeQueueRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
```

## DescribeQuickConnectRequestRequestTypeDef

```python
# DescribeQuickConnectRequestRequestTypeDef definition

class DescribeQuickConnectRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
```

## DescribeRoutingProfileRequestRequestTypeDef

```python
# DescribeRoutingProfileRequestRequestTypeDef definition

class DescribeRoutingProfileRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
```

## DescribeRuleRequestRequestTypeDef

```python
# DescribeRuleRequestRequestTypeDef definition

class DescribeRuleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RuleId: str,
```

## DescribeSecurityProfileRequestRequestTypeDef

```python
# DescribeSecurityProfileRequestRequestTypeDef definition

class DescribeSecurityProfileRequestRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
```

## SecurityProfileTypeDef

```python
# SecurityProfileTypeDef definition

class SecurityProfileTypeDef(TypedDict):
    Id: NotRequired[str],
    OrganizationResourceId: NotRequired[str],
    Arn: NotRequired[str],
    SecurityProfileName: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    AllowedAccessControlTags: NotRequired[Dict[str, str]],
    TagRestrictedResources: NotRequired[List[str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## DescribeTrafficDistributionGroupRequestRequestTypeDef

```python
# DescribeTrafficDistributionGroupRequestRequestTypeDef definition

class DescribeTrafficDistributionGroupRequestRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
```

## TrafficDistributionGroupTypeDef

```python
# TrafficDistributionGroupTypeDef definition

class TrafficDistributionGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    InstanceArn: NotRequired[str],
    Status: NotRequired[TrafficDistributionGroupStatusType],  # (1)
    Tags: NotRequired[Dict[str, str]],
    IsDefault: NotRequired[bool],
```

1. See [:material-code-brackets: TrafficDistributionGroupStatusType](./literals.md#trafficdistributiongroupstatustype) 
## DescribeUserHierarchyGroupRequestRequestTypeDef

```python
# DescribeUserHierarchyGroupRequestRequestTypeDef definition

class DescribeUserHierarchyGroupRequestRequestTypeDef(TypedDict):
    HierarchyGroupId: str,
    InstanceId: str,
```

## DescribeUserHierarchyStructureRequestRequestTypeDef

```python
# DescribeUserHierarchyStructureRequestRequestTypeDef definition

class DescribeUserHierarchyStructureRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DescribeUserRequestRequestTypeDef

```python
# DescribeUserRequestRequestTypeDef definition

class DescribeUserRequestRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
```

## DescribeViewRequestRequestTypeDef

```python
# DescribeViewRequestRequestTypeDef definition

class DescribeViewRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
```

## DescribeVocabularyRequestRequestTypeDef

```python
# DescribeVocabularyRequestRequestTypeDef definition

class DescribeVocabularyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    VocabularyId: str,
```

## VocabularyTypeDef

```python
# VocabularyTypeDef definition

class VocabularyTypeDef(TypedDict):
    Name: str,
    Id: str,
    Arn: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    State: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: NotRequired[str],
    Content: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## RoutingProfileReferenceTypeDef

```python
# RoutingProfileReferenceTypeDef definition

class RoutingProfileReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## DisassociateAnalyticsDataSetRequestRequestTypeDef

```python
# DisassociateAnalyticsDataSetRequestRequestTypeDef definition

class DisassociateAnalyticsDataSetRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetId: str,
    TargetAccountId: NotRequired[str],
```

## DisassociateApprovedOriginRequestRequestTypeDef

```python
# DisassociateApprovedOriginRequestRequestTypeDef definition

class DisassociateApprovedOriginRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Origin: str,
```

## DisassociateFlowRequestRequestTypeDef

```python
# DisassociateFlowRequestRequestTypeDef definition

class DisassociateFlowRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
## DisassociateInstanceStorageConfigRequestRequestTypeDef

```python
# DisassociateInstanceStorageConfigRequestRequestTypeDef definition

class DisassociateInstanceStorageConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
## DisassociateLambdaFunctionRequestRequestTypeDef

```python
# DisassociateLambdaFunctionRequestRequestTypeDef definition

class DisassociateLambdaFunctionRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    FunctionArn: str,
```

## DisassociateLexBotRequestRequestTypeDef

```python
# DisassociateLexBotRequestRequestTypeDef definition

class DisassociateLexBotRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    BotName: str,
    LexRegion: str,
```

## DisassociatePhoneNumberContactFlowRequestRequestTypeDef

```python
# DisassociatePhoneNumberContactFlowRequestRequestTypeDef definition

class DisassociatePhoneNumberContactFlowRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    InstanceId: str,
```

## DisassociateQueueQuickConnectsRequestRequestTypeDef

```python
# DisassociateQueueQuickConnectsRequestRequestTypeDef definition

class DisassociateQueueQuickConnectsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    QuickConnectIds: Sequence[str],
```

## RoutingProfileQueueReferenceTypeDef

```python
# RoutingProfileQueueReferenceTypeDef definition

class RoutingProfileQueueReferenceTypeDef(TypedDict):
    QueueId: str,
    Channel: ChannelType,  # (1)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## DisassociateSecurityKeyRequestRequestTypeDef

```python
# DisassociateSecurityKeyRequestRequestTypeDef definition

class DisassociateSecurityKeyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
```

## DisassociateTrafficDistributionGroupUserRequestRequestTypeDef

```python
# DisassociateTrafficDistributionGroupUserRequestRequestTypeDef definition

class DisassociateTrafficDistributionGroupUserRequestRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    UserId: str,
    InstanceId: str,
```

## UserProficiencyDisassociateTypeDef

```python
# UserProficiencyDisassociateTypeDef definition

class UserProficiencyDisassociateTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: str,
```

## DisconnectReasonTypeDef

```python
# DisconnectReasonTypeDef definition

class DisconnectReasonTypeDef(TypedDict):
    Code: NotRequired[str],
```

## DismissUserContactRequestRequestTypeDef

```python
# DismissUserContactRequestRequestTypeDef definition

class DismissUserContactRequestRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
    ContactId: str,
```

## EmailReferenceTypeDef

```python
# EmailReferenceTypeDef definition

class EmailReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    EncryptionType: EncryptionTypeType,  # (1)
    KeyId: str,
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## EvaluationAnswerDataTypeDef

```python
# EvaluationAnswerDataTypeDef definition

class EvaluationAnswerDataTypeDef(TypedDict):
    StringValue: NotRequired[str],
    NumericValue: NotRequired[float],
    NotApplicable: NotRequired[bool],
```

## NumericQuestionPropertyValueAutomationTypeDef

```python
# NumericQuestionPropertyValueAutomationTypeDef definition

class NumericQuestionPropertyValueAutomationTypeDef(TypedDict):
    Label: NumericQuestionPropertyAutomationLabelType,  # (1)
```

1. See [:material-code-brackets: NumericQuestionPropertyAutomationLabelType](./literals.md#numericquestionpropertyautomationlabeltype) 
## EvaluationFormNumericQuestionOptionTypeDef

```python
# EvaluationFormNumericQuestionOptionTypeDef definition

class EvaluationFormNumericQuestionOptionTypeDef(TypedDict):
    MinValue: int,
    MaxValue: int,
    Score: NotRequired[int],
    AutomaticFail: NotRequired[bool],
```

## EvaluationFormSectionTypeDef

```python
# EvaluationFormSectionTypeDef definition

class EvaluationFormSectionTypeDef(TypedDict):
    Title: str,
    RefId: str,
    Items: Sequence[EvaluationFormItemTypeDef],  # (1)
    Instructions: NotRequired[str],
    Weight: NotRequired[float],
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
## SingleSelectQuestionRuleCategoryAutomationTypeDef

```python
# SingleSelectQuestionRuleCategoryAutomationTypeDef definition

class SingleSelectQuestionRuleCategoryAutomationTypeDef(TypedDict):
    Category: str,
    Condition: SingleSelectQuestionRuleCategoryAutomationConditionType,  # (1)
    OptionRefId: str,
```

1. See [:material-code-brackets: SingleSelectQuestionRuleCategoryAutomationConditionType](./literals.md#singleselectquestionrulecategoryautomationconditiontype) 
## EvaluationFormSingleSelectQuestionOptionTypeDef

```python
# EvaluationFormSingleSelectQuestionOptionTypeDef definition

class EvaluationFormSingleSelectQuestionOptionTypeDef(TypedDict):
    RefId: str,
    Text: str,
    Score: NotRequired[int],
    AutomaticFail: NotRequired[bool],
```

## EvaluationFormSummaryTypeDef

```python
# EvaluationFormSummaryTypeDef definition

class EvaluationFormSummaryTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    Title: str,
    CreatedTime: datetime,
    CreatedBy: str,
    LastModifiedTime: datetime,
    LastModifiedBy: str,
    LatestVersion: int,
    LastActivatedTime: NotRequired[datetime],
    LastActivatedBy: NotRequired[str],
    ActiveVersion: NotRequired[int],
```

## EvaluationFormVersionSummaryTypeDef

```python
# EvaluationFormVersionSummaryTypeDef definition

class EvaluationFormVersionSummaryTypeDef(TypedDict):
    EvaluationFormArn: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Locked: bool,
    Status: EvaluationFormVersionStatusType,  # (1)
    CreatedTime: datetime,
    CreatedBy: str,
    LastModifiedTime: datetime,
    LastModifiedBy: str,
```

1. See [:material-code-brackets: EvaluationFormVersionStatusType](./literals.md#evaluationformversionstatustype) 
## EvaluationScoreTypeDef

```python
# EvaluationScoreTypeDef definition

class EvaluationScoreTypeDef(TypedDict):
    Percentage: NotRequired[float],
    NotApplicable: NotRequired[bool],
    AutomaticFail: NotRequired[bool],
```

## EvaluationNoteTypeDef

```python
# EvaluationNoteTypeDef definition

class EvaluationNoteTypeDef(TypedDict):
    Value: NotRequired[str],
```

## EventBridgeActionDefinitionTypeDef

```python
# EventBridgeActionDefinitionTypeDef definition

class EventBridgeActionDefinitionTypeDef(TypedDict):
    Name: str,
```

## FieldValueUnionTypeDef

```python
# FieldValueUnionTypeDef definition

class FieldValueUnionTypeDef(TypedDict):
    BooleanValue: NotRequired[bool],
    DoubleValue: NotRequired[float],
    EmptyValue: NotRequired[Mapping[str, Any]],
    StringValue: NotRequired[str],
```

## FilterV2TypeDef

```python
# FilterV2TypeDef definition

class FilterV2TypeDef(TypedDict):
    FilterKey: NotRequired[str],
    FilterValues: NotRequired[Sequence[str]],
```

## FiltersTypeDef

```python
# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    Queues: NotRequired[Sequence[str]],
    Channels: NotRequired[Sequence[ChannelType]],  # (1)
    RoutingProfiles: NotRequired[Sequence[str]],
    RoutingStepExpressions: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## GetContactAttributesRequestRequestTypeDef

```python
# GetContactAttributesRequestRequestTypeDef definition

class GetContactAttributesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    InitialContactId: str,
```

## GetFederationTokenRequestRequestTypeDef

```python
# GetFederationTokenRequestRequestTypeDef definition

class GetFederationTokenRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## GetFlowAssociationRequestRequestTypeDef

```python
# GetFlowAssociationRequestRequestTypeDef definition

class GetFlowAssociationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## IntervalDetailsTypeDef

```python
# IntervalDetailsTypeDef definition

class IntervalDetailsTypeDef(TypedDict):
    TimeZone: NotRequired[str],
    IntervalPeriod: NotRequired[IntervalPeriodType],  # (1)
```

1. See [:material-code-brackets: IntervalPeriodType](./literals.md#intervalperiodtype) 
## GetPromptFileRequestRequestTypeDef

```python
# GetPromptFileRequestRequestTypeDef definition

class GetPromptFileRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
```

## GetTaskTemplateRequestRequestTypeDef

```python
# GetTaskTemplateRequestRequestTypeDef definition

class GetTaskTemplateRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    TaskTemplateId: str,
    SnapshotVersion: NotRequired[str],
```

## GetTrafficDistributionRequestRequestTypeDef

```python
# GetTrafficDistributionRequestRequestTypeDef definition

class GetTrafficDistributionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## HierarchyGroupConditionTypeDef

```python
# HierarchyGroupConditionTypeDef definition

class HierarchyGroupConditionTypeDef(TypedDict):
    Value: NotRequired[str],
    HierarchyGroupMatchType: NotRequired[HierarchyGroupMatchTypeType],  # (1)
```

1. See [:material-code-brackets: HierarchyGroupMatchTypeType](./literals.md#hierarchygroupmatchtypetype) 
## HierarchyGroupSummaryReferenceTypeDef

```python
# HierarchyGroupSummaryReferenceTypeDef definition

class HierarchyGroupSummaryReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## HierarchyGroupSummaryTypeDef

```python
# HierarchyGroupSummaryTypeDef definition

class HierarchyGroupSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## HierarchyLevelTypeDef

```python
# HierarchyLevelTypeDef definition

class HierarchyLevelTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## HierarchyLevelUpdateTypeDef

```python
# HierarchyLevelUpdateTypeDef definition

class HierarchyLevelUpdateTypeDef(TypedDict):
    Name: str,
```

## ThresholdTypeDef

```python
# ThresholdTypeDef definition

class ThresholdTypeDef(TypedDict):
    Comparison: NotRequired[ComparisonType],  # (1)
    ThresholdValue: NotRequired[float],
```

1. See [:material-code-brackets: ComparisonType](./literals.md#comparisontype) 
## HoursOfOperationTimeSliceTypeDef

```python
# HoursOfOperationTimeSliceTypeDef definition

class HoursOfOperationTimeSliceTypeDef(TypedDict):
    Hours: int,
    Minutes: int,
```

## StringConditionTypeDef

```python
# StringConditionTypeDef definition

class StringConditionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    Value: NotRequired[str],
    ComparisonType: NotRequired[StringComparisonTypeType],  # (1)
```

1. See [:material-code-brackets: StringComparisonTypeType](./literals.md#stringcomparisontypetype) 
## HoursOfOperationSummaryTypeDef

```python
# HoursOfOperationSummaryTypeDef definition

class HoursOfOperationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ImportPhoneNumberRequestRequestTypeDef

```python
# ImportPhoneNumberRequestRequestTypeDef definition

class ImportPhoneNumberRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    SourcePhoneNumberArn: str,
    PhoneNumberDescription: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
```

## InstanceStatusReasonTypeDef

```python
# InstanceStatusReasonTypeDef definition

class InstanceStatusReasonTypeDef(TypedDict):
    Message: NotRequired[str],
```

## KinesisFirehoseConfigTypeDef

```python
# KinesisFirehoseConfigTypeDef definition

class KinesisFirehoseConfigTypeDef(TypedDict):
    FirehoseArn: str,
```

## KinesisStreamConfigTypeDef

```python
# KinesisStreamConfigTypeDef definition

class KinesisStreamConfigTypeDef(TypedDict):
    StreamArn: str,
```

## InstanceSummaryTypeDef

```python
# InstanceSummaryTypeDef definition

class InstanceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    IdentityManagementType: NotRequired[DirectoryTypeType],  # (1)
    InstanceAlias: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    ServiceRole: NotRequired[str],
    InstanceStatus: NotRequired[InstanceStatusType],  # (2)
    InboundCallsEnabled: NotRequired[bool],
    OutboundCallsEnabled: NotRequired[bool],
    InstanceAccessUrl: NotRequired[str],
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
2. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
## IntegrationAssociationSummaryTypeDef

```python
# IntegrationAssociationSummaryTypeDef definition

class IntegrationAssociationSummaryTypeDef(TypedDict):
    IntegrationAssociationId: NotRequired[str],
    IntegrationAssociationArn: NotRequired[str],
    InstanceId: NotRequired[str],
    IntegrationType: NotRequired[IntegrationTypeType],  # (1)
    IntegrationArn: NotRequired[str],
    SourceApplicationUrl: NotRequired[str],
    SourceApplicationName: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (2)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## TaskTemplateFieldIdentifierTypeDef

```python
# TaskTemplateFieldIdentifierTypeDef definition

class TaskTemplateFieldIdentifierTypeDef(TypedDict):
    Name: NotRequired[str],
```

## ListAgentStatusRequestRequestTypeDef

```python
# ListAgentStatusRequestRequestTypeDef definition

class ListAgentStatusRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AgentStatusTypes: NotRequired[Sequence[AgentStatusTypeType]],  # (1)
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
## ListAnalyticsDataAssociationsRequestRequestTypeDef

```python
# ListAnalyticsDataAssociationsRequestRequestTypeDef definition

class ListAnalyticsDataAssociationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    DataSetId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListApprovedOriginsRequestRequestTypeDef

```python
# ListApprovedOriginsRequestRequestTypeDef definition

class ListApprovedOriginsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListBotsRequestRequestTypeDef

```python
# ListBotsRequestRequestTypeDef definition

class ListBotsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype) 
## ListContactEvaluationsRequestRequestTypeDef

```python
# ListContactEvaluationsRequestRequestTypeDef definition

class ListContactEvaluationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    NextToken: NotRequired[str],
```

## ListContactFlowModulesRequestRequestTypeDef

```python
# ListContactFlowModulesRequestRequestTypeDef definition

class ListContactFlowModulesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ContactFlowModuleState: NotRequired[ContactFlowModuleStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
## ListContactFlowsRequestRequestTypeDef

```python
# ListContactFlowsRequestRequestTypeDef definition

class ListContactFlowsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowTypes: NotRequired[Sequence[ContactFlowTypeType]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
## ListContactReferencesRequestRequestTypeDef

```python
# ListContactReferencesRequestRequestTypeDef definition

class ListContactReferencesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
## ListDefaultVocabulariesRequestRequestTypeDef

```python
# ListDefaultVocabulariesRequestRequestTypeDef definition

class ListDefaultVocabulariesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## ListEvaluationFormVersionsRequestRequestTypeDef

```python
# ListEvaluationFormVersionsRequestRequestTypeDef definition

class ListEvaluationFormVersionsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEvaluationFormsRequestRequestTypeDef

```python
# ListEvaluationFormsRequestRequestTypeDef definition

class ListEvaluationFormsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFlowAssociationsRequestRequestTypeDef

```python
# ListFlowAssociationsRequestRequestTypeDef definition

class ListFlowAssociationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
## ListHoursOfOperationsRequestRequestTypeDef

```python
# ListHoursOfOperationsRequestRequestTypeDef definition

class ListHoursOfOperationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInstanceAttributesRequestRequestTypeDef

```python
# ListInstanceAttributesRequestRequestTypeDef definition

class ListInstanceAttributesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInstanceStorageConfigsRequestRequestTypeDef

```python
# ListInstanceStorageConfigsRequestRequestTypeDef definition

class ListInstanceStorageConfigsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
## ListInstancesRequestRequestTypeDef

```python
# ListInstancesRequestRequestTypeDef definition

class ListInstancesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIntegrationAssociationsRequestRequestTypeDef

```python
# ListIntegrationAssociationsRequestRequestTypeDef definition

class ListIntegrationAssociationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationType: NotRequired[IntegrationTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IntegrationArn: NotRequired[str],
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
## ListLambdaFunctionsRequestRequestTypeDef

```python
# ListLambdaFunctionsRequestRequestTypeDef definition

class ListLambdaFunctionsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListLexBotsRequestRequestTypeDef

```python
# ListLexBotsRequestRequestTypeDef definition

class ListLexBotsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPhoneNumbersRequestRequestTypeDef

```python
# ListPhoneNumbersRequestRequestTypeDef definition

class ListPhoneNumbersRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (1)
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
## PhoneNumberSummaryTypeDef

```python
# PhoneNumberSummaryTypeDef definition

class PhoneNumberSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (1)
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (2)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
## ListPhoneNumbersSummaryTypeDef

```python
# ListPhoneNumbersSummaryTypeDef definition

class ListPhoneNumbersSummaryTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    PhoneNumberArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (1)
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (2)
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberDescription: NotRequired[str],
    SourcePhoneNumberArn: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## ListPhoneNumbersV2RequestRequestTypeDef

```python
# ListPhoneNumbersV2RequestRequestTypeDef definition

class ListPhoneNumbersV2RequestRequestTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (1)
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (2)
    PhoneNumberPrefix: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## ListPredefinedAttributesRequestRequestTypeDef

```python
# ListPredefinedAttributesRequestRequestTypeDef definition

class ListPredefinedAttributesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PredefinedAttributeSummaryTypeDef

```python
# PredefinedAttributeSummaryTypeDef definition

class PredefinedAttributeSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListPromptsRequestRequestTypeDef

```python
# ListPromptsRequestRequestTypeDef definition

class ListPromptsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PromptSummaryTypeDef

```python
# PromptSummaryTypeDef definition

class PromptSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListQueueQuickConnectsRequestRequestTypeDef

```python
# ListQueueQuickConnectsRequestRequestTypeDef definition

class ListQueueQuickConnectsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QuickConnectSummaryTypeDef

```python
# QuickConnectSummaryTypeDef definition

class QuickConnectSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    QuickConnectType: NotRequired[QuickConnectTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
## ListQueuesRequestRequestTypeDef

```python
# ListQueuesRequestRequestTypeDef definition

class ListQueuesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueTypes: NotRequired[Sequence[QueueTypeType]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
## QueueSummaryTypeDef

```python
# QueueSummaryTypeDef definition

class QueueSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    QueueType: NotRequired[QueueTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
## ListQuickConnectsRequestRequestTypeDef

```python
# ListQuickConnectsRequestRequestTypeDef definition

class ListQuickConnectsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuickConnectTypes: NotRequired[Sequence[QuickConnectTypeType]],  # (1)
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
## ListRealtimeContactAnalysisSegmentsV2RequestRequestTypeDef

```python
# ListRealtimeContactAnalysisSegmentsV2RequestRequestTypeDef definition

class ListRealtimeContactAnalysisSegmentsV2RequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    OutputType: RealTimeContactAnalysisOutputTypeType,  # (1)
    SegmentTypes: Sequence[RealTimeContactAnalysisSegmentTypeType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RealTimeContactAnalysisOutputTypeType](./literals.md#realtimecontactanalysisoutputtypetype) 
2. See [:material-code-brackets: RealTimeContactAnalysisSegmentTypeType](./literals.md#realtimecontactanalysissegmenttypetype) 
## ListRoutingProfileQueuesRequestRequestTypeDef

```python
# ListRoutingProfileQueuesRequestRequestTypeDef definition

class ListRoutingProfileQueuesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RoutingProfileQueueConfigSummaryTypeDef

```python
# RoutingProfileQueueConfigSummaryTypeDef definition

class RoutingProfileQueueConfigSummaryTypeDef(TypedDict):
    QueueId: str,
    QueueArn: str,
    QueueName: str,
    Priority: int,
    Delay: int,
    Channel: ChannelType,  # (1)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
## ListRoutingProfilesRequestRequestTypeDef

```python
# ListRoutingProfilesRequestRequestTypeDef definition

class ListRoutingProfilesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RoutingProfileSummaryTypeDef

```python
# RoutingProfileSummaryTypeDef definition

class RoutingProfileSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListRulesRequestRequestTypeDef

```python
# ListRulesRequestRequestTypeDef definition

class ListRulesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    PublishStatus: NotRequired[RulePublishStatusType],  # (1)
    EventSourceName: NotRequired[EventSourceNameType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
## ListSecurityKeysRequestRequestTypeDef

```python
# ListSecurityKeysRequestRequestTypeDef definition

class ListSecurityKeysRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SecurityKeyTypeDef

```python
# SecurityKeyTypeDef definition

class SecurityKeyTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    Key: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

## ListSecurityProfileApplicationsRequestRequestTypeDef

```python
# ListSecurityProfileApplicationsRequestRequestTypeDef definition

class ListSecurityProfileApplicationsRequestRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSecurityProfilePermissionsRequestRequestTypeDef

```python
# ListSecurityProfilePermissionsRequestRequestTypeDef definition

class ListSecurityProfilePermissionsRequestRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSecurityProfilesRequestRequestTypeDef

```python
# ListSecurityProfilesRequestRequestTypeDef definition

class ListSecurityProfilesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SecurityProfileSummaryTypeDef

```python
# SecurityProfileSummaryTypeDef definition

class SecurityProfileSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTaskTemplatesRequestRequestTypeDef

```python
# ListTaskTemplatesRequestRequestTypeDef definition

class ListTaskTemplatesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Status: NotRequired[TaskTemplateStatusType],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
## TaskTemplateMetadataTypeDef

```python
# TaskTemplateMetadataTypeDef definition

class TaskTemplateMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[TaskTemplateStatusType],  # (1)
    LastModifiedTime: NotRequired[datetime],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
## ListTrafficDistributionGroupUsersRequestRequestTypeDef

```python
# ListTrafficDistributionGroupUsersRequestRequestTypeDef definition

class ListTrafficDistributionGroupUsersRequestRequestTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## TrafficDistributionGroupUserSummaryTypeDef

```python
# TrafficDistributionGroupUserSummaryTypeDef definition

class TrafficDistributionGroupUserSummaryTypeDef(TypedDict):
    UserId: NotRequired[str],
```

## ListTrafficDistributionGroupsRequestRequestTypeDef

```python
# ListTrafficDistributionGroupsRequestRequestTypeDef definition

class ListTrafficDistributionGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    InstanceId: NotRequired[str],
```

## TrafficDistributionGroupSummaryTypeDef

```python
# TrafficDistributionGroupSummaryTypeDef definition

class TrafficDistributionGroupSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    InstanceArn: NotRequired[str],
    Status: NotRequired[TrafficDistributionGroupStatusType],  # (1)
    IsDefault: NotRequired[bool],
```

1. See [:material-code-brackets: TrafficDistributionGroupStatusType](./literals.md#trafficdistributiongroupstatustype) 
## ListUseCasesRequestRequestTypeDef

```python
# ListUseCasesRequestRequestTypeDef definition

class ListUseCasesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## UseCaseTypeDef

```python
# UseCaseTypeDef definition

class UseCaseTypeDef(TypedDict):
    UseCaseId: NotRequired[str],
    UseCaseArn: NotRequired[str],
    UseCaseType: NotRequired[UseCaseTypeType],  # (1)
```

1. See [:material-code-brackets: UseCaseTypeType](./literals.md#usecasetypetype) 
## ListUserHierarchyGroupsRequestRequestTypeDef

```python
# ListUserHierarchyGroupsRequestRequestTypeDef definition

class ListUserHierarchyGroupsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListUserProficienciesRequestRequestTypeDef

```python
# ListUserProficienciesRequestRequestTypeDef definition

class ListUserProficienciesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## UserSummaryTypeDef

```python
# UserSummaryTypeDef definition

class UserSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Username: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

## ListViewVersionsRequestRequestTypeDef

```python
# ListViewVersionsRequestRequestTypeDef definition

class ListViewVersionsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ViewVersionSummaryTypeDef

```python
# ViewVersionSummaryTypeDef definition

class ViewVersionSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Description: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ViewTypeType],  # (1)
    Version: NotRequired[int],
    VersionDescription: NotRequired[str],
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
## ListViewsRequestRequestTypeDef

```python
# ListViewsRequestRequestTypeDef definition

class ListViewsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Type: NotRequired[ViewTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
## ViewSummaryTypeDef

```python
# ViewSummaryTypeDef definition

class ViewSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ViewTypeType],  # (1)
    Status: NotRequired[ViewStatusType],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
2. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
## MediaPlacementTypeDef

```python
# MediaPlacementTypeDef definition

class MediaPlacementTypeDef(TypedDict):
    AudioHostUrl: NotRequired[str],
    AudioFallbackUrl: NotRequired[str],
    SignalingUrl: NotRequired[str],
    TurnControlUrl: NotRequired[str],
    EventIngestionUrl: NotRequired[str],
```

## MetricFilterV2TypeDef

```python
# MetricFilterV2TypeDef definition

class MetricFilterV2TypeDef(TypedDict):
    MetricFilterKey: NotRequired[str],
    MetricFilterValues: NotRequired[Sequence[str]],
    Negate: NotRequired[bool],
```

## MetricIntervalTypeDef

```python
# MetricIntervalTypeDef definition

class MetricIntervalTypeDef(TypedDict):
    Interval: NotRequired[IntervalPeriodType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IntervalPeriodType](./literals.md#intervalperiodtype) 
## ThresholdV2TypeDef

```python
# ThresholdV2TypeDef definition

class ThresholdV2TypeDef(TypedDict):
    Comparison: NotRequired[str],
    ThresholdValue: NotRequired[float],
```

## MonitorContactRequestRequestTypeDef

```python
# MonitorContactRequestRequestTypeDef definition

class MonitorContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    UserId: str,
    AllowedMonitorCapabilities: NotRequired[Sequence[MonitorCapabilityType]],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: MonitorCapabilityType](./literals.md#monitorcapabilitytype) 
## ParticipantDetailsTypeDef

```python
# ParticipantDetailsTypeDef definition

class ParticipantDetailsTypeDef(TypedDict):
    DisplayName: str,
```

## NotificationRecipientTypeTypeDef

```python
# NotificationRecipientTypeTypeDef definition

class NotificationRecipientTypeTypeDef(TypedDict):
    UserTags: NotRequired[Mapping[str, str]],
    UserIds: NotRequired[Sequence[str]],
```

## NumberReferenceTypeDef

```python
# NumberReferenceTypeDef definition

class NumberReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## ParticipantTimerValueTypeDef

```python
# ParticipantTimerValueTypeDef definition

class ParticipantTimerValueTypeDef(TypedDict):
    ParticipantTimerAction: NotRequired[ParticipantTimerActionType],  # (1)
    ParticipantTimerDurationInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: ParticipantTimerActionType](./literals.md#participanttimeractiontype) 
## PauseContactRequestRequestTypeDef

```python
# PauseContactRequestRequestTypeDef definition

class PauseContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    ContactFlowId: NotRequired[str],
```

## PersistentChatTypeDef

```python
# PersistentChatTypeDef definition

class PersistentChatTypeDef(TypedDict):
    RehydrationType: NotRequired[RehydrationTypeType],  # (1)
    SourceContactId: NotRequired[str],
```

1. See [:material-code-brackets: RehydrationTypeType](./literals.md#rehydrationtypetype) 
## PhoneNumberQuickConnectConfigTypeDef

```python
# PhoneNumberQuickConnectConfigTypeDef definition

class PhoneNumberQuickConnectConfigTypeDef(TypedDict):
    PhoneNumber: str,
```

## PredefinedAttributeValuesPaginatorTypeDef

```python
# PredefinedAttributeValuesPaginatorTypeDef definition

class PredefinedAttributeValuesPaginatorTypeDef(TypedDict):
    StringList: NotRequired[List[str]],
```

## PutUserStatusRequestRequestTypeDef

```python
# PutUserStatusRequestRequestTypeDef definition

class PutUserStatusRequestRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
    AgentStatusId: str,
```

## QueueQuickConnectConfigTypeDef

```python
# QueueQuickConnectConfigTypeDef definition

class QueueQuickConnectConfigTypeDef(TypedDict):
    QueueId: str,
    ContactFlowId: str,
```

## UserQuickConnectConfigTypeDef

```python
# UserQuickConnectConfigTypeDef definition

class UserQuickConnectConfigTypeDef(TypedDict):
    UserId: str,
    ContactFlowId: str,
```

## RealTimeContactAnalysisAttachmentTypeDef

```python
# RealTimeContactAnalysisAttachmentTypeDef definition

class RealTimeContactAnalysisAttachmentTypeDef(TypedDict):
    AttachmentName: str,
    AttachmentId: str,
    ContentType: NotRequired[str],
    Status: NotRequired[ArtifactStatusType],  # (1)
```

1. See [:material-code-brackets: ArtifactStatusType](./literals.md#artifactstatustype) 
## RealTimeContactAnalysisCharacterIntervalTypeDef

```python
# RealTimeContactAnalysisCharacterIntervalTypeDef definition

class RealTimeContactAnalysisCharacterIntervalTypeDef(TypedDict):
    BeginOffsetChar: int,
    EndOffsetChar: int,
```

## RealTimeContactAnalysisTimeDataTypeDef

```python
# RealTimeContactAnalysisTimeDataTypeDef definition

class RealTimeContactAnalysisTimeDataTypeDef(TypedDict):
    AbsoluteTime: NotRequired[datetime],
```

## StringReferenceTypeDef

```python
# StringReferenceTypeDef definition

class StringReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## UrlReferenceTypeDef

```python
# UrlReferenceTypeDef definition

class UrlReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## ReferenceTypeDef

```python
# ReferenceTypeDef definition

class ReferenceTypeDef(TypedDict):
    Value: str,
    Type: ReferenceTypeType,  # (1)
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
## ReleasePhoneNumberRequestRequestTypeDef

```python
# ReleasePhoneNumberRequestRequestTypeDef definition

class ReleasePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    ClientToken: NotRequired[str],
```

## ReplicateInstanceRequestRequestTypeDef

```python
# ReplicateInstanceRequestRequestTypeDef definition

class ReplicateInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ReplicaRegion: str,
    ReplicaAlias: str,
    ClientToken: NotRequired[str],
```

## TagSearchConditionTypeDef

```python
# TagSearchConditionTypeDef definition

class TagSearchConditionTypeDef(TypedDict):
    tagKey: NotRequired[str],
    tagValue: NotRequired[str],
    tagKeyComparisonType: NotRequired[StringComparisonTypeType],  # (1)
    tagValueComparisonType: NotRequired[StringComparisonTypeType],  # (1)
```

1. See [:material-code-brackets: StringComparisonTypeType](./literals.md#stringcomparisontypetype) 
2. See [:material-code-brackets: StringComparisonTypeType](./literals.md#stringcomparisontypetype) 
## ResumeContactRecordingRequestRequestTypeDef

```python
# ResumeContactRecordingRequestRequestTypeDef definition

class ResumeContactRecordingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
```

## ResumeContactRequestRequestTypeDef

```python
# ResumeContactRequestRequestTypeDef definition

class ResumeContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    ContactFlowId: NotRequired[str],
```

## SearchAvailablePhoneNumbersRequestRequestTypeDef

```python
# SearchAvailablePhoneNumbersRequestRequestTypeDef definition

class SearchAvailablePhoneNumbersRequestRequestTypeDef(TypedDict):
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberPrefix: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    FieldName: SortableFieldNameType,  # (1)
    Order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SortableFieldNameType](./literals.md#sortablefieldnametype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SearchPredefinedAttributesRequestRequestTypeDef

```python
# SearchPredefinedAttributesRequestRequestTypeDef definition

class SearchPredefinedAttributesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchCriteria: NotRequired[PredefinedAttributeSearchCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: PredefinedAttributeSearchCriteriaTypeDef](./type_defs.md#predefinedattributesearchcriteriatypedef) 
## TagSetTypeDef

```python
# TagSetTypeDef definition

class TagSetTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## SecurityProfileSearchSummaryTypeDef

```python
# SecurityProfileSearchSummaryTypeDef definition

class SecurityProfileSearchSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    OrganizationResourceId: NotRequired[str],
    Arn: NotRequired[str],
    SecurityProfileName: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## SearchVocabulariesRequestRequestTypeDef

```python
# SearchVocabulariesRequestRequestTypeDef definition

class SearchVocabulariesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    State: NotRequired[VocabularyStateType],  # (1)
    NameStartsWith: NotRequired[str],
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (2)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
## VocabularySummaryTypeDef

```python
# VocabularySummaryTypeDef definition

class VocabularySummaryTypeDef(TypedDict):
    Name: str,
    Id: str,
    Arn: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    State: VocabularyStateType,  # (2)
    LastModifiedTime: datetime,
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
## SearchableContactAttributesCriteriaTypeDef

```python
# SearchableContactAttributesCriteriaTypeDef definition

class SearchableContactAttributesCriteriaTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## SegmentAttributeValueTypeDef

```python
# SegmentAttributeValueTypeDef definition

class SegmentAttributeValueTypeDef(TypedDict):
    ValueString: NotRequired[str],
```

## SignInDistributionTypeDef

```python
# SignInDistributionTypeDef definition

class SignInDistributionTypeDef(TypedDict):
    Region: str,
    Enabled: bool,
```

## StartContactEvaluationRequestRequestTypeDef

```python
# StartContactEvaluationRequestRequestTypeDef definition

class StartContactEvaluationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    EvaluationFormId: str,
    ClientToken: NotRequired[str],
```

## VoiceRecordingConfigurationTypeDef

```python
# VoiceRecordingConfigurationTypeDef definition

class VoiceRecordingConfigurationTypeDef(TypedDict):
    VoiceRecordingTrack: NotRequired[VoiceRecordingTrackType],  # (1)
```

1. See [:material-code-brackets: VoiceRecordingTrackType](./literals.md#voicerecordingtracktype) 
## StopContactRecordingRequestRequestTypeDef

```python
# StopContactRecordingRequestRequestTypeDef definition

class StopContactRecordingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
```

## StopContactStreamingRequestRequestTypeDef

```python
# StopContactStreamingRequestRequestTypeDef definition

class StopContactStreamingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    StreamingId: str,
```

## SuspendContactRecordingRequestRequestTypeDef

```python
# SuspendContactRecordingRequestRequestTypeDef definition

class SuspendContactRecordingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
```

## TagContactRequestRequestTypeDef

```python
# TagContactRequestRequestTypeDef definition

class TagContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    Tags: Mapping[str, str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TranscriptCriteriaTypeDef

```python
# TranscriptCriteriaTypeDef definition

class TranscriptCriteriaTypeDef(TypedDict):
    ParticipantRole: ParticipantRoleType,  # (1)
    SearchText: Sequence[str],
    MatchType: SearchContactsMatchTypeType,  # (2)
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## TransferContactRequestRequestTypeDef

```python
# TransferContactRequestRequestTypeDef definition

class TransferContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ContactFlowId: str,
    QueueId: NotRequired[str],
    UserId: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UntagContactRequestRequestTypeDef

```python
# UntagContactRequestRequestTypeDef definition

class UntagContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    TagKeys: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAgentStatusRequestRequestTypeDef

```python
# UpdateAgentStatusRequestRequestTypeDef definition

class UpdateAgentStatusRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AgentStatusId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[AgentStatusStateType],  # (1)
    DisplayOrder: NotRequired[int],
    ResetOrderNumber: NotRequired[bool],
```

1. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
## UpdateContactAttributesRequestRequestTypeDef

```python
# UpdateContactAttributesRequestRequestTypeDef definition

class UpdateContactAttributesRequestRequestTypeDef(TypedDict):
    InitialContactId: str,
    InstanceId: str,
    Attributes: Mapping[str, str],
```

## UpdateContactFlowContentRequestRequestTypeDef

```python
# UpdateContactFlowContentRequestRequestTypeDef definition

class UpdateContactFlowContentRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Content: str,
```

## UpdateContactFlowMetadataRequestRequestTypeDef

```python
# UpdateContactFlowMetadataRequestRequestTypeDef definition

class UpdateContactFlowMetadataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ContactFlowState: NotRequired[ContactFlowStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 
## UpdateContactFlowModuleContentRequestRequestTypeDef

```python
# UpdateContactFlowModuleContentRequestRequestTypeDef definition

class UpdateContactFlowModuleContentRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
    Content: str,
```

## UpdateContactFlowModuleMetadataRequestRequestTypeDef

```python
# UpdateContactFlowModuleMetadataRequestRequestTypeDef definition

class UpdateContactFlowModuleMetadataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[ContactFlowModuleStateType],  # (1)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
## UpdateContactFlowNameRequestRequestTypeDef

```python
# UpdateContactFlowNameRequestRequestTypeDef definition

class UpdateContactFlowNameRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateContactRoutingDataRequestRequestTypeDef

```python
# UpdateContactRoutingDataRequestRequestTypeDef definition

class UpdateContactRoutingDataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    QueueTimeAdjustmentSeconds: NotRequired[int],
    QueuePriority: NotRequired[int],
```

## UpdateInstanceAttributeRequestRequestTypeDef

```python
# UpdateInstanceAttributeRequestRequestTypeDef definition

class UpdateInstanceAttributeRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AttributeType: InstanceAttributeTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
## UpdatePhoneNumberMetadataRequestRequestTypeDef

```python
# UpdatePhoneNumberMetadataRequestRequestTypeDef definition

class UpdatePhoneNumberMetadataRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberDescription: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UpdatePhoneNumberRequestRequestTypeDef

```python
# UpdatePhoneNumberRequestRequestTypeDef definition

class UpdatePhoneNumberRequestRequestTypeDef(TypedDict):
    PhoneNumberId: str,
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    ClientToken: NotRequired[str],
```

## UpdatePromptRequestRequestTypeDef

```python
# UpdatePromptRequestRequestTypeDef definition

class UpdatePromptRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    PromptId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    S3Uri: NotRequired[str],
```

## UpdateQueueHoursOfOperationRequestRequestTypeDef

```python
# UpdateQueueHoursOfOperationRequestRequestTypeDef definition

class UpdateQueueHoursOfOperationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    HoursOfOperationId: str,
```

## UpdateQueueMaxContactsRequestRequestTypeDef

```python
# UpdateQueueMaxContactsRequestRequestTypeDef definition

class UpdateQueueMaxContactsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    MaxContacts: NotRequired[int],
```

## UpdateQueueNameRequestRequestTypeDef

```python
# UpdateQueueNameRequestRequestTypeDef definition

class UpdateQueueNameRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateQueueStatusRequestRequestTypeDef

```python
# UpdateQueueStatusRequestRequestTypeDef definition

class UpdateQueueStatusRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    Status: QueueStatusType,  # (1)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## UpdateQuickConnectNameRequestRequestTypeDef

```python
# UpdateQuickConnectNameRequestRequestTypeDef definition

class UpdateQuickConnectNameRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateRoutingProfileAgentAvailabilityTimerRequestRequestTypeDef

```python
# UpdateRoutingProfileAgentAvailabilityTimerRequestRequestTypeDef definition

class UpdateRoutingProfileAgentAvailabilityTimerRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    AgentAvailabilityTimer: AgentAvailabilityTimerType,  # (1)
```

1. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
## UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef

```python
# UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef definition

class UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    DefaultOutboundQueueId: str,
```

## UpdateRoutingProfileNameRequestRequestTypeDef

```python
# UpdateRoutingProfileNameRequestRequestTypeDef definition

class UpdateRoutingProfileNameRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateUserHierarchyGroupNameRequestRequestTypeDef

```python
# UpdateUserHierarchyGroupNameRequestRequestTypeDef definition

class UpdateUserHierarchyGroupNameRequestRequestTypeDef(TypedDict):
    Name: str,
    HierarchyGroupId: str,
    InstanceId: str,
```

## UpdateUserHierarchyRequestRequestTypeDef

```python
# UpdateUserHierarchyRequestRequestTypeDef definition

class UpdateUserHierarchyRequestRequestTypeDef(TypedDict):
    UserId: str,
    InstanceId: str,
    HierarchyGroupId: NotRequired[str],
```

## UpdateUserRoutingProfileRequestRequestTypeDef

```python
# UpdateUserRoutingProfileRequestRequestTypeDef definition

class UpdateUserRoutingProfileRequestRequestTypeDef(TypedDict):
    RoutingProfileId: str,
    UserId: str,
    InstanceId: str,
```

## UpdateUserSecurityProfilesRequestRequestTypeDef

```python
# UpdateUserSecurityProfilesRequestRequestTypeDef definition

class UpdateUserSecurityProfilesRequestRequestTypeDef(TypedDict):
    SecurityProfileIds: Sequence[str],
    UserId: str,
    InstanceId: str,
```

## UpdateViewMetadataRequestRequestTypeDef

```python
# UpdateViewMetadataRequestRequestTypeDef definition

class UpdateViewMetadataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UserReferenceTypeDef

```python
# UserReferenceTypeDef definition

class UserReferenceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## UserIdentityInfoLiteTypeDef

```python
# UserIdentityInfoLiteTypeDef definition

class UserIdentityInfoLiteTypeDef(TypedDict):
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
```

## ViewContentTypeDef

```python
# ViewContentTypeDef definition

class ViewContentTypeDef(TypedDict):
    InputSchema: NotRequired[str],
    Template: NotRequired[str],
    Actions: NotRequired[List[str]],
```

## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    Name: str,
    RuleId: str,
    RuleArn: str,
    EventSourceName: EventSourceNameType,  # (1)
    PublishStatus: RulePublishStatusType,  # (2)
    ActionSummaries: List[ActionSummaryTypeDef],  # (3)
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
```

1. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
2. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
3. See [:material-code-braces: ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef) 
## ActivateEvaluationFormResponseTypeDef

```python
# ActivateEvaluationFormResponseTypeDef definition

class ActivateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    EvaluationFormVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateAnalyticsDataSetResponseTypeDef

```python
# AssociateAnalyticsDataSetResponseTypeDef definition

class AssociateAnalyticsDataSetResponseTypeDef(TypedDict):
    DataSetId: str,
    TargetAccountId: str,
    ResourceShareId: str,
    ResourceShareArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateInstanceStorageConfigResponseTypeDef

```python
# AssociateInstanceStorageConfigResponseTypeDef definition

class AssociateInstanceStorageConfigResponseTypeDef(TypedDict):
    AssociationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateSecurityKeyResponseTypeDef

```python
# AssociateSecurityKeyResponseTypeDef definition

class AssociateSecurityKeyResponseTypeDef(TypedDict):
    AssociationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClaimPhoneNumberResponseTypeDef

```python
# ClaimPhoneNumberResponseTypeDef definition

class ClaimPhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAgentStatusResponseTypeDef

```python
# CreateAgentStatusResponseTypeDef definition

class CreateAgentStatusResponseTypeDef(TypedDict):
    AgentStatusARN: str,
    AgentStatusId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactFlowModuleResponseTypeDef

```python
# CreateContactFlowModuleResponseTypeDef definition

class CreateContactFlowModuleResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactFlowResponseTypeDef

```python
# CreateContactFlowResponseTypeDef definition

class CreateContactFlowResponseTypeDef(TypedDict):
    ContactFlowId: str,
    ContactFlowArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEvaluationFormResponseTypeDef

```python
# CreateEvaluationFormResponseTypeDef definition

class CreateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHoursOfOperationResponseTypeDef

```python
# CreateHoursOfOperationResponseTypeDef definition

class CreateHoursOfOperationResponseTypeDef(TypedDict):
    HoursOfOperationId: str,
    HoursOfOperationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResponseTypeDef

```python
# CreateInstanceResponseTypeDef definition

class CreateInstanceResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationAssociationResponseTypeDef

```python
# CreateIntegrationAssociationResponseTypeDef definition

class CreateIntegrationAssociationResponseTypeDef(TypedDict):
    IntegrationAssociationId: str,
    IntegrationAssociationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePersistentContactAssociationResponseTypeDef

```python
# CreatePersistentContactAssociationResponseTypeDef definition

class CreatePersistentContactAssociationResponseTypeDef(TypedDict):
    ContinuedFromContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePromptResponseTypeDef

```python
# CreatePromptResponseTypeDef definition

class CreatePromptResponseTypeDef(TypedDict):
    PromptARN: str,
    PromptId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    QueueArn: str,
    QueueId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQuickConnectResponseTypeDef

```python
# CreateQuickConnectResponseTypeDef definition

class CreateQuickConnectResponseTypeDef(TypedDict):
    QuickConnectARN: str,
    QuickConnectId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRoutingProfileResponseTypeDef

```python
# CreateRoutingProfileResponseTypeDef definition

class CreateRoutingProfileResponseTypeDef(TypedDict):
    RoutingProfileArn: str,
    RoutingProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleResponseTypeDef

```python
# CreateRuleResponseTypeDef definition

class CreateRuleResponseTypeDef(TypedDict):
    RuleArn: str,
    RuleId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityProfileResponseTypeDef

```python
# CreateSecurityProfileResponseTypeDef definition

class CreateSecurityProfileResponseTypeDef(TypedDict):
    SecurityProfileId: str,
    SecurityProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskTemplateResponseTypeDef

```python
# CreateTaskTemplateResponseTypeDef definition

class CreateTaskTemplateResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrafficDistributionGroupResponseTypeDef

```python
# CreateTrafficDistributionGroupResponseTypeDef definition

class CreateTrafficDistributionGroupResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUseCaseResponseTypeDef

```python
# CreateUseCaseResponseTypeDef definition

class CreateUseCaseResponseTypeDef(TypedDict):
    UseCaseId: str,
    UseCaseArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserHierarchyGroupResponseTypeDef

```python
# CreateUserHierarchyGroupResponseTypeDef definition

class CreateUserHierarchyGroupResponseTypeDef(TypedDict):
    HierarchyGroupId: str,
    HierarchyGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    UserId: str,
    UserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVocabularyResponseTypeDef

```python
# CreateVocabularyResponseTypeDef definition

class CreateVocabularyResponseTypeDef(TypedDict):
    VocabularyArn: str,
    VocabularyId: str,
    State: VocabularyStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeactivateEvaluationFormResponseTypeDef

```python
# DeactivateEvaluationFormResponseTypeDef definition

class DeactivateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    EvaluationFormVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVocabularyResponseTypeDef

```python
# DeleteVocabularyResponseTypeDef definition

class DeleteVocabularyResponseTypeDef(TypedDict):
    VocabularyArn: str,
    VocabularyId: str,
    State: VocabularyStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactAttributesResponseTypeDef

```python
# GetContactAttributesResponseTypeDef definition

class GetContactAttributesResponseTypeDef(TypedDict):
    Attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFlowAssociationResponseTypeDef

```python
# GetFlowAssociationResponseTypeDef definition

class GetFlowAssociationResponseTypeDef(TypedDict):
    ResourceId: str,
    FlowId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPromptFileResponseTypeDef

```python
# GetPromptFileResponseTypeDef definition

class GetPromptFileResponseTypeDef(TypedDict):
    PromptPresignedUrl: str,
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportPhoneNumberResponseTypeDef

```python
# ImportPhoneNumberResponseTypeDef definition

class ImportPhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApprovedOriginsResponseTypeDef

```python
# ListApprovedOriginsResponseTypeDef definition

class ListApprovedOriginsResponseTypeDef(TypedDict):
    Origins: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLambdaFunctionsResponseTypeDef

```python
# ListLambdaFunctionsResponseTypeDef definition

class ListLambdaFunctionsResponseTypeDef(TypedDict):
    LambdaFunctions: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfilePermissionsResponseTypeDef

```python
# ListSecurityProfilePermissionsResponseTypeDef definition

class ListSecurityProfilePermissionsResponseTypeDef(TypedDict):
    Permissions: List[str],
    NextToken: str,
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MonitorContactResponseTypeDef

```python
# MonitorContactResponseTypeDef definition

class MonitorContactResponseTypeDef(TypedDict):
    ContactId: str,
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicateInstanceResponseTypeDef

```python
# ReplicateInstanceResponseTypeDef definition

class ReplicateInstanceResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendChatIntegrationEventResponseTypeDef

```python
# SendChatIntegrationEventResponseTypeDef definition

class SendChatIntegrationEventResponseTypeDef(TypedDict):
    InitialContactId: str,
    NewChatCreated: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChatContactResponseTypeDef

```python
# StartChatContactResponseTypeDef definition

class StartChatContactResponseTypeDef(TypedDict):
    ContactId: str,
    ParticipantId: str,
    ParticipantToken: str,
    ContinuedFromContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactEvaluationResponseTypeDef

```python
# StartContactEvaluationResponseTypeDef definition

class StartContactEvaluationResponseTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactStreamingResponseTypeDef

```python
# StartContactStreamingResponseTypeDef definition

class StartContactStreamingResponseTypeDef(TypedDict):
    StreamingId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartOutboundVoiceContactResponseTypeDef

```python
# StartOutboundVoiceContactResponseTypeDef definition

class StartOutboundVoiceContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTaskContactResponseTypeDef

```python
# StartTaskContactResponseTypeDef definition

class StartTaskContactResponseTypeDef(TypedDict):
    ContactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitContactEvaluationResponseTypeDef

```python
# SubmitContactEvaluationResponseTypeDef definition

class SubmitContactEvaluationResponseTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransferContactResponseTypeDef

```python
# TransferContactResponseTypeDef definition

class TransferContactResponseTypeDef(TypedDict):
    ContactId: str,
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContactEvaluationResponseTypeDef

```python
# UpdateContactEvaluationResponseTypeDef definition

class UpdateContactEvaluationResponseTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEvaluationFormResponseTypeDef

```python
# UpdateEvaluationFormResponseTypeDef definition

class UpdateEvaluationFormResponseTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormArn: str,
    EvaluationFormVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePhoneNumberResponseTypeDef

```python
# UpdatePhoneNumberResponseTypeDef definition

class UpdatePhoneNumberResponseTypeDef(TypedDict):
    PhoneNumberId: str,
    PhoneNumberArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePromptResponseTypeDef

```python
# UpdatePromptResponseTypeDef definition

class UpdatePromptResponseTypeDef(TypedDict):
    PromptARN: str,
    PromptId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AgentConfigTypeDef

```python
# AgentConfigTypeDef definition

class AgentConfigTypeDef(TypedDict):
    Distributions: List[DistributionTypeDef],  # (1)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## TelephonyConfigTypeDef

```python
# TelephonyConfigTypeDef definition

class TelephonyConfigTypeDef(TypedDict):
    Distributions: List[DistributionTypeDef],  # (1)
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## AgentContactReferenceTypeDef

```python
# AgentContactReferenceTypeDef definition

class AgentContactReferenceTypeDef(TypedDict):
    ContactId: NotRequired[str],
    Channel: NotRequired[ChannelType],  # (1)
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (2)
    AgentContactState: NotRequired[ContactStateType],  # (3)
    StateStartTimestamp: NotRequired[datetime],
    ConnectedToAgentTimestamp: NotRequired[datetime],
    Queue: NotRequired[QueueReferenceTypeDef],  # (4)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
2. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
3. See [:material-code-brackets: ContactStateType](./literals.md#contactstatetype) 
4. See [:material-code-braces: QueueReferenceTypeDef](./type_defs.md#queuereferencetypedef) 
## ListAgentStatusResponseTypeDef

```python
# ListAgentStatusResponseTypeDef definition

class ListAgentStatusResponseTypeDef(TypedDict):
    NextToken: str,
    AgentStatusSummaryList: List[AgentStatusSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentStatusSummaryTypeDef](./type_defs.md#agentstatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAgentStatusResponseTypeDef

```python
# DescribeAgentStatusResponseTypeDef definition

class DescribeAgentStatusResponseTypeDef(TypedDict):
    AgentStatus: AgentStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentStatusTypeDef](./type_defs.md#agentstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AllowedCapabilitiesTypeDef

```python
# AllowedCapabilitiesTypeDef definition

class AllowedCapabilitiesTypeDef(TypedDict):
    Customer: NotRequired[ParticipantCapabilitiesTypeDef],  # (1)
    Agent: NotRequired[ParticipantCapabilitiesTypeDef],  # (1)
```

1. See [:material-code-braces: ParticipantCapabilitiesTypeDef](./type_defs.md#participantcapabilitiestypedef) 
2. See [:material-code-braces: ParticipantCapabilitiesTypeDef](./type_defs.md#participantcapabilitiestypedef) 
## ListAnalyticsDataAssociationsResponseTypeDef

```python
# ListAnalyticsDataAssociationsResponseTypeDef definition

class ListAnalyticsDataAssociationsResponseTypeDef(TypedDict):
    Results: List[AnalyticsDataAssociationResultTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyticsDataAssociationResultTypeDef](./type_defs.md#analyticsdataassociationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfileApplicationsResponsePaginatorTypeDef

```python
# ListSecurityProfileApplicationsResponsePaginatorTypeDef definition

class ListSecurityProfileApplicationsResponsePaginatorTypeDef(TypedDict):
    Applications: List[ApplicationPaginatorTypeDef],  # (1)
    NextToken: str,
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationPaginatorTypeDef](./type_defs.md#applicationpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityProfileRequestRequestTypeDef

```python
# CreateSecurityProfileRequestRequestTypeDef definition

class CreateSecurityProfileRequestRequestTypeDef(TypedDict):
    SecurityProfileName: str,
    InstanceId: str,
    Description: NotRequired[str],
    Permissions: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
    AllowedAccessControlTags: NotRequired[Mapping[str, str]],
    TagRestrictedResources: NotRequired[Sequence[str]],
    Applications: NotRequired[Sequence[ApplicationTypeDef]],  # (1)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
## ListSecurityProfileApplicationsResponseTypeDef

```python
# ListSecurityProfileApplicationsResponseTypeDef definition

class ListSecurityProfileApplicationsResponseTypeDef(TypedDict):
    Applications: List[ApplicationTypeDef],  # (1)
    NextToken: str,
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityProfileRequestRequestTypeDef

```python
# UpdateSecurityProfileRequestRequestTypeDef definition

class UpdateSecurityProfileRequestRequestTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    Description: NotRequired[str],
    Permissions: NotRequired[Sequence[str]],
    AllowedAccessControlTags: NotRequired[Mapping[str, str]],
    TagRestrictedResources: NotRequired[Sequence[str]],
    Applications: NotRequired[Sequence[ApplicationTypeDef]],  # (1)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
## AssociateLexBotRequestRequestTypeDef

```python
# AssociateLexBotRequestRequestTypeDef definition

class AssociateLexBotRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LexBot: LexBotTypeDef,  # (1)
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
## ListLexBotsResponseTypeDef

```python
# ListLexBotsResponseTypeDef definition

class ListLexBotsResponseTypeDef(TypedDict):
    LexBots: List[LexBotTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateBotRequestRequestTypeDef

```python
# AssociateBotRequestRequestTypeDef definition

class AssociateBotRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LexBot: NotRequired[LexBotTypeDef],  # (1)
    LexV2Bot: NotRequired[LexV2BotTypeDef],  # (2)
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
## DisassociateBotRequestRequestTypeDef

```python
# DisassociateBotRequestRequestTypeDef definition

class DisassociateBotRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LexBot: NotRequired[LexBotTypeDef],  # (1)
    LexV2Bot: NotRequired[LexV2BotTypeDef],  # (2)
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
## LexBotConfigTypeDef

```python
# LexBotConfigTypeDef definition

class LexBotConfigTypeDef(TypedDict):
    LexBot: NotRequired[LexBotTypeDef],  # (1)
    LexV2Bot: NotRequired[LexV2BotTypeDef],  # (2)
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
## AssociateUserProficienciesRequestRequestTypeDef

```python
# AssociateUserProficienciesRequestRequestTypeDef definition

class AssociateUserProficienciesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyTypeDef],  # (1)
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
## ListUserProficienciesResponseTypeDef

```python
# ListUserProficienciesResponseTypeDef definition

class ListUserProficienciesResponseTypeDef(TypedDict):
    NextToken: str,
    UserProficiencyList: List[UserProficiencyTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserProficienciesRequestRequestTypeDef

```python
# UpdateUserProficienciesRequestRequestTypeDef definition

class UpdateUserProficienciesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyTypeDef],  # (1)
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
## DescribeInstanceAttributeResponseTypeDef

```python
# DescribeInstanceAttributeResponseTypeDef definition

class DescribeInstanceAttributeResponseTypeDef(TypedDict):
    Attribute: AttributeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceAttributesResponseTypeDef

```python
# ListInstanceAttributesResponseTypeDef definition

class ListInstanceAttributesResponseTypeDef(TypedDict):
    Attributes: List[AttributeTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MeetingFeaturesConfigurationTypeDef

```python
# MeetingFeaturesConfigurationTypeDef definition

class MeetingFeaturesConfigurationTypeDef(TypedDict):
    Audio: NotRequired[AudioFeaturesTypeDef],  # (1)
```

1. See [:material-code-braces: AudioFeaturesTypeDef](./type_defs.md#audiofeaturestypedef) 
## SearchAvailablePhoneNumbersResponseTypeDef

```python
# SearchAvailablePhoneNumbersResponseTypeDef definition

class SearchAvailablePhoneNumbersResponseTypeDef(TypedDict):
    NextToken: str,
    AvailableNumbersList: List[AvailableNumberSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AvailableNumberSummaryTypeDef](./type_defs.md#availablenumbersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchAssociateAnalyticsDataSetResponseTypeDef

```python
# BatchAssociateAnalyticsDataSetResponseTypeDef definition

class BatchAssociateAnalyticsDataSetResponseTypeDef(TypedDict):
    Created: List[AnalyticsDataAssociationResultTypeDef],  # (1)
    Errors: List[ErrorResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AnalyticsDataAssociationResultTypeDef](./type_defs.md#analyticsdataassociationresulttypedef) 
2. See [:material-code-braces: ErrorResultTypeDef](./type_defs.md#errorresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateAnalyticsDataSetResponseTypeDef

```python
# BatchDisassociateAnalyticsDataSetResponseTypeDef definition

class BatchDisassociateAnalyticsDataSetResponseTypeDef(TypedDict):
    Deleted: List[str],
    Errors: List[ErrorResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ErrorResultTypeDef](./type_defs.md#errorresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetFlowAssociationResponseTypeDef

```python
# BatchGetFlowAssociationResponseTypeDef definition

class BatchGetFlowAssociationResponseTypeDef(TypedDict):
    FlowAssociationSummaryList: List[FlowAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowAssociationSummaryTypeDef](./type_defs.md#flowassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFlowAssociationsResponseTypeDef

```python
# ListFlowAssociationsResponseTypeDef definition

class ListFlowAssociationsResponseTypeDef(TypedDict):
    FlowAssociationSummaryList: List[FlowAssociationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowAssociationSummaryTypeDef](./type_defs.md#flowassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutContactResponseTypeDef

```python
# BatchPutContactResponseTypeDef definition

class BatchPutContactResponseTypeDef(TypedDict):
    SuccessfulRequestList: List[SuccessfulRequestTypeDef],  # (1)
    FailedRequestList: List[FailedRequestTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef) 
2. See [:material-code-braces: FailedRequestTypeDef](./type_defs.md#failedrequesttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartContactStreamingRequestRequestTypeDef

```python
# StartContactStreamingRequestRequestTypeDef definition

class StartContactStreamingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ChatStreamingConfiguration: ChatStreamingConfigurationTypeDef,  # (1)
    ClientToken: str,
```

1. See [:material-code-braces: ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef) 
## ClaimedPhoneNumberSummaryTypeDef

```python
# ClaimedPhoneNumberSummaryTypeDef definition

class ClaimedPhoneNumberSummaryTypeDef(TypedDict):
    PhoneNumberId: NotRequired[str],
    PhoneNumberArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    PhoneNumberCountryCode: NotRequired[PhoneNumberCountryCodeType],  # (1)
    PhoneNumberType: NotRequired[PhoneNumberTypeType],  # (2)
    PhoneNumberDescription: NotRequired[str],
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    PhoneNumberStatus: NotRequired[PhoneNumberStatusTypeDef],  # (3)
    SourcePhoneNumberArn: NotRequired[str],
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: PhoneNumberStatusTypeDef](./type_defs.md#phonenumberstatustypedef) 
## ContactDataRequestTypeDef

```python
# ContactDataRequestTypeDef definition

class ContactDataRequestTypeDef(TypedDict):
    SystemEndpoint: NotRequired[EndpointTypeDef],  # (1)
    CustomerEndpoint: NotRequired[EndpointTypeDef],  # (1)
    RequestIdentifier: NotRequired[str],
    QueueId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    Campaign: NotRequired[CampaignTypeDef],  # (3)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: CampaignTypeDef](./type_defs.md#campaigntypedef) 
## UserDataFiltersTypeDef

```python
# UserDataFiltersTypeDef definition

class UserDataFiltersTypeDef(TypedDict):
    Queues: NotRequired[Sequence[str]],
    ContactFilter: NotRequired[ContactFilterTypeDef],  # (1)
    RoutingProfiles: NotRequired[Sequence[str]],
    Agents: NotRequired[Sequence[str]],
    UserHierarchyGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ContactFilterTypeDef](./type_defs.md#contactfiltertypedef) 
## ListContactFlowModulesResponseTypeDef

```python
# ListContactFlowModulesResponseTypeDef definition

class ListContactFlowModulesResponseTypeDef(TypedDict):
    ContactFlowModulesSummaryList: List[ContactFlowModuleSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactFlowModuleSummaryTypeDef](./type_defs.md#contactflowmodulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactFlowModuleResponseTypeDef

```python
# DescribeContactFlowModuleResponseTypeDef definition

class DescribeContactFlowModuleResponseTypeDef(TypedDict):
    ContactFlowModule: ContactFlowModuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactFlowModuleTypeDef](./type_defs.md#contactflowmoduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContactFlowsResponseTypeDef

```python
# ListContactFlowsResponseTypeDef definition

class ListContactFlowsResponseTypeDef(TypedDict):
    ContactFlowSummaryList: List[ContactFlowSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactFlowSummaryTypeDef](./type_defs.md#contactflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactFlowResponseTypeDef

```python
# DescribeContactFlowResponseTypeDef definition

class DescribeContactFlowResponseTypeDef(TypedDict):
    ContactFlow: ContactFlowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactFlowTypeDef](./type_defs.md#contactflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContactSearchSummaryTypeDef

```python
# ContactSearchSummaryTypeDef definition

class ContactSearchSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    InitialContactId: NotRequired[str],
    PreviousContactId: NotRequired[str],
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (1)
    Channel: NotRequired[ChannelType],  # (2)
    QueueInfo: NotRequired[ContactSearchSummaryQueueInfoTypeDef],  # (3)
    AgentInfo: NotRequired[ContactSearchSummaryAgentInfoTypeDef],  # (4)
    InitiationTimestamp: NotRequired[datetime],
    DisconnectTimestamp: NotRequired[datetime],
    ScheduledTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: ContactSearchSummaryQueueInfoTypeDef](./type_defs.md#contactsearchsummaryqueueinfotypedef) 
4. See [:material-code-braces: ContactSearchSummaryAgentInfoTypeDef](./type_defs.md#contactsearchsummaryagentinfotypedef) 
## ContactTypeDef

```python
# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    InitialContactId: NotRequired[str],
    PreviousContactId: NotRequired[str],
    InitiationMethod: NotRequired[ContactInitiationMethodType],  # (1)
    Name: NotRequired[str],
    Description: NotRequired[str],
    Channel: NotRequired[ChannelType],  # (2)
    QueueInfo: NotRequired[QueueInfoTypeDef],  # (3)
    AgentInfo: NotRequired[AgentInfoTypeDef],  # (4)
    InitiationTimestamp: NotRequired[datetime],
    DisconnectTimestamp: NotRequired[datetime],
    LastUpdateTimestamp: NotRequired[datetime],
    LastPausedTimestamp: NotRequired[datetime],
    LastResumedTimestamp: NotRequired[datetime],
    TotalPauseCount: NotRequired[int],
    TotalPauseDurationInSeconds: NotRequired[int],
    ScheduledTimestamp: NotRequired[datetime],
    RelatedContactId: NotRequired[str],
    WisdomInfo: NotRequired[WisdomInfoTypeDef],  # (5)
    QueueTimeAdjustmentSeconds: NotRequired[int],
    QueuePriority: NotRequired[int],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: QueueInfoTypeDef](./type_defs.md#queueinfotypedef) 
4. See [:material-code-braces: AgentInfoTypeDef](./type_defs.md#agentinfotypedef) 
5. See [:material-code-braces: WisdomInfoTypeDef](./type_defs.md#wisdominfotypedef) 
## ControlPlaneTagFilterTypeDef

```python
# ControlPlaneTagFilterTypeDef definition

class ControlPlaneTagFilterTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Sequence[TagConditionTypeDef]]],  # (1)
    AndConditions: NotRequired[Sequence[TagConditionTypeDef]],  # (2)
    TagCondition: NotRequired[TagConditionTypeDef],  # (3)
```

1. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
2. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
3. See [:material-code-braces: TagConditionTypeDef](./type_defs.md#tagconditiontypedef) 
## CreateEvaluationFormRequestRequestTypeDef

```python
# CreateEvaluationFormRequestRequestTypeDef definition

class CreateEvaluationFormRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Title: str,
    Items: Sequence[EvaluationFormItemTypeDef],  # (1)
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## EvaluationFormContentTypeDef

```python
# EvaluationFormContentTypeDef definition

class EvaluationFormContentTypeDef(TypedDict):
    EvaluationFormVersion: int,
    EvaluationFormId: str,
    EvaluationFormArn: str,
    Title: str,
    Items: List[EvaluationFormItemTypeDef],  # (1)
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## EvaluationFormTypeDef

```python
# EvaluationFormTypeDef definition

class EvaluationFormTypeDef(TypedDict):
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Locked: bool,
    EvaluationFormArn: str,
    Title: str,
    Status: EvaluationFormVersionStatusType,  # (1)
    Items: List[EvaluationFormItemTypeDef],  # (2)
    CreatedTime: datetime,
    CreatedBy: str,
    LastModifiedTime: datetime,
    LastModifiedBy: str,
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (3)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EvaluationFormVersionStatusType](./literals.md#evaluationformversionstatustype) 
2. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
3. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## UpdateEvaluationFormRequestRequestTypeDef

```python
# UpdateEvaluationFormRequestRequestTypeDef definition

class UpdateEvaluationFormRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Title: str,
    Items: Sequence[EvaluationFormItemTypeDef],  # (1)
    CreateNewVersion: NotRequired[bool],
    Description: NotRequired[str],
    ScoringStrategy: NotRequired[EvaluationFormScoringStrategyTypeDef],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
## CreateParticipantRequestRequestTypeDef

```python
# CreateParticipantRequestRequestTypeDef definition

class CreateParticipantRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ParticipantDetails: ParticipantDetailsToAddTypeDef,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ParticipantDetailsToAddTypeDef](./type_defs.md#participantdetailstoaddtypedef) 
## CreateParticipantResponseTypeDef

```python
# CreateParticipantResponseTypeDef definition

class CreateParticipantResponseTypeDef(TypedDict):
    ParticipantCredentials: ParticipantTokenCredentialsTypeDef,  # (1)
    ParticipantId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParticipantTokenCredentialsTypeDef](./type_defs.md#participanttokencredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePredefinedAttributeRequestRequestTypeDef

```python
# CreatePredefinedAttributeRequestRequestTypeDef definition

class CreatePredefinedAttributeRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Values: PredefinedAttributeValuesTypeDef,  # (1)
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) 
## PredefinedAttributeTypeDef

```python
# PredefinedAttributeTypeDef definition

class PredefinedAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[PredefinedAttributeValuesTypeDef],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) 
## UpdatePredefinedAttributeRequestRequestTypeDef

```python
# UpdatePredefinedAttributeRequestRequestTypeDef definition

class UpdatePredefinedAttributeRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Values: NotRequired[PredefinedAttributeValuesTypeDef],  # (1)
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) 
## CreateQueueRequestRequestTypeDef

```python
# CreateQueueRequestRequestTypeDef definition

class CreateQueueRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    HoursOfOperationId: str,
    Description: NotRequired[str],
    OutboundCallerConfig: NotRequired[OutboundCallerConfigTypeDef],  # (1)
    MaxContacts: NotRequired[int],
    QuickConnectIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
## QueueTypeDef

```python
# QueueTypeDef definition

class QueueTypeDef(TypedDict):
    Name: NotRequired[str],
    QueueArn: NotRequired[str],
    QueueId: NotRequired[str],
    Description: NotRequired[str],
    OutboundCallerConfig: NotRequired[OutboundCallerConfigTypeDef],  # (1)
    HoursOfOperationId: NotRequired[str],
    MaxContacts: NotRequired[int],
    Status: NotRequired[QueueStatusType],  # (2)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
2. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## UpdateQueueOutboundCallerConfigRequestRequestTypeDef

```python
# UpdateQueueOutboundCallerConfigRequestRequestTypeDef definition

class UpdateQueueOutboundCallerConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    OutboundCallerConfig: OutboundCallerConfigTypeDef,  # (1)
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
## UpdateUserIdentityInfoRequestRequestTypeDef

```python
# UpdateUserIdentityInfoRequestRequestTypeDef definition

class UpdateUserIdentityInfoRequestRequestTypeDef(TypedDict):
    IdentityInfo: UserIdentityInfoTypeDef,  # (1)
    UserId: str,
    InstanceId: str,
```

1. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    Username: str,
    PhoneConfig: UserPhoneConfigTypeDef,  # (1)
    SecurityProfileIds: Sequence[str],
    RoutingProfileId: str,
    InstanceId: str,
    Password: NotRequired[str],
    IdentityInfo: NotRequired[UserIdentityInfoTypeDef],  # (2)
    DirectoryUserId: NotRequired[str],
    HierarchyGroupId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
2. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
## UpdateUserPhoneConfigRequestRequestTypeDef

```python
# UpdateUserPhoneConfigRequestRequestTypeDef definition

class UpdateUserPhoneConfigRequestRequestTypeDef(TypedDict):
    PhoneConfig: UserPhoneConfigTypeDef,  # (1)
    UserId: str,
    InstanceId: str,
```

1. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Username: NotRequired[str],
    IdentityInfo: NotRequired[UserIdentityInfoTypeDef],  # (1)
    PhoneConfig: NotRequired[UserPhoneConfigTypeDef],  # (2)
    DirectoryUserId: NotRequired[str],
    SecurityProfileIds: NotRequired[List[str]],
    RoutingProfileId: NotRequired[str],
    HierarchyGroupId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
2. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
## CreateViewRequestRequestTypeDef

```python
# CreateViewRequestRequestTypeDef definition

class CreateViewRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Status: ViewStatusType,  # (1)
    Content: ViewInputContentTypeDef,  # (2)
    Name: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-braces: ViewInputContentTypeDef](./type_defs.md#viewinputcontenttypedef) 
## UpdateViewContentRequestRequestTypeDef

```python
# UpdateViewContentRequestRequestTypeDef definition

class UpdateViewContentRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    Status: ViewStatusType,  # (1)
    Content: ViewInputContentTypeDef,  # (2)
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-braces: ViewInputContentTypeDef](./type_defs.md#viewinputcontenttypedef) 
## GetFederationTokenResponseTypeDef

```python
# GetFederationTokenResponseTypeDef definition

class GetFederationTokenResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    SignInUrl: str,
    UserArn: str,
    UserId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MediaConcurrencyTypeDef

```python
# MediaConcurrencyTypeDef definition

class MediaConcurrencyTypeDef(TypedDict):
    Channel: ChannelType,  # (1)
    Concurrency: int,
    CrossChannelBehavior: NotRequired[CrossChannelBehaviorTypeDef],  # (2)
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
2. See [:material-code-braces: CrossChannelBehaviorTypeDef](./type_defs.md#crosschannelbehaviortypedef) 
## CurrentMetricDataTypeDef

```python
# CurrentMetricDataTypeDef definition

class CurrentMetricDataTypeDef(TypedDict):
    Metric: NotRequired[CurrentMetricTypeDef],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-braces: CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef) 
## ListDefaultVocabulariesResponseTypeDef

```python
# ListDefaultVocabulariesResponseTypeDef definition

class ListDefaultVocabulariesResponseTypeDef(TypedDict):
    DefaultVocabularyList: List[DefaultVocabularyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DefaultVocabularyTypeDef](./type_defs.md#defaultvocabularytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePromptResponseTypeDef

```python
# DescribePromptResponseTypeDef definition

class DescribePromptResponseTypeDef(TypedDict):
    Prompt: PromptTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPromptsResponseTypeDef

```python
# SearchPromptsResponseTypeDef definition

class SearchPromptsResponseTypeDef(TypedDict):
    Prompts: List[PromptTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptTypeDef](./type_defs.md#prompttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSecurityProfileResponseTypeDef

```python
# DescribeSecurityProfileResponseTypeDef definition

class DescribeSecurityProfileResponseTypeDef(TypedDict):
    SecurityProfile: SecurityProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityProfileTypeDef](./type_defs.md#securityprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrafficDistributionGroupResponseTypeDef

```python
# DescribeTrafficDistributionGroupResponseTypeDef definition

class DescribeTrafficDistributionGroupResponseTypeDef(TypedDict):
    TrafficDistributionGroup: TrafficDistributionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficDistributionGroupTypeDef](./type_defs.md#trafficdistributiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVocabularyResponseTypeDef

```python
# DescribeVocabularyResponseTypeDef definition

class DescribeVocabularyResponseTypeDef(TypedDict):
    Vocabulary: VocabularyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VocabularyTypeDef](./type_defs.md#vocabularytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DimensionsTypeDef

```python
# DimensionsTypeDef definition

class DimensionsTypeDef(TypedDict):
    Queue: NotRequired[QueueReferenceTypeDef],  # (1)
    Channel: NotRequired[ChannelType],  # (2)
    RoutingProfile: NotRequired[RoutingProfileReferenceTypeDef],  # (3)
    RoutingStepExpression: NotRequired[str],
```

1. See [:material-code-braces: QueueReferenceTypeDef](./type_defs.md#queuereferencetypedef) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: RoutingProfileReferenceTypeDef](./type_defs.md#routingprofilereferencetypedef) 
## DisassociateRoutingProfileQueuesRequestRequestTypeDef

```python
# DisassociateRoutingProfileQueuesRequestRequestTypeDef definition

class DisassociateRoutingProfileQueuesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef) 
## RoutingProfileQueueConfigTypeDef

```python
# RoutingProfileQueueConfigTypeDef definition

class RoutingProfileQueueConfigTypeDef(TypedDict):
    QueueReference: RoutingProfileQueueReferenceTypeDef,  # (1)
    Priority: int,
    Delay: int,
```

1. See [:material-code-braces: RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef) 
## DisassociateUserProficienciesRequestRequestTypeDef

```python
# DisassociateUserProficienciesRequestRequestTypeDef definition

class DisassociateUserProficienciesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyDisassociateTypeDef],  # (1)
```

1. See [:material-code-braces: UserProficiencyDisassociateTypeDef](./type_defs.md#userproficiencydisassociatetypedef) 
## StopContactRequestRequestTypeDef

```python
# StopContactRequestRequestTypeDef definition

class StopContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    InstanceId: str,
    DisconnectReason: NotRequired[DisconnectReasonTypeDef],  # (1)
```

1. See [:material-code-braces: DisconnectReasonTypeDef](./type_defs.md#disconnectreasontypedef) 
## KinesisVideoStreamConfigTypeDef

```python
# KinesisVideoStreamConfigTypeDef definition

class KinesisVideoStreamConfigTypeDef(TypedDict):
    Prefix: str,
    RetentionPeriodHours: int,
    EncryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## S3ConfigTypeDef

```python
# S3ConfigTypeDef definition

class S3ConfigTypeDef(TypedDict):
    BucketName: str,
    BucketPrefix: str,
    EncryptionConfig: NotRequired[EncryptionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## EvaluationAnswerInputTypeDef

```python
# EvaluationAnswerInputTypeDef definition

class EvaluationAnswerInputTypeDef(TypedDict):
    Value: NotRequired[EvaluationAnswerDataTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationAnswerDataTypeDef](./type_defs.md#evaluationanswerdatatypedef) 
## EvaluationAnswerOutputTypeDef

```python
# EvaluationAnswerOutputTypeDef definition

class EvaluationAnswerOutputTypeDef(TypedDict):
    Value: NotRequired[EvaluationAnswerDataTypeDef],  # (1)
    SystemSuggestedValue: NotRequired[EvaluationAnswerDataTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationAnswerDataTypeDef](./type_defs.md#evaluationanswerdatatypedef) 
2. See [:material-code-braces: EvaluationAnswerDataTypeDef](./type_defs.md#evaluationanswerdatatypedef) 
## EvaluationFormNumericQuestionAutomationTypeDef

```python
# EvaluationFormNumericQuestionAutomationTypeDef definition

class EvaluationFormNumericQuestionAutomationTypeDef(TypedDict):
    PropertyValue: NotRequired[NumericQuestionPropertyValueAutomationTypeDef],  # (1)
```

1. See [:material-code-braces: NumericQuestionPropertyValueAutomationTypeDef](./type_defs.md#numericquestionpropertyvalueautomationtypedef) 
## EvaluationFormSingleSelectQuestionAutomationOptionTypeDef

```python
# EvaluationFormSingleSelectQuestionAutomationOptionTypeDef definition

class EvaluationFormSingleSelectQuestionAutomationOptionTypeDef(TypedDict):
    RuleCategory: NotRequired[SingleSelectQuestionRuleCategoryAutomationTypeDef],  # (1)
```

1. See [:material-code-braces: SingleSelectQuestionRuleCategoryAutomationTypeDef](./type_defs.md#singleselectquestionrulecategoryautomationtypedef) 
## ListEvaluationFormsResponseTypeDef

```python
# ListEvaluationFormsResponseTypeDef definition

class ListEvaluationFormsResponseTypeDef(TypedDict):
    EvaluationFormSummaryList: List[EvaluationFormSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationFormSummaryTypeDef](./type_defs.md#evaluationformsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEvaluationFormVersionsResponseTypeDef

```python
# ListEvaluationFormVersionsResponseTypeDef definition

class ListEvaluationFormVersionsResponseTypeDef(TypedDict):
    EvaluationFormVersionSummaryList: List[EvaluationFormVersionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationFormVersionSummaryTypeDef](./type_defs.md#evaluationformversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationMetadataTypeDef

```python
# EvaluationMetadataTypeDef definition

class EvaluationMetadataTypeDef(TypedDict):
    ContactId: str,
    EvaluatorArn: str,
    ContactAgentId: NotRequired[str],
    Score: NotRequired[EvaluationScoreTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationScoreTypeDef](./type_defs.md#evaluationscoretypedef) 
## EvaluationSummaryTypeDef

```python
# EvaluationSummaryTypeDef definition

class EvaluationSummaryTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    EvaluationFormTitle: str,
    EvaluationFormId: str,
    Status: EvaluationStatusType,  # (1)
    EvaluatorArn: str,
    CreatedTime: datetime,
    LastModifiedTime: datetime,
    Score: NotRequired[EvaluationScoreTypeDef],  # (2)
```

1. See [:material-code-brackets: EvaluationStatusType](./literals.md#evaluationstatustype) 
2. See [:material-code-braces: EvaluationScoreTypeDef](./type_defs.md#evaluationscoretypedef) 
## FieldValueTypeDef

```python
# FieldValueTypeDef definition

class FieldValueTypeDef(TypedDict):
    Id: str,
    Value: FieldValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) 
## GetCurrentMetricDataRequestRequestTypeDef

```python
# GetCurrentMetricDataRequestRequestTypeDef definition

class GetCurrentMetricDataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Filters: FiltersTypeDef,  # (1)
    CurrentMetrics: Sequence[CurrentMetricTypeDef],  # (2)
    Groupings: NotRequired[Sequence[GroupingType]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortCriteria: NotRequired[Sequence[CurrentMetricSortCriteriaTypeDef]],  # (4)
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: CurrentMetricSortCriteriaTypeDef](./type_defs.md#currentmetricsortcriteriatypedef) 
## ListAgentStatusRequestListAgentStatusesPaginateTypeDef

```python
# ListAgentStatusRequestListAgentStatusesPaginateTypeDef definition

class ListAgentStatusRequestListAgentStatusesPaginateTypeDef(TypedDict):
    InstanceId: str,
    AgentStatusTypes: NotRequired[Sequence[AgentStatusTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef

```python
# ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef definition

class ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBotsRequestListBotsPaginateTypeDef

```python
# ListBotsRequestListBotsPaginateTypeDef definition

class ListBotsRequestListBotsPaginateTypeDef(TypedDict):
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef

```python
# ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef definition

class ListContactEvaluationsRequestListContactEvaluationsPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef

```python
# ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef definition

class ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowModuleState: NotRequired[ContactFlowModuleStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactFlowsRequestListContactFlowsPaginateTypeDef

```python
# ListContactFlowsRequestListContactFlowsPaginateTypeDef definition

class ListContactFlowsRequestListContactFlowsPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowTypes: NotRequired[Sequence[ContactFlowTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactReferencesRequestListContactReferencesPaginateTypeDef

```python
# ListContactReferencesRequestListContactReferencesPaginateTypeDef definition

class ListContactReferencesRequestListContactReferencesPaginateTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef

```python
# ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef definition

class ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef(TypedDict):
    InstanceId: str,
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef

```python
# ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef definition

class ListEvaluationFormVersionsRequestListEvaluationFormVersionsPaginateTypeDef(TypedDict):
    InstanceId: str,
    EvaluationFormId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef

```python
# ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef definition

class ListEvaluationFormsRequestListEvaluationFormsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowAssociationsRequestListFlowAssociationsPaginateTypeDef

```python
# ListFlowAssociationsRequestListFlowAssociationsPaginateTypeDef definition

class ListFlowAssociationsRequestListFlowAssociationsPaginateTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: NotRequired[ListFlowAssociationResourceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef

```python
# ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef definition

class ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef

```python
# ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef definition

class ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef

```python
# ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef definition

class ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesRequestListInstancesPaginateTypeDef

```python
# ListInstancesRequestListInstancesPaginateTypeDef definition

class ListInstancesRequestListInstancesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef

```python
# ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef definition

class ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef(TypedDict):
    InstanceId: str,
    IntegrationType: NotRequired[IntegrationTypeType],  # (1)
    IntegrationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef

```python
# ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef definition

class ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLexBotsRequestListLexBotsPaginateTypeDef

```python
# ListLexBotsRequestListLexBotsPaginateTypeDef definition

class ListLexBotsRequestListLexBotsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef

```python
# ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef definition

class ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef(TypedDict):
    InstanceId: str,
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (1)
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef

```python
# ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef definition

class ListPhoneNumbersV2RequestListPhoneNumbersV2PaginateTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberCountryCodes: NotRequired[Sequence[PhoneNumberCountryCodeType]],  # (1)
    PhoneNumberTypes: NotRequired[Sequence[PhoneNumberTypeType]],  # (2)
    PhoneNumberPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPredefinedAttributesRequestListPredefinedAttributesPaginateTypeDef

```python
# ListPredefinedAttributesRequestListPredefinedAttributesPaginateTypeDef definition

class ListPredefinedAttributesRequestListPredefinedAttributesPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPromptsRequestListPromptsPaginateTypeDef

```python
# ListPromptsRequestListPromptsPaginateTypeDef definition

class ListPromptsRequestListPromptsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef

```python
# ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef definition

class ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef(TypedDict):
    InstanceId: str,
    QueueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestListQueuesPaginateTypeDef

```python
# ListQueuesRequestListQueuesPaginateTypeDef definition

class ListQueuesRequestListQueuesPaginateTypeDef(TypedDict):
    InstanceId: str,
    QueueTypes: NotRequired[Sequence[QueueTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQuickConnectsRequestListQuickConnectsPaginateTypeDef

```python
# ListQuickConnectsRequestListQuickConnectsPaginateTypeDef definition

class ListQuickConnectsRequestListQuickConnectsPaginateTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectTypes: NotRequired[Sequence[QuickConnectTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef

```python
# ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef definition

class ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef

```python
# ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef definition

class ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesRequestListRulesPaginateTypeDef

```python
# ListRulesRequestListRulesPaginateTypeDef definition

class ListRulesRequestListRulesPaginateTypeDef(TypedDict):
    InstanceId: str,
    PublishStatus: NotRequired[RulePublishStatusType],  # (1)
    EventSourceName: NotRequired[EventSourceNameType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityKeysRequestListSecurityKeysPaginateTypeDef

```python
# ListSecurityKeysRequestListSecurityKeysPaginateTypeDef definition

class ListSecurityKeysRequestListSecurityKeysPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfileApplicationsRequestListSecurityProfileApplicationsPaginateTypeDef

```python
# ListSecurityProfileApplicationsRequestListSecurityProfileApplicationsPaginateTypeDef definition

class ListSecurityProfileApplicationsRequestListSecurityProfileApplicationsPaginateTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef

```python
# ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef definition

class ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef(TypedDict):
    SecurityProfileId: str,
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef

```python
# ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef definition

class ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef

```python
# ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef definition

class ListTaskTemplatesRequestListTaskTemplatesPaginateTypeDef(TypedDict):
    InstanceId: str,
    Status: NotRequired[TaskTemplateStatusType],  # (1)
    Name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrafficDistributionGroupUsersRequestListTrafficDistributionGroupUsersPaginateTypeDef

```python
# ListTrafficDistributionGroupUsersRequestListTrafficDistributionGroupUsersPaginateTypeDef definition

class ListTrafficDistributionGroupUsersRequestListTrafficDistributionGroupUsersPaginateTypeDef(TypedDict):
    TrafficDistributionGroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef

```python
# ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef definition

class ListTrafficDistributionGroupsRequestListTrafficDistributionGroupsPaginateTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUseCasesRequestListUseCasesPaginateTypeDef

```python
# ListUseCasesRequestListUseCasesPaginateTypeDef definition

class ListUseCasesRequestListUseCasesPaginateTypeDef(TypedDict):
    InstanceId: str,
    IntegrationAssociationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef

```python
# ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef definition

class ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserProficienciesRequestListUserProficienciesPaginateTypeDef

```python
# ListUserProficienciesRequestListUserProficienciesPaginateTypeDef definition

class ListUserProficienciesRequestListUserProficienciesPaginateTypeDef(TypedDict):
    InstanceId: str,
    UserId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestListUsersPaginateTypeDef

```python
# ListUsersRequestListUsersPaginateTypeDef definition

class ListUsersRequestListUsersPaginateTypeDef(TypedDict):
    InstanceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViewVersionsRequestListViewVersionsPaginateTypeDef

```python
# ListViewVersionsRequestListViewVersionsPaginateTypeDef definition

class ListViewVersionsRequestListViewVersionsPaginateTypeDef(TypedDict):
    InstanceId: str,
    ViewId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViewsRequestListViewsPaginateTypeDef

```python
# ListViewsRequestListViewsPaginateTypeDef definition

class ListViewsRequestListViewsPaginateTypeDef(TypedDict):
    InstanceId: str,
    Type: NotRequired[ViewTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef

```python
# SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef definition

class SearchAvailablePhoneNumbersRequestSearchAvailablePhoneNumbersPaginateTypeDef(TypedDict):
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    TargetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    PhoneNumberPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef

```python
# SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef definition

class SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef(TypedDict):
    InstanceId: str,
    State: NotRequired[VocabularyStateType],  # (1)
    NameStartsWith: NotRequired[str],
    LanguageCode: NotRequired[VocabularyLanguageCodeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchContactsTimeRangeTypeDef

```python
# SearchContactsTimeRangeTypeDef definition

class SearchContactsTimeRangeTypeDef(TypedDict):
    Type: SearchContactsTimeRangeTypeType,  # (1)
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
```

1. See [:material-code-brackets: SearchContactsTimeRangeTypeType](./literals.md#searchcontactstimerangetypetype) 
## UpdateContactScheduleRequestRequestTypeDef

```python
# UpdateContactScheduleRequestRequestTypeDef definition

class UpdateContactScheduleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ScheduledTime: Union[datetime, str],
```

## HierarchyPathReferenceTypeDef

```python
# HierarchyPathReferenceTypeDef definition

class HierarchyPathReferenceTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyGroupSummaryReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
2. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
3. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
4. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
5. See [:material-code-braces: HierarchyGroupSummaryReferenceTypeDef](./type_defs.md#hierarchygroupsummaryreferencetypedef) 
## HierarchyPathTypeDef

```python
# HierarchyPathTypeDef definition

class HierarchyPathTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyGroupSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
2. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
3. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
4. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
5. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
## ListUserHierarchyGroupsResponseTypeDef

```python
# ListUserHierarchyGroupsResponseTypeDef definition

class ListUserHierarchyGroupsResponseTypeDef(TypedDict):
    UserHierarchyGroupSummaryList: List[HierarchyGroupSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HierarchyStructureTypeDef

```python
# HierarchyStructureTypeDef definition

class HierarchyStructureTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyLevelTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyLevelTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
2. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
3. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
4. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
5. See [:material-code-braces: HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef) 
## HierarchyStructureUpdateTypeDef

```python
# HierarchyStructureUpdateTypeDef definition

class HierarchyStructureUpdateTypeDef(TypedDict):
    LevelOne: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelTwo: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelThree: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelFour: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
    LevelFive: NotRequired[HierarchyLevelUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
2. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
3. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
4. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
5. See [:material-code-braces: HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef) 
## HistoricalMetricTypeDef

```python
# HistoricalMetricTypeDef definition

class HistoricalMetricTypeDef(TypedDict):
    Name: NotRequired[HistoricalMetricNameType],  # (1)
    Threshold: NotRequired[ThresholdTypeDef],  # (2)
    Statistic: NotRequired[StatisticType],  # (3)
    Unit: NotRequired[UnitType],  # (4)
```

1. See [:material-code-brackets: HistoricalMetricNameType](./literals.md#historicalmetricnametype) 
2. See [:material-code-braces: ThresholdTypeDef](./type_defs.md#thresholdtypedef) 
3. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
4. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## HoursOfOperationConfigTypeDef

```python
# HoursOfOperationConfigTypeDef definition

class HoursOfOperationConfigTypeDef(TypedDict):
    Day: HoursOfOperationDaysType,  # (1)
    StartTime: HoursOfOperationTimeSliceTypeDef,  # (2)
    EndTime: HoursOfOperationTimeSliceTypeDef,  # (2)
```

1. See [:material-code-brackets: HoursOfOperationDaysType](./literals.md#hoursofoperationdaystype) 
2. See [:material-code-braces: HoursOfOperationTimeSliceTypeDef](./type_defs.md#hoursofoperationtimeslicetypedef) 
3. See [:material-code-braces: HoursOfOperationTimeSliceTypeDef](./type_defs.md#hoursofoperationtimeslicetypedef) 
## HoursOfOperationSearchCriteriaTypeDef

```python
# HoursOfOperationSearchCriteriaTypeDef definition

class HoursOfOperationSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## PredefinedAttributeSearchCriteriaTypeDef

```python
# PredefinedAttributeSearchCriteriaTypeDef definition

class PredefinedAttributeSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## PromptSearchCriteriaTypeDef

```python
# PromptSearchCriteriaTypeDef definition

class PromptSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## QueueSearchCriteriaTypeDef

```python
# QueueSearchCriteriaTypeDef definition

class QueueSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    QueueTypeCondition: NotRequired[SearchableQueueTypeType],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-brackets: SearchableQueueTypeType](./literals.md#searchablequeuetypetype) 
## QuickConnectSearchCriteriaTypeDef

```python
# QuickConnectSearchCriteriaTypeDef definition

class QuickConnectSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## RoutingProfileSearchCriteriaTypeDef

```python
# RoutingProfileSearchCriteriaTypeDef definition

class RoutingProfileSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## SecurityProfileSearchCriteriaTypeDef

```python
# SecurityProfileSearchCriteriaTypeDef definition

class SecurityProfileSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## UserSearchCriteriaTypeDef

```python
# UserSearchCriteriaTypeDef definition

class UserSearchCriteriaTypeDef(TypedDict):
    OrConditions: NotRequired[Sequence[Dict[str, Any]]],
    AndConditions: NotRequired[Sequence[Dict[str, Any]]],
    StringCondition: NotRequired[StringConditionTypeDef],  # (1)
    HierarchyGroupCondition: NotRequired[HierarchyGroupConditionTypeDef],  # (2)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: HierarchyGroupConditionTypeDef](./type_defs.md#hierarchygroupconditiontypedef) 
## ListHoursOfOperationsResponseTypeDef

```python
# ListHoursOfOperationsResponseTypeDef definition

class ListHoursOfOperationsResponseTypeDef(TypedDict):
    HoursOfOperationSummaryList: List[HoursOfOperationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HoursOfOperationSummaryTypeDef](./type_defs.md#hoursofoperationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    IdentityManagementType: NotRequired[DirectoryTypeType],  # (1)
    InstanceAlias: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    ServiceRole: NotRequired[str],
    InstanceStatus: NotRequired[InstanceStatusType],  # (2)
    StatusReason: NotRequired[InstanceStatusReasonTypeDef],  # (3)
    InboundCallsEnabled: NotRequired[bool],
    OutboundCallsEnabled: NotRequired[bool],
    InstanceAccessUrl: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
2. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
3. See [:material-code-braces: InstanceStatusReasonTypeDef](./type_defs.md#instancestatusreasontypedef) 
## ListInstancesResponseTypeDef

```python
# ListInstancesResponseTypeDef definition

class ListInstancesResponseTypeDef(TypedDict):
    InstanceSummaryList: List[InstanceSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIntegrationAssociationsResponseTypeDef

```python
# ListIntegrationAssociationsResponseTypeDef definition

class ListIntegrationAssociationsResponseTypeDef(TypedDict):
    IntegrationAssociationSummaryList: List[IntegrationAssociationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntegrationAssociationSummaryTypeDef](./type_defs.md#integrationassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvisibleFieldInfoTypeDef

```python
# InvisibleFieldInfoTypeDef definition

class InvisibleFieldInfoTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## ReadOnlyFieldInfoTypeDef

```python
# ReadOnlyFieldInfoTypeDef definition

class ReadOnlyFieldInfoTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## RequiredFieldInfoTypeDef

```python
# RequiredFieldInfoTypeDef definition

class RequiredFieldInfoTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## TaskTemplateDefaultFieldValueTypeDef

```python
# TaskTemplateDefaultFieldValueTypeDef definition

class TaskTemplateDefaultFieldValueTypeDef(TypedDict):
    Id: NotRequired[TaskTemplateFieldIdentifierTypeDef],  # (1)
    DefaultValue: NotRequired[str],
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
## TaskTemplateFieldTypeDef

```python
# TaskTemplateFieldTypeDef definition

class TaskTemplateFieldTypeDef(TypedDict):
    Id: TaskTemplateFieldIdentifierTypeDef,  # (1)
    Description: NotRequired[str],
    Type: NotRequired[TaskTemplateFieldTypeType],  # (2)
    SingleSelectOptions: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TaskTemplateFieldIdentifierTypeDef](./type_defs.md#tasktemplatefieldidentifiertypedef) 
2. See [:material-code-brackets: TaskTemplateFieldTypeType](./literals.md#tasktemplatefieldtypetype) 
## ListPhoneNumbersResponseTypeDef

```python
# ListPhoneNumbersResponseTypeDef definition

class ListPhoneNumbersResponseTypeDef(TypedDict):
    PhoneNumberSummaryList: List[PhoneNumberSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PhoneNumberSummaryTypeDef](./type_defs.md#phonenumbersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumbersV2ResponseTypeDef

```python
# ListPhoneNumbersV2ResponseTypeDef definition

class ListPhoneNumbersV2ResponseTypeDef(TypedDict):
    NextToken: str,
    ListPhoneNumbersSummaryList: List[ListPhoneNumbersSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListPhoneNumbersSummaryTypeDef](./type_defs.md#listphonenumberssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPredefinedAttributesResponseTypeDef

```python
# ListPredefinedAttributesResponseTypeDef definition

class ListPredefinedAttributesResponseTypeDef(TypedDict):
    NextToken: str,
    PredefinedAttributeSummaryList: List[PredefinedAttributeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredefinedAttributeSummaryTypeDef](./type_defs.md#predefinedattributesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPromptsResponseTypeDef

```python
# ListPromptsResponseTypeDef definition

class ListPromptsResponseTypeDef(TypedDict):
    PromptSummaryList: List[PromptSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptSummaryTypeDef](./type_defs.md#promptsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueQuickConnectsResponseTypeDef

```python
# ListQueueQuickConnectsResponseTypeDef definition

class ListQueueQuickConnectsResponseTypeDef(TypedDict):
    NextToken: str,
    QuickConnectSummaryList: List[QuickConnectSummaryTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickConnectSummaryTypeDef](./type_defs.md#quickconnectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQuickConnectsResponseTypeDef

```python
# ListQuickConnectsResponseTypeDef definition

class ListQuickConnectsResponseTypeDef(TypedDict):
    QuickConnectSummaryList: List[QuickConnectSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickConnectSummaryTypeDef](./type_defs.md#quickconnectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    QueueSummaryList: List[QueueSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutingProfileQueuesResponseTypeDef

```python
# ListRoutingProfileQueuesResponseTypeDef definition

class ListRoutingProfileQueuesResponseTypeDef(TypedDict):
    NextToken: str,
    RoutingProfileQueueConfigSummaryList: List[RoutingProfileQueueConfigSummaryTypeDef],  # (1)
    LastModifiedTime: datetime,
    LastModifiedRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutingProfileQueueConfigSummaryTypeDef](./type_defs.md#routingprofilequeueconfigsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutingProfilesResponseTypeDef

```python
# ListRoutingProfilesResponseTypeDef definition

class ListRoutingProfilesResponseTypeDef(TypedDict):
    RoutingProfileSummaryList: List[RoutingProfileSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutingProfileSummaryTypeDef](./type_defs.md#routingprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityKeysResponseTypeDef

```python
# ListSecurityKeysResponseTypeDef definition

class ListSecurityKeysResponseTypeDef(TypedDict):
    SecurityKeys: List[SecurityKeyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityKeyTypeDef](./type_defs.md#securitykeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityProfilesResponseTypeDef

```python
# ListSecurityProfilesResponseTypeDef definition

class ListSecurityProfilesResponseTypeDef(TypedDict):
    SecurityProfileSummaryList: List[SecurityProfileSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityProfileSummaryTypeDef](./type_defs.md#securityprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskTemplatesResponseTypeDef

```python
# ListTaskTemplatesResponseTypeDef definition

class ListTaskTemplatesResponseTypeDef(TypedDict):
    TaskTemplates: List[TaskTemplateMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskTemplateMetadataTypeDef](./type_defs.md#tasktemplatemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficDistributionGroupUsersResponseTypeDef

```python
# ListTrafficDistributionGroupUsersResponseTypeDef definition

class ListTrafficDistributionGroupUsersResponseTypeDef(TypedDict):
    NextToken: str,
    TrafficDistributionGroupUserSummaryList: List[TrafficDistributionGroupUserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficDistributionGroupUserSummaryTypeDef](./type_defs.md#trafficdistributiongroupusersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficDistributionGroupsResponseTypeDef

```python
# ListTrafficDistributionGroupsResponseTypeDef definition

class ListTrafficDistributionGroupsResponseTypeDef(TypedDict):
    NextToken: str,
    TrafficDistributionGroupSummaryList: List[TrafficDistributionGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficDistributionGroupSummaryTypeDef](./type_defs.md#trafficdistributiongroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUseCasesResponseTypeDef

```python
# ListUseCasesResponseTypeDef definition

class ListUseCasesResponseTypeDef(TypedDict):
    UseCaseSummaryList: List[UseCaseTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UseCaseTypeDef](./type_defs.md#usecasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    UserSummaryList: List[UserSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViewVersionsResponseTypeDef

```python
# ListViewVersionsResponseTypeDef definition

class ListViewVersionsResponseTypeDef(TypedDict):
    ViewVersionSummaryList: List[ViewVersionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewVersionSummaryTypeDef](./type_defs.md#viewversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViewsResponseTypeDef

```python
# ListViewsResponseTypeDef definition

class ListViewsResponseTypeDef(TypedDict):
    ViewsSummaryList: List[ViewSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewSummaryTypeDef](./type_defs.md#viewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricV2TypeDef

```python
# MetricV2TypeDef definition

class MetricV2TypeDef(TypedDict):
    Name: NotRequired[str],
    Threshold: NotRequired[Sequence[ThresholdV2TypeDef]],  # (1)
    MetricFilters: NotRequired[Sequence[MetricFilterV2TypeDef]],  # (2)
```

1. See [:material-code-braces: ThresholdV2TypeDef](./type_defs.md#thresholdv2typedef) 
2. See [:material-code-braces: MetricFilterV2TypeDef](./type_defs.md#metricfilterv2typedef) 
## NewSessionDetailsTypeDef

```python
# NewSessionDetailsTypeDef definition

class NewSessionDetailsTypeDef(TypedDict):
    SupportedMessagingContentTypes: NotRequired[Sequence[str]],
    ParticipantDetails: NotRequired[ParticipantDetailsTypeDef],  # (1)
    Attributes: NotRequired[Mapping[str, str]],
    StreamingConfiguration: NotRequired[ChatStreamingConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef) 
## SendNotificationActionDefinitionTypeDef

```python
# SendNotificationActionDefinitionTypeDef definition

class SendNotificationActionDefinitionTypeDef(TypedDict):
    DeliveryMethod: NotificationDeliveryTypeType,  # (1)
    Content: str,
    ContentType: NotificationContentTypeType,  # (2)
    Recipient: NotificationRecipientTypeTypeDef,  # (3)
    Subject: NotRequired[str],
```

1. See [:material-code-brackets: NotificationDeliveryTypeType](./literals.md#notificationdeliverytypetype) 
2. See [:material-code-brackets: NotificationContentTypeType](./literals.md#notificationcontenttypetype) 
3. See [:material-code-braces: NotificationRecipientTypeTypeDef](./type_defs.md#notificationrecipienttypetypedef) 
## ParticipantTimerConfigurationTypeDef

```python
# ParticipantTimerConfigurationTypeDef definition

class ParticipantTimerConfigurationTypeDef(TypedDict):
    ParticipantRole: TimerEligibleParticipantRolesType,  # (1)
    TimerType: ParticipantTimerTypeType,  # (2)
    TimerValue: ParticipantTimerValueTypeDef,  # (3)
```

1. See [:material-code-brackets: TimerEligibleParticipantRolesType](./literals.md#timereligibleparticipantrolestype) 
2. See [:material-code-brackets: ParticipantTimerTypeType](./literals.md#participanttimertypetype) 
3. See [:material-code-braces: ParticipantTimerValueTypeDef](./type_defs.md#participanttimervaluetypedef) 
## PredefinedAttributePaginatorTypeDef

```python
# PredefinedAttributePaginatorTypeDef definition

class PredefinedAttributePaginatorTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[PredefinedAttributeValuesPaginatorTypeDef],  # (1)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: PredefinedAttributeValuesPaginatorTypeDef](./type_defs.md#predefinedattributevaluespaginatortypedef) 
## QuickConnectConfigTypeDef

```python
# QuickConnectConfigTypeDef definition

class QuickConnectConfigTypeDef(TypedDict):
    QuickConnectType: QuickConnectTypeType,  # (1)
    UserConfig: NotRequired[UserQuickConnectConfigTypeDef],  # (2)
    QueueConfig: NotRequired[QueueQuickConnectConfigTypeDef],  # (3)
    PhoneConfig: NotRequired[PhoneNumberQuickConnectConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
2. See [:material-code-braces: UserQuickConnectConfigTypeDef](./type_defs.md#userquickconnectconfigtypedef) 
3. See [:material-code-braces: QueueQuickConnectConfigTypeDef](./type_defs.md#queuequickconnectconfigtypedef) 
4. See [:material-code-braces: PhoneNumberQuickConnectConfigTypeDef](./type_defs.md#phonenumberquickconnectconfigtypedef) 
## RealTimeContactAnalysisTranscriptItemRedactionTypeDef

```python
# RealTimeContactAnalysisTranscriptItemRedactionTypeDef definition

class RealTimeContactAnalysisTranscriptItemRedactionTypeDef(TypedDict):
    CharacterOffsets: NotRequired[List[RealTimeContactAnalysisCharacterIntervalTypeDef]],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCharacterIntervalTypeDef](./type_defs.md#realtimecontactanalysischaracterintervaltypedef) 
## RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef

```python
# RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef definition

class RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef(TypedDict):
    Id: str,
    CharacterOffsets: NotRequired[RealTimeContactAnalysisCharacterIntervalTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCharacterIntervalTypeDef](./type_defs.md#realtimecontactanalysischaracterintervaltypedef) 
## RealTimeContactAnalysisTranscriptItemWithContentTypeDef

```python
# RealTimeContactAnalysisTranscriptItemWithContentTypeDef definition

class RealTimeContactAnalysisTranscriptItemWithContentTypeDef(TypedDict):
    Id: str,
    Content: NotRequired[str],
    CharacterOffsets: NotRequired[RealTimeContactAnalysisCharacterIntervalTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCharacterIntervalTypeDef](./type_defs.md#realtimecontactanalysischaracterintervaltypedef) 
## RealTimeContactAnalysisSegmentAttachmentsTypeDef

```python
# RealTimeContactAnalysisSegmentAttachmentsTypeDef definition

class RealTimeContactAnalysisSegmentAttachmentsTypeDef(TypedDict):
    Id: str,
    ParticipantId: str,
    ParticipantRole: ParticipantRoleType,  # (1)
    Attachments: List[RealTimeContactAnalysisAttachmentTypeDef],  # (2)
    Time: RealTimeContactAnalysisTimeDataTypeDef,  # (3)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: RealTimeContactAnalysisAttachmentTypeDef](./type_defs.md#realtimecontactanalysisattachmenttypedef) 
3. See [:material-code-braces: RealTimeContactAnalysisTimeDataTypeDef](./type_defs.md#realtimecontactanalysistimedatatypedef) 
## RealTimeContactAnalysisSegmentEventTypeDef

```python
# RealTimeContactAnalysisSegmentEventTypeDef definition

class RealTimeContactAnalysisSegmentEventTypeDef(TypedDict):
    Id: str,
    EventType: str,
    Time: RealTimeContactAnalysisTimeDataTypeDef,  # (2)
    ParticipantId: NotRequired[str],
    ParticipantRole: NotRequired[ParticipantRoleType],  # (1)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: RealTimeContactAnalysisTimeDataTypeDef](./type_defs.md#realtimecontactanalysistimedatatypedef) 
## ReferenceSummaryTypeDef

```python
# ReferenceSummaryTypeDef definition

class ReferenceSummaryTypeDef(TypedDict):
    Url: NotRequired[UrlReferenceTypeDef],  # (1)
    Attachment: NotRequired[AttachmentReferenceTypeDef],  # (2)
    String: NotRequired[StringReferenceTypeDef],  # (3)
    Number: NotRequired[NumberReferenceTypeDef],  # (4)
    Date: NotRequired[DateReferenceTypeDef],  # (5)
    Email: NotRequired[EmailReferenceTypeDef],  # (6)
```

1. See [:material-code-braces: UrlReferenceTypeDef](./type_defs.md#urlreferencetypedef) 
2. See [:material-code-braces: AttachmentReferenceTypeDef](./type_defs.md#attachmentreferencetypedef) 
3. See [:material-code-braces: StringReferenceTypeDef](./type_defs.md#stringreferencetypedef) 
4. See [:material-code-braces: NumberReferenceTypeDef](./type_defs.md#numberreferencetypedef) 
5. See [:material-code-braces: DateReferenceTypeDef](./type_defs.md#datereferencetypedef) 
6. See [:material-code-braces: EmailReferenceTypeDef](./type_defs.md#emailreferencetypedef) 
## StartOutboundVoiceContactRequestRequestTypeDef

```python
# StartOutboundVoiceContactRequestRequestTypeDef definition

class StartOutboundVoiceContactRequestRequestTypeDef(TypedDict):
    DestinationPhoneNumber: str,
    ContactFlowId: str,
    InstanceId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
    RelatedContactId: NotRequired[str],
    ClientToken: NotRequired[str],
    SourcePhoneNumber: NotRequired[str],
    QueueId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    AnswerMachineDetectionConfig: NotRequired[AnswerMachineDetectionConfigTypeDef],  # (2)
    CampaignId: NotRequired[str],
    TrafficType: NotRequired[TrafficTypeType],  # (3)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
3. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
## StartTaskContactRequestRequestTypeDef

```python
# StartTaskContactRequestRequestTypeDef definition

class StartTaskContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    PreviousContactId: NotRequired[str],
    ContactFlowId: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    ScheduledTime: NotRequired[Union[datetime, str]],
    TaskTemplateId: NotRequired[str],
    QuickConnectId: NotRequired[str],
    RelatedContactId: NotRequired[str],
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## TaskActionDefinitionTypeDef

```python
# TaskActionDefinitionTypeDef definition

class TaskActionDefinitionTypeDef(TypedDict):
    Name: str,
    ContactFlowId: str,
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## UpdateContactRequestRequestTypeDef

```python
# UpdateContactRequestRequestTypeDef definition

class UpdateContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## ResourceTagsSearchCriteriaTypeDef

```python
# ResourceTagsSearchCriteriaTypeDef definition

class ResourceTagsSearchCriteriaTypeDef(TypedDict):
    TagSearchCondition: NotRequired[TagSearchConditionTypeDef],  # (1)
```

1. See [:material-code-braces: TagSearchConditionTypeDef](./type_defs.md#tagsearchconditiontypedef) 
## SearchResourceTagsResponseTypeDef

```python
# SearchResourceTagsResponseTypeDef definition

class SearchResourceTagsResponseTypeDef(TypedDict):
    Tags: List[TagSetTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagSetTypeDef](./type_defs.md#tagsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchSecurityProfilesResponseTypeDef

```python
# SearchSecurityProfilesResponseTypeDef definition

class SearchSecurityProfilesResponseTypeDef(TypedDict):
    SecurityProfiles: List[SecurityProfileSearchSummaryTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityProfileSearchSummaryTypeDef](./type_defs.md#securityprofilesearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchVocabulariesResponseTypeDef

```python
# SearchVocabulariesResponseTypeDef definition

class SearchVocabulariesResponseTypeDef(TypedDict):
    VocabularySummaryList: List[VocabularySummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VocabularySummaryTypeDef](./type_defs.md#vocabularysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchableContactAttributesTypeDef

```python
# SearchableContactAttributesTypeDef definition

class SearchableContactAttributesTypeDef(TypedDict):
    Criteria: Sequence[SearchableContactAttributesCriteriaTypeDef],  # (1)
    MatchType: NotRequired[SearchContactsMatchTypeType],  # (2)
```

1. See [:material-code-braces: SearchableContactAttributesCriteriaTypeDef](./type_defs.md#searchablecontactattributescriteriatypedef) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## StartChatContactRequestRequestTypeDef

```python
# StartChatContactRequestRequestTypeDef definition

class StartChatContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactFlowId: str,
    ParticipantDetails: ParticipantDetailsTypeDef,  # (1)
    Attributes: NotRequired[Mapping[str, str]],
    InitialMessage: NotRequired[ChatMessageTypeDef],  # (2)
    ClientToken: NotRequired[str],
    ChatDurationInMinutes: NotRequired[int],
    SupportedMessagingContentTypes: NotRequired[Sequence[str]],
    PersistentChat: NotRequired[PersistentChatTypeDef],  # (3)
    RelatedContactId: NotRequired[str],
    SegmentAttributes: NotRequired[Mapping[str, SegmentAttributeValueTypeDef]],  # (4)
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: ChatMessageTypeDef](./type_defs.md#chatmessagetypedef) 
3. See [:material-code-braces: PersistentChatTypeDef](./type_defs.md#persistentchattypedef) 
4. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
## SignInConfigTypeDef

```python
# SignInConfigTypeDef definition

class SignInConfigTypeDef(TypedDict):
    Distributions: List[SignInDistributionTypeDef],  # (1)
```

1. See [:material-code-braces: SignInDistributionTypeDef](./type_defs.md#signindistributiontypedef) 
## StartContactRecordingRequestRequestTypeDef

```python
# StartContactRecordingRequestRequestTypeDef definition

class StartContactRecordingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: VoiceRecordingConfigurationTypeDef](./type_defs.md#voicerecordingconfigurationtypedef) 
## TranscriptTypeDef

```python
# TranscriptTypeDef definition

class TranscriptTypeDef(TypedDict):
    Criteria: Sequence[TranscriptCriteriaTypeDef],  # (1)
    MatchType: NotRequired[SearchContactsMatchTypeType],  # (2)
```

1. See [:material-code-braces: TranscriptCriteriaTypeDef](./type_defs.md#transcriptcriteriatypedef) 
2. See [:material-code-brackets: SearchContactsMatchTypeType](./literals.md#searchcontactsmatchtypetype) 
## UserSearchSummaryTypeDef

```python
# UserSearchSummaryTypeDef definition

class UserSearchSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    DirectoryUserId: NotRequired[str],
    HierarchyGroupId: NotRequired[str],
    Id: NotRequired[str],
    IdentityInfo: NotRequired[UserIdentityInfoLiteTypeDef],  # (1)
    PhoneConfig: NotRequired[UserPhoneConfigTypeDef],  # (2)
    RoutingProfileId: NotRequired[str],
    SecurityProfileIds: NotRequired[List[str]],
    Tags: NotRequired[Dict[str, str]],
    Username: NotRequired[str],
```

1. See [:material-code-braces: UserIdentityInfoLiteTypeDef](./type_defs.md#useridentityinfolitetypedef) 
2. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
## ViewTypeDef

```python
# ViewTypeDef definition

class ViewTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ViewStatusType],  # (1)
    Type: NotRequired[ViewTypeType],  # (2)
    Description: NotRequired[str],
    Version: NotRequired[int],
    VersionDescription: NotRequired[str],
    Content: NotRequired[ViewContentTypeDef],  # (3)
    Tags: NotRequired[Dict[str, str]],
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    ViewContentSha256: NotRequired[str],
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
3. See [:material-code-braces: ViewContentTypeDef](./type_defs.md#viewcontenttypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    RuleSummaryList: List[RuleSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWebRTCContactRequestRequestTypeDef

```python
# StartWebRTCContactRequestRequestTypeDef definition

class StartWebRTCContactRequestRequestTypeDef(TypedDict):
    ContactFlowId: str,
    InstanceId: str,
    ParticipantDetails: ParticipantDetailsTypeDef,  # (1)
    Attributes: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
    AllowedCapabilities: NotRequired[AllowedCapabilitiesTypeDef],  # (2)
    RelatedContactId: NotRequired[str],
    References: NotRequired[Mapping[str, ReferenceTypeDef]],  # (3)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: AllowedCapabilitiesTypeDef](./type_defs.md#allowedcapabilitiestypedef) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
## ListBotsResponseTypeDef

```python
# ListBotsResponseTypeDef definition

class ListBotsResponseTypeDef(TypedDict):
    LexBots: List[LexBotConfigTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LexBotConfigTypeDef](./type_defs.md#lexbotconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MeetingTypeDef

```python
# MeetingTypeDef definition

class MeetingTypeDef(TypedDict):
    MediaRegion: NotRequired[str],
    MediaPlacement: NotRequired[MediaPlacementTypeDef],  # (1)
    MeetingFeatures: NotRequired[MeetingFeaturesConfigurationTypeDef],  # (2)
    MeetingId: NotRequired[str],
```

1. See [:material-code-braces: MediaPlacementTypeDef](./type_defs.md#mediaplacementtypedef) 
2. See [:material-code-braces: MeetingFeaturesConfigurationTypeDef](./type_defs.md#meetingfeaturesconfigurationtypedef) 
## DescribePhoneNumberResponseTypeDef

```python
# DescribePhoneNumberResponseTypeDef definition

class DescribePhoneNumberResponseTypeDef(TypedDict):
    ClaimedPhoneNumberSummary: ClaimedPhoneNumberSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClaimedPhoneNumberSummaryTypeDef](./type_defs.md#claimedphonenumbersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutContactRequestRequestTypeDef

```python
# BatchPutContactRequestRequestTypeDef definition

class BatchPutContactRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactDataRequestList: Sequence[ContactDataRequestTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ContactDataRequestTypeDef](./type_defs.md#contactdatarequesttypedef) 
## GetCurrentUserDataRequestRequestTypeDef

```python
# GetCurrentUserDataRequestRequestTypeDef definition

class GetCurrentUserDataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Filters: UserDataFiltersTypeDef,  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: UserDataFiltersTypeDef](./type_defs.md#userdatafilterstypedef) 
## SearchContactsResponseTypeDef

```python
# SearchContactsResponseTypeDef definition

class SearchContactsResponseTypeDef(TypedDict):
    Contacts: List[ContactSearchSummaryTypeDef],  # (1)
    NextToken: str,
    TotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactSearchSummaryTypeDef](./type_defs.md#contactsearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContactResponseTypeDef

```python
# DescribeContactResponseTypeDef definition

class DescribeContactResponseTypeDef(TypedDict):
    Contact: ContactTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HoursOfOperationSearchFilterTypeDef

```python
# HoursOfOperationSearchFilterTypeDef definition

class HoursOfOperationSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## PromptSearchFilterTypeDef

```python
# PromptSearchFilterTypeDef definition

class PromptSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## QueueSearchFilterTypeDef

```python
# QueueSearchFilterTypeDef definition

class QueueSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## QuickConnectSearchFilterTypeDef

```python
# QuickConnectSearchFilterTypeDef definition

class QuickConnectSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## RoutingProfileSearchFilterTypeDef

```python
# RoutingProfileSearchFilterTypeDef definition

class RoutingProfileSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## SecurityProfilesSearchFilterTypeDef

```python
# SecurityProfilesSearchFilterTypeDef definition

class SecurityProfilesSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## UserSearchFilterTypeDef

```python
# UserSearchFilterTypeDef definition

class UserSearchFilterTypeDef(TypedDict):
    TagFilter: NotRequired[ControlPlaneTagFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlaneTagFilterTypeDef](./type_defs.md#controlplanetagfiltertypedef) 
## DescribeEvaluationFormResponseTypeDef

```python
# DescribeEvaluationFormResponseTypeDef definition

class DescribeEvaluationFormResponseTypeDef(TypedDict):
    EvaluationForm: EvaluationFormTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationFormTypeDef](./type_defs.md#evaluationformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePredefinedAttributeResponseTypeDef

```python
# DescribePredefinedAttributeResponseTypeDef definition

class DescribePredefinedAttributeResponseTypeDef(TypedDict):
    PredefinedAttribute: PredefinedAttributeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredefinedAttributeTypeDef](./type_defs.md#predefinedattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPredefinedAttributesResponseTypeDef

```python
# SearchPredefinedAttributesResponseTypeDef definition

class SearchPredefinedAttributesResponseTypeDef(TypedDict):
    PredefinedAttributes: List[PredefinedAttributeTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredefinedAttributeTypeDef](./type_defs.md#predefinedattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeQueueResponseTypeDef

```python
# DescribeQueueResponseTypeDef definition

class DescribeQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchQueuesResponseTypeDef

```python
# SearchQueuesResponseTypeDef definition

class SearchQueuesResponseTypeDef(TypedDict):
    Queues: List[QueueTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResponseTypeDef

```python
# DescribeUserResponseTypeDef definition

class DescribeUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoutingProfileTypeDef

```python
# RoutingProfileTypeDef definition

class RoutingProfileTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    Name: NotRequired[str],
    RoutingProfileArn: NotRequired[str],
    RoutingProfileId: NotRequired[str],
    Description: NotRequired[str],
    MediaConcurrencies: NotRequired[List[MediaConcurrencyTypeDef]],  # (1)
    DefaultOutboundQueueId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    NumberOfAssociatedQueues: NotRequired[int],
    NumberOfAssociatedUsers: NotRequired[int],
    AgentAvailabilityTimer: NotRequired[AgentAvailabilityTimerType],  # (2)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
    IsDefault: NotRequired[bool],
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
2. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
## UpdateRoutingProfileConcurrencyRequestRequestTypeDef

```python
# UpdateRoutingProfileConcurrencyRequestRequestTypeDef definition

class UpdateRoutingProfileConcurrencyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],  # (1)
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
## CurrentMetricResultTypeDef

```python
# CurrentMetricResultTypeDef definition

class CurrentMetricResultTypeDef(TypedDict):
    Dimensions: NotRequired[DimensionsTypeDef],  # (1)
    Collections: NotRequired[List[CurrentMetricDataTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionsTypeDef](./type_defs.md#dimensionstypedef) 
2. See [:material-code-braces: CurrentMetricDataTypeDef](./type_defs.md#currentmetricdatatypedef) 
## AssociateRoutingProfileQueuesRequestRequestTypeDef

```python
# AssociateRoutingProfileQueuesRequestRequestTypeDef definition

class AssociateRoutingProfileQueuesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
## CreateRoutingProfileRequestRequestTypeDef

```python
# CreateRoutingProfileRequestRequestTypeDef definition

class CreateRoutingProfileRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Description: str,
    DefaultOutboundQueueId: str,
    MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],  # (1)
    QueueConfigs: NotRequired[Sequence[RoutingProfileQueueConfigTypeDef]],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    AgentAvailabilityTimer: NotRequired[AgentAvailabilityTimerType],  # (3)
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
2. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
3. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
## UpdateRoutingProfileQueuesRequestRequestTypeDef

```python
# UpdateRoutingProfileQueuesRequestRequestTypeDef definition

class UpdateRoutingProfileQueuesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    RoutingProfileId: str,
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
## InstanceStorageConfigTypeDef

```python
# InstanceStorageConfigTypeDef definition

class InstanceStorageConfigTypeDef(TypedDict):
    StorageType: StorageTypeType,  # (1)
    AssociationId: NotRequired[str],
    S3Config: NotRequired[S3ConfigTypeDef],  # (2)
    KinesisVideoStreamConfig: NotRequired[KinesisVideoStreamConfigTypeDef],  # (3)
    KinesisStreamConfig: NotRequired[KinesisStreamConfigTypeDef],  # (4)
    KinesisFirehoseConfig: NotRequired[KinesisFirehoseConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
3. See [:material-code-braces: KinesisVideoStreamConfigTypeDef](./type_defs.md#kinesisvideostreamconfigtypedef) 
4. See [:material-code-braces: KinesisStreamConfigTypeDef](./type_defs.md#kinesisstreamconfigtypedef) 
5. See [:material-code-braces: KinesisFirehoseConfigTypeDef](./type_defs.md#kinesisfirehoseconfigtypedef) 
## SubmitContactEvaluationRequestRequestTypeDef

```python
# SubmitContactEvaluationRequestRequestTypeDef definition

class SubmitContactEvaluationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
    Answers: NotRequired[Mapping[str, EvaluationAnswerInputTypeDef]],  # (1)
    Notes: NotRequired[Mapping[str, EvaluationNoteTypeDef]],  # (2)
```

1. See [:material-code-braces: EvaluationAnswerInputTypeDef](./type_defs.md#evaluationanswerinputtypedef) 
2. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
## UpdateContactEvaluationRequestRequestTypeDef

```python
# UpdateContactEvaluationRequestRequestTypeDef definition

class UpdateContactEvaluationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    EvaluationId: str,
    Answers: NotRequired[Mapping[str, EvaluationAnswerInputTypeDef]],  # (1)
    Notes: NotRequired[Mapping[str, EvaluationNoteTypeDef]],  # (2)
```

1. See [:material-code-braces: EvaluationAnswerInputTypeDef](./type_defs.md#evaluationanswerinputtypedef) 
2. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
## EvaluationFormNumericQuestionPropertiesTypeDef

```python
# EvaluationFormNumericQuestionPropertiesTypeDef definition

class EvaluationFormNumericQuestionPropertiesTypeDef(TypedDict):
    MinValue: int,
    MaxValue: int,
    Options: NotRequired[Sequence[EvaluationFormNumericQuestionOptionTypeDef]],  # (1)
    Automation: NotRequired[EvaluationFormNumericQuestionAutomationTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormNumericQuestionOptionTypeDef](./type_defs.md#evaluationformnumericquestionoptiontypedef) 
2. See [:material-code-braces: EvaluationFormNumericQuestionAutomationTypeDef](./type_defs.md#evaluationformnumericquestionautomationtypedef) 
## EvaluationFormSingleSelectQuestionAutomationTypeDef

```python
# EvaluationFormSingleSelectQuestionAutomationTypeDef definition

class EvaluationFormSingleSelectQuestionAutomationTypeDef(TypedDict):
    Options: Sequence[EvaluationFormSingleSelectQuestionAutomationOptionTypeDef],  # (1)
    DefaultOptionRefId: NotRequired[str],
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationOptionTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationoptiontypedef) 
## EvaluationTypeDef

```python
# EvaluationTypeDef definition

class EvaluationTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationArn: str,
    Metadata: EvaluationMetadataTypeDef,  # (1)
    Answers: Dict[str, EvaluationAnswerOutputTypeDef],  # (2)
    Notes: Dict[str, EvaluationNoteTypeDef],  # (3)
    Status: EvaluationStatusType,  # (4)
    CreatedTime: datetime,
    LastModifiedTime: datetime,
    Scores: NotRequired[Dict[str, EvaluationScoreTypeDef]],  # (5)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EvaluationMetadataTypeDef](./type_defs.md#evaluationmetadatatypedef) 
2. See [:material-code-braces: EvaluationAnswerOutputTypeDef](./type_defs.md#evaluationansweroutputtypedef) 
3. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
4. See [:material-code-brackets: EvaluationStatusType](./literals.md#evaluationstatustype) 
5. See [:material-code-braces: EvaluationScoreTypeDef](./type_defs.md#evaluationscoretypedef) 
## ListContactEvaluationsResponseTypeDef

```python
# ListContactEvaluationsResponseTypeDef definition

class ListContactEvaluationsResponseTypeDef(TypedDict):
    EvaluationSummaryList: List[EvaluationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationSummaryTypeDef](./type_defs.md#evaluationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseActionDefinitionTypeDef

```python
# CreateCaseActionDefinitionTypeDef definition

class CreateCaseActionDefinitionTypeDef(TypedDict):
    Fields: Sequence[FieldValueTypeDef],  # (1)
    TemplateId: str,
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
## UpdateCaseActionDefinitionTypeDef

```python
# UpdateCaseActionDefinitionTypeDef definition

class UpdateCaseActionDefinitionTypeDef(TypedDict):
    Fields: Sequence[FieldValueTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
## UserDataTypeDef

```python
# UserDataTypeDef definition

class UserDataTypeDef(TypedDict):
    User: NotRequired[UserReferenceTypeDef],  # (1)
    RoutingProfile: NotRequired[RoutingProfileReferenceTypeDef],  # (2)
    HierarchyPath: NotRequired[HierarchyPathReferenceTypeDef],  # (3)
    Status: NotRequired[AgentStatusReferenceTypeDef],  # (4)
    AvailableSlotsByChannel: NotRequired[Dict[ChannelType, int]],  # (5)
    MaxSlotsByChannel: NotRequired[Dict[ChannelType, int]],  # (5)
    ActiveSlotsByChannel: NotRequired[Dict[ChannelType, int]],  # (5)
    Contacts: NotRequired[List[AgentContactReferenceTypeDef]],  # (8)
    NextStatus: NotRequired[str],
```

1. See [:material-code-braces: UserReferenceTypeDef](./type_defs.md#userreferencetypedef) 
2. See [:material-code-braces: RoutingProfileReferenceTypeDef](./type_defs.md#routingprofilereferencetypedef) 
3. See [:material-code-braces: HierarchyPathReferenceTypeDef](./type_defs.md#hierarchypathreferencetypedef) 
4. See [:material-code-braces: AgentStatusReferenceTypeDef](./type_defs.md#agentstatusreferencetypedef) 
5. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
6. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
7. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
8. See [:material-code-braces: AgentContactReferenceTypeDef](./type_defs.md#agentcontactreferencetypedef) 
## HierarchyGroupTypeDef

```python
# HierarchyGroupTypeDef definition

class HierarchyGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    LevelId: NotRequired[str],
    HierarchyPath: NotRequired[HierarchyPathTypeDef],  # (1)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: HierarchyPathTypeDef](./type_defs.md#hierarchypathtypedef) 
## DescribeUserHierarchyStructureResponseTypeDef

```python
# DescribeUserHierarchyStructureResponseTypeDef definition

class DescribeUserHierarchyStructureResponseTypeDef(TypedDict):
    HierarchyStructure: HierarchyStructureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HierarchyStructureTypeDef](./type_defs.md#hierarchystructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserHierarchyStructureRequestRequestTypeDef

```python
# UpdateUserHierarchyStructureRequestRequestTypeDef definition

class UpdateUserHierarchyStructureRequestRequestTypeDef(TypedDict):
    HierarchyStructure: HierarchyStructureUpdateTypeDef,  # (1)
    InstanceId: str,
```

1. See [:material-code-braces: HierarchyStructureUpdateTypeDef](./type_defs.md#hierarchystructureupdatetypedef) 
## GetMetricDataRequestGetMetricDataPaginateTypeDef

```python
# GetMetricDataRequestGetMetricDataPaginateTypeDef definition

class GetMetricDataRequestGetMetricDataPaginateTypeDef(TypedDict):
    InstanceId: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: NotRequired[Sequence[GroupingType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetMetricDataRequestRequestTypeDef

```python
# GetMetricDataRequestRequestTypeDef definition

class GetMetricDataRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: NotRequired[Sequence[GroupingType]],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
## HistoricalMetricDataTypeDef

```python
# HistoricalMetricDataTypeDef definition

class HistoricalMetricDataTypeDef(TypedDict):
    Metric: NotRequired[HistoricalMetricTypeDef],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
## CreateHoursOfOperationRequestRequestTypeDef

```python
# CreateHoursOfOperationRequestRequestTypeDef definition

class CreateHoursOfOperationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    TimeZone: str,
    Config: Sequence[HoursOfOperationConfigTypeDef],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
## HoursOfOperationTypeDef

```python
# HoursOfOperationTypeDef definition

class HoursOfOperationTypeDef(TypedDict):
    HoursOfOperationId: NotRequired[str],
    HoursOfOperationArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    TimeZone: NotRequired[str],
    Config: NotRequired[List[HoursOfOperationConfigTypeDef]],  # (1)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
## UpdateHoursOfOperationRequestRequestTypeDef

```python
# UpdateHoursOfOperationRequestRequestTypeDef definition

class UpdateHoursOfOperationRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    HoursOfOperationId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    TimeZone: NotRequired[str],
    Config: NotRequired[Sequence[HoursOfOperationConfigTypeDef]],  # (1)
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
## SearchPredefinedAttributesRequestSearchPredefinedAttributesPaginateTypeDef

```python
# SearchPredefinedAttributesRequestSearchPredefinedAttributesPaginateTypeDef definition

class SearchPredefinedAttributesRequestSearchPredefinedAttributesPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchCriteria: NotRequired[PredefinedAttributeSearchCriteriaTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PredefinedAttributeSearchCriteriaTypeDef](./type_defs.md#predefinedattributesearchcriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstanceResponseTypeDef

```python
# DescribeInstanceResponseTypeDef definition

class DescribeInstanceResponseTypeDef(TypedDict):
    Instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaskTemplateConstraintsTypeDef

```python
# TaskTemplateConstraintsTypeDef definition

class TaskTemplateConstraintsTypeDef(TypedDict):
    RequiredFields: NotRequired[Sequence[RequiredFieldInfoTypeDef]],  # (1)
    ReadOnlyFields: NotRequired[Sequence[ReadOnlyFieldInfoTypeDef]],  # (2)
    InvisibleFields: NotRequired[Sequence[InvisibleFieldInfoTypeDef]],  # (3)
```

1. See [:material-code-braces: RequiredFieldInfoTypeDef](./type_defs.md#requiredfieldinfotypedef) 
2. See [:material-code-braces: ReadOnlyFieldInfoTypeDef](./type_defs.md#readonlyfieldinfotypedef) 
3. See [:material-code-braces: InvisibleFieldInfoTypeDef](./type_defs.md#invisiblefieldinfotypedef) 
## TaskTemplateDefaultsTypeDef

```python
# TaskTemplateDefaultsTypeDef definition

class TaskTemplateDefaultsTypeDef(TypedDict):
    DefaultFieldValues: NotRequired[Sequence[TaskTemplateDefaultFieldValueTypeDef]],  # (1)
```

1. See [:material-code-braces: TaskTemplateDefaultFieldValueTypeDef](./type_defs.md#tasktemplatedefaultfieldvaluetypedef) 
## GetMetricDataV2RequestRequestTypeDef

```python
# GetMetricDataV2RequestRequestTypeDef definition

class GetMetricDataV2RequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Filters: Sequence[FilterV2TypeDef],  # (1)
    Metrics: Sequence[MetricV2TypeDef],  # (2)
    Interval: NotRequired[IntervalDetailsTypeDef],  # (3)
    Groupings: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterV2TypeDef](./type_defs.md#filterv2typedef) 
2. See [:material-code-braces: MetricV2TypeDef](./type_defs.md#metricv2typedef) 
3. See [:material-code-braces: IntervalDetailsTypeDef](./type_defs.md#intervaldetailstypedef) 
## MetricDataV2TypeDef

```python
# MetricDataV2TypeDef definition

class MetricDataV2TypeDef(TypedDict):
    Metric: NotRequired[MetricV2TypeDef],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-braces: MetricV2TypeDef](./type_defs.md#metricv2typedef) 
## SendChatIntegrationEventRequestRequestTypeDef

```python
# SendChatIntegrationEventRequestRequestTypeDef definition

class SendChatIntegrationEventRequestRequestTypeDef(TypedDict):
    SourceId: str,
    DestinationId: str,
    Event: ChatEventTypeDef,  # (1)
    Subtype: NotRequired[str],
    NewSessionDetails: NotRequired[NewSessionDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: ChatEventTypeDef](./type_defs.md#chateventtypedef) 
2. See [:material-code-braces: NewSessionDetailsTypeDef](./type_defs.md#newsessiondetailstypedef) 
## ChatParticipantRoleConfigTypeDef

```python
# ChatParticipantRoleConfigTypeDef definition

class ChatParticipantRoleConfigTypeDef(TypedDict):
    ParticipantTimerConfigList: Sequence[ParticipantTimerConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ParticipantTimerConfigurationTypeDef](./type_defs.md#participanttimerconfigurationtypedef) 
## SearchPredefinedAttributesResponsePaginatorTypeDef

```python
# SearchPredefinedAttributesResponsePaginatorTypeDef definition

class SearchPredefinedAttributesResponsePaginatorTypeDef(TypedDict):
    PredefinedAttributes: List[PredefinedAttributePaginatorTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredefinedAttributePaginatorTypeDef](./type_defs.md#predefinedattributepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQuickConnectRequestRequestTypeDef

```python
# CreateQuickConnectRequestRequestTypeDef definition

class CreateQuickConnectRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    QuickConnectConfig: QuickConnectConfigTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
## QuickConnectTypeDef

```python
# QuickConnectTypeDef definition

class QuickConnectTypeDef(TypedDict):
    QuickConnectARN: NotRequired[str],
    QuickConnectId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    QuickConnectConfig: NotRequired[QuickConnectConfigTypeDef],  # (1)
    Tags: NotRequired[Dict[str, str]],
    LastModifiedTime: NotRequired[datetime],
    LastModifiedRegion: NotRequired[str],
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
## UpdateQuickConnectConfigRequestRequestTypeDef

```python
# UpdateQuickConnectConfigRequestRequestTypeDef definition

class UpdateQuickConnectConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    QuickConnectId: str,
    QuickConnectConfig: QuickConnectConfigTypeDef,  # (1)
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
## RealTimeContactAnalysisSegmentTranscriptTypeDef

```python
# RealTimeContactAnalysisSegmentTranscriptTypeDef definition

class RealTimeContactAnalysisSegmentTranscriptTypeDef(TypedDict):
    Id: str,
    ParticipantId: str,
    ParticipantRole: ParticipantRoleType,  # (1)
    Content: str,
    Time: RealTimeContactAnalysisTimeDataTypeDef,  # (2)
    DisplayName: NotRequired[str],
    ContentType: NotRequired[str],
    Redaction: NotRequired[RealTimeContactAnalysisTranscriptItemRedactionTypeDef],  # (3)
    Sentiment: NotRequired[RealTimeContactAnalysisSentimentLabelType],  # (4)
```

1. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
2. See [:material-code-braces: RealTimeContactAnalysisTimeDataTypeDef](./type_defs.md#realtimecontactanalysistimedatatypedef) 
3. See [:material-code-braces: RealTimeContactAnalysisTranscriptItemRedactionTypeDef](./type_defs.md#realtimecontactanalysistranscriptitemredactiontypedef) 
4. See [:material-code-brackets: RealTimeContactAnalysisSentimentLabelType](./literals.md#realtimecontactanalysissentimentlabeltype) 
## RealTimeContactAnalysisPointOfInterestTypeDef

```python
# RealTimeContactAnalysisPointOfInterestTypeDef definition

class RealTimeContactAnalysisPointOfInterestTypeDef(TypedDict):
    TranscriptItems: NotRequired[List[RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef]],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisTranscriptItemWithCharacterOffsetsTypeDef](./type_defs.md#realtimecontactanalysistranscriptitemwithcharacteroffsetstypedef) 
## RealTimeContactAnalysisIssueDetectedTypeDef

```python
# RealTimeContactAnalysisIssueDetectedTypeDef definition

class RealTimeContactAnalysisIssueDetectedTypeDef(TypedDict):
    TranscriptItems: List[RealTimeContactAnalysisTranscriptItemWithContentTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisTranscriptItemWithContentTypeDef](./type_defs.md#realtimecontactanalysistranscriptitemwithcontenttypedef) 
## ListContactReferencesResponseTypeDef

```python
# ListContactReferencesResponseTypeDef definition

class ListContactReferencesResponseTypeDef(TypedDict):
    ReferenceSummaryList: List[ReferenceSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReferenceSummaryTypeDef](./type_defs.md#referencesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchResourceTagsRequestRequestTypeDef

```python
# SearchResourceTagsRequestRequestTypeDef definition

class SearchResourceTagsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceTypes: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchCriteria: NotRequired[ResourceTagsSearchCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagsSearchCriteriaTypeDef](./type_defs.md#resourcetagssearchcriteriatypedef) 
## SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef

```python
# SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef definition

class SearchResourceTagsRequestSearchResourceTagsPaginateTypeDef(TypedDict):
    InstanceId: str,
    ResourceTypes: NotRequired[Sequence[str]],
    SearchCriteria: NotRequired[ResourceTagsSearchCriteriaTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceTagsSearchCriteriaTypeDef](./type_defs.md#resourcetagssearchcriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTrafficDistributionResponseTypeDef

```python
# GetTrafficDistributionResponseTypeDef definition

class GetTrafficDistributionResponseTypeDef(TypedDict):
    TelephonyConfig: TelephonyConfigTypeDef,  # (1)
    Id: str,
    Arn: str,
    SignInConfig: SignInConfigTypeDef,  # (2)
    AgentConfig: AgentConfigTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TelephonyConfigTypeDef](./type_defs.md#telephonyconfigtypedef) 
2. See [:material-code-braces: SignInConfigTypeDef](./type_defs.md#signinconfigtypedef) 
3. See [:material-code-braces: AgentConfigTypeDef](./type_defs.md#agentconfigtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrafficDistributionRequestRequestTypeDef

```python
# UpdateTrafficDistributionRequestRequestTypeDef definition

class UpdateTrafficDistributionRequestRequestTypeDef(TypedDict):
    Id: str,
    TelephonyConfig: NotRequired[TelephonyConfigTypeDef],  # (1)
    SignInConfig: NotRequired[SignInConfigTypeDef],  # (2)
    AgentConfig: NotRequired[AgentConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TelephonyConfigTypeDef](./type_defs.md#telephonyconfigtypedef) 
2. See [:material-code-braces: SignInConfigTypeDef](./type_defs.md#signinconfigtypedef) 
3. See [:material-code-braces: AgentConfigTypeDef](./type_defs.md#agentconfigtypedef) 
## ContactAnalysisTypeDef

```python
# ContactAnalysisTypeDef definition

class ContactAnalysisTypeDef(TypedDict):
    Transcript: NotRequired[TranscriptTypeDef],  # (1)
```

1. See [:material-code-braces: TranscriptTypeDef](./type_defs.md#transcripttypedef) 
## SearchUsersResponseTypeDef

```python
# SearchUsersResponseTypeDef definition

class SearchUsersResponseTypeDef(TypedDict):
    Users: List[UserSearchSummaryTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserSearchSummaryTypeDef](./type_defs.md#usersearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewResponseTypeDef

```python
# CreateViewResponseTypeDef definition

class CreateViewResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewVersionResponseTypeDef

```python
# CreateViewVersionResponseTypeDef definition

class CreateViewVersionResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeViewResponseTypeDef

```python
# DescribeViewResponseTypeDef definition

class DescribeViewResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateViewContentResponseTypeDef

```python
# UpdateViewContentResponseTypeDef definition

class UpdateViewContentResponseTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionDataTypeDef

```python
# ConnectionDataTypeDef definition

class ConnectionDataTypeDef(TypedDict):
    Attendee: NotRequired[AttendeeTypeDef],  # (1)
    Meeting: NotRequired[MeetingTypeDef],  # (2)
```

1. See [:material-code-braces: AttendeeTypeDef](./type_defs.md#attendeetypedef) 
2. See [:material-code-braces: MeetingTypeDef](./type_defs.md#meetingtypedef) 
## SearchHoursOfOperationsRequestRequestTypeDef

```python
# SearchHoursOfOperationsRequestRequestTypeDef definition

class SearchHoursOfOperationsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[HoursOfOperationSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[HoursOfOperationSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationSearchCriteriaTypeDef](./type_defs.md#hoursofoperationsearchcriteriatypedef) 
## SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef

```python
# SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef definition

class SearchHoursOfOperationsRequestSearchHoursOfOperationsPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[HoursOfOperationSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[HoursOfOperationSearchCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationSearchCriteriaTypeDef](./type_defs.md#hoursofoperationsearchcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchPromptsRequestRequestTypeDef

```python
# SearchPromptsRequestRequestTypeDef definition

class SearchPromptsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[PromptSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[PromptSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: PromptSearchFilterTypeDef](./type_defs.md#promptsearchfiltertypedef) 
2. See [:material-code-braces: PromptSearchCriteriaTypeDef](./type_defs.md#promptsearchcriteriatypedef) 
## SearchPromptsRequestSearchPromptsPaginateTypeDef

```python
# SearchPromptsRequestSearchPromptsPaginateTypeDef definition

class SearchPromptsRequestSearchPromptsPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[PromptSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[PromptSearchCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: PromptSearchFilterTypeDef](./type_defs.md#promptsearchfiltertypedef) 
2. See [:material-code-braces: PromptSearchCriteriaTypeDef](./type_defs.md#promptsearchcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQueuesRequestRequestTypeDef

```python
# SearchQueuesRequestRequestTypeDef definition

class SearchQueuesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[QueueSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QueueSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: QueueSearchFilterTypeDef](./type_defs.md#queuesearchfiltertypedef) 
2. See [:material-code-braces: QueueSearchCriteriaTypeDef](./type_defs.md#queuesearchcriteriatypedef) 
## SearchQueuesRequestSearchQueuesPaginateTypeDef

```python
# SearchQueuesRequestSearchQueuesPaginateTypeDef definition

class SearchQueuesRequestSearchQueuesPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[QueueSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QueueSearchCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: QueueSearchFilterTypeDef](./type_defs.md#queuesearchfiltertypedef) 
2. See [:material-code-braces: QueueSearchCriteriaTypeDef](./type_defs.md#queuesearchcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchQuickConnectsRequestRequestTypeDef

```python
# SearchQuickConnectsRequestRequestTypeDef definition

class SearchQuickConnectsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[QuickConnectSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QuickConnectSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: QuickConnectSearchFilterTypeDef](./type_defs.md#quickconnectsearchfiltertypedef) 
2. See [:material-code-braces: QuickConnectSearchCriteriaTypeDef](./type_defs.md#quickconnectsearchcriteriatypedef) 
## SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef

```python
# SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef definition

class SearchQuickConnectsRequestSearchQuickConnectsPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[QuickConnectSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[QuickConnectSearchCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: QuickConnectSearchFilterTypeDef](./type_defs.md#quickconnectsearchfiltertypedef) 
2. See [:material-code-braces: QuickConnectSearchCriteriaTypeDef](./type_defs.md#quickconnectsearchcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchRoutingProfilesRequestRequestTypeDef

```python
# SearchRoutingProfilesRequestRequestTypeDef definition

class SearchRoutingProfilesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[RoutingProfileSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[RoutingProfileSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: RoutingProfileSearchFilterTypeDef](./type_defs.md#routingprofilesearchfiltertypedef) 
2. See [:material-code-braces: RoutingProfileSearchCriteriaTypeDef](./type_defs.md#routingprofilesearchcriteriatypedef) 
## SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef

```python
# SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef definition

class SearchRoutingProfilesRequestSearchRoutingProfilesPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[RoutingProfileSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[RoutingProfileSearchCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: RoutingProfileSearchFilterTypeDef](./type_defs.md#routingprofilesearchfiltertypedef) 
2. See [:material-code-braces: RoutingProfileSearchCriteriaTypeDef](./type_defs.md#routingprofilesearchcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchSecurityProfilesRequestRequestTypeDef

```python
# SearchSecurityProfilesRequestRequestTypeDef definition

class SearchSecurityProfilesRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchCriteria: NotRequired[SecurityProfileSearchCriteriaTypeDef],  # (1)
    SearchFilter: NotRequired[SecurityProfilesSearchFilterTypeDef],  # (2)
```

1. See [:material-code-braces: SecurityProfileSearchCriteriaTypeDef](./type_defs.md#securityprofilesearchcriteriatypedef) 
2. See [:material-code-braces: SecurityProfilesSearchFilterTypeDef](./type_defs.md#securityprofilessearchfiltertypedef) 
## SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef

```python
# SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef definition

class SearchSecurityProfilesRequestSearchSecurityProfilesPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchCriteria: NotRequired[SecurityProfileSearchCriteriaTypeDef],  # (1)
    SearchFilter: NotRequired[SecurityProfilesSearchFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: SecurityProfileSearchCriteriaTypeDef](./type_defs.md#securityprofilesearchcriteriatypedef) 
2. See [:material-code-braces: SecurityProfilesSearchFilterTypeDef](./type_defs.md#securityprofilessearchfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUsersRequestRequestTypeDef

```python
# SearchUsersRequestRequestTypeDef definition

class SearchUsersRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SearchFilter: NotRequired[UserSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[UserSearchCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: UserSearchFilterTypeDef](./type_defs.md#usersearchfiltertypedef) 
2. See [:material-code-braces: UserSearchCriteriaTypeDef](./type_defs.md#usersearchcriteriatypedef) 
## SearchUsersRequestSearchUsersPaginateTypeDef

```python
# SearchUsersRequestSearchUsersPaginateTypeDef definition

class SearchUsersRequestSearchUsersPaginateTypeDef(TypedDict):
    InstanceId: str,
    SearchFilter: NotRequired[UserSearchFilterTypeDef],  # (1)
    SearchCriteria: NotRequired[UserSearchCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: UserSearchFilterTypeDef](./type_defs.md#usersearchfiltertypedef) 
2. See [:material-code-braces: UserSearchCriteriaTypeDef](./type_defs.md#usersearchcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRoutingProfileResponseTypeDef

```python
# DescribeRoutingProfileResponseTypeDef definition

class DescribeRoutingProfileResponseTypeDef(TypedDict):
    RoutingProfile: RoutingProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutingProfileTypeDef](./type_defs.md#routingprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchRoutingProfilesResponseTypeDef

```python
# SearchRoutingProfilesResponseTypeDef definition

class SearchRoutingProfilesResponseTypeDef(TypedDict):
    RoutingProfiles: List[RoutingProfileTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoutingProfileTypeDef](./type_defs.md#routingprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCurrentMetricDataResponseTypeDef

```python
# GetCurrentMetricDataResponseTypeDef definition

class GetCurrentMetricDataResponseTypeDef(TypedDict):
    NextToken: str,
    MetricResults: List[CurrentMetricResultTypeDef],  # (1)
    DataSnapshotTime: datetime,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CurrentMetricResultTypeDef](./type_defs.md#currentmetricresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateInstanceStorageConfigRequestRequestTypeDef

```python
# AssociateInstanceStorageConfigRequestRequestTypeDef definition

class AssociateInstanceStorageConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    StorageConfig: InstanceStorageConfigTypeDef,  # (2)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
## DescribeInstanceStorageConfigResponseTypeDef

```python
# DescribeInstanceStorageConfigResponseTypeDef definition

class DescribeInstanceStorageConfigResponseTypeDef(TypedDict):
    StorageConfig: InstanceStorageConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceStorageConfigsResponseTypeDef

```python
# ListInstanceStorageConfigsResponseTypeDef definition

class ListInstanceStorageConfigsResponseTypeDef(TypedDict):
    StorageConfigs: List[InstanceStorageConfigTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInstanceStorageConfigRequestRequestTypeDef

```python
# UpdateInstanceStorageConfigRequestRequestTypeDef definition

class UpdateInstanceStorageConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    StorageConfig: InstanceStorageConfigTypeDef,  # (2)
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
## EvaluationFormSingleSelectQuestionPropertiesTypeDef

```python
# EvaluationFormSingleSelectQuestionPropertiesTypeDef definition

class EvaluationFormSingleSelectQuestionPropertiesTypeDef(TypedDict):
    Options: Sequence[EvaluationFormSingleSelectQuestionOptionTypeDef],  # (1)
    DisplayAs: NotRequired[EvaluationFormSingleSelectQuestionDisplayModeType],  # (2)
    Automation: NotRequired[EvaluationFormSingleSelectQuestionAutomationTypeDef],  # (3)
```

1. See [:material-code-braces: EvaluationFormSingleSelectQuestionOptionTypeDef](./type_defs.md#evaluationformsingleselectquestionoptiontypedef) 
2. See [:material-code-brackets: EvaluationFormSingleSelectQuestionDisplayModeType](./literals.md#evaluationformsingleselectquestiondisplaymodetype) 
3. See [:material-code-braces: EvaluationFormSingleSelectQuestionAutomationTypeDef](./type_defs.md#evaluationformsingleselectquestionautomationtypedef) 
## DescribeContactEvaluationResponseTypeDef

```python
# DescribeContactEvaluationResponseTypeDef definition

class DescribeContactEvaluationResponseTypeDef(TypedDict):
    Evaluation: EvaluationTypeDef,  # (1)
    EvaluationForm: EvaluationFormContentTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) 
2. See [:material-code-braces: EvaluationFormContentTypeDef](./type_defs.md#evaluationformcontenttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleActionTypeDef

```python
# RuleActionTypeDef definition

class RuleActionTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
    TaskAction: NotRequired[TaskActionDefinitionTypeDef],  # (2)
    EventBridgeAction: NotRequired[EventBridgeActionDefinitionTypeDef],  # (3)
    AssignContactCategoryAction: NotRequired[Mapping[str, Any]],
    SendNotificationAction: NotRequired[SendNotificationActionDefinitionTypeDef],  # (4)
    CreateCaseAction: NotRequired[CreateCaseActionDefinitionTypeDef],  # (5)
    UpdateCaseAction: NotRequired[UpdateCaseActionDefinitionTypeDef],  # (6)
    EndAssociatedTasksAction: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: TaskActionDefinitionTypeDef](./type_defs.md#taskactiondefinitiontypedef) 
3. See [:material-code-braces: EventBridgeActionDefinitionTypeDef](./type_defs.md#eventbridgeactiondefinitiontypedef) 
4. See [:material-code-braces: SendNotificationActionDefinitionTypeDef](./type_defs.md#sendnotificationactiondefinitiontypedef) 
5. See [:material-code-braces: CreateCaseActionDefinitionTypeDef](./type_defs.md#createcaseactiondefinitiontypedef) 
6. See [:material-code-braces: UpdateCaseActionDefinitionTypeDef](./type_defs.md#updatecaseactiondefinitiontypedef) 
## GetCurrentUserDataResponseTypeDef

```python
# GetCurrentUserDataResponseTypeDef definition

class GetCurrentUserDataResponseTypeDef(TypedDict):
    NextToken: str,
    UserDataList: List[UserDataTypeDef],  # (1)
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserDataTypeDef](./type_defs.md#userdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserHierarchyGroupResponseTypeDef

```python
# DescribeUserHierarchyGroupResponseTypeDef definition

class DescribeUserHierarchyGroupResponseTypeDef(TypedDict):
    HierarchyGroup: HierarchyGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HierarchyGroupTypeDef](./type_defs.md#hierarchygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HistoricalMetricResultTypeDef

```python
# HistoricalMetricResultTypeDef definition

class HistoricalMetricResultTypeDef(TypedDict):
    Dimensions: NotRequired[DimensionsTypeDef],  # (1)
    Collections: NotRequired[List[HistoricalMetricDataTypeDef]],  # (2)
```

1. See [:material-code-braces: DimensionsTypeDef](./type_defs.md#dimensionstypedef) 
2. See [:material-code-braces: HistoricalMetricDataTypeDef](./type_defs.md#historicalmetricdatatypedef) 
## DescribeHoursOfOperationResponseTypeDef

```python
# DescribeHoursOfOperationResponseTypeDef definition

class DescribeHoursOfOperationResponseTypeDef(TypedDict):
    HoursOfOperation: HoursOfOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HoursOfOperationTypeDef](./type_defs.md#hoursofoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchHoursOfOperationsResponseTypeDef

```python
# SearchHoursOfOperationsResponseTypeDef definition

class SearchHoursOfOperationsResponseTypeDef(TypedDict):
    HoursOfOperations: List[HoursOfOperationTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HoursOfOperationTypeDef](./type_defs.md#hoursofoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskTemplateRequestRequestTypeDef

```python
# CreateTaskTemplateRequestRequestTypeDef definition

class CreateTaskTemplateRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    Fields: Sequence[TaskTemplateFieldTypeDef],  # (1)
    Description: NotRequired[str],
    ContactFlowId: NotRequired[str],
    Constraints: NotRequired[TaskTemplateConstraintsTypeDef],  # (2)
    Defaults: NotRequired[TaskTemplateDefaultsTypeDef],  # (3)
    Status: NotRequired[TaskTemplateStatusType],  # (4)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
2. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
3. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
## GetTaskTemplateResponseTypeDef

```python
# GetTaskTemplateResponseTypeDef definition

class GetTaskTemplateResponseTypeDef(TypedDict):
    InstanceId: str,
    Id: str,
    Arn: str,
    Name: str,
    Description: str,
    ContactFlowId: str,
    Constraints: TaskTemplateConstraintsTypeDef,  # (1)
    Defaults: TaskTemplateDefaultsTypeDef,  # (2)
    Fields: List[TaskTemplateFieldTypeDef],  # (3)
    Status: TaskTemplateStatusType,  # (4)
    LastModifiedTime: datetime,
    CreatedTime: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
3. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskTemplateRequestRequestTypeDef

```python
# UpdateTaskTemplateRequestRequestTypeDef definition

class UpdateTaskTemplateRequestRequestTypeDef(TypedDict):
    TaskTemplateId: str,
    InstanceId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ContactFlowId: NotRequired[str],
    Constraints: NotRequired[TaskTemplateConstraintsTypeDef],  # (1)
    Defaults: NotRequired[TaskTemplateDefaultsTypeDef],  # (2)
    Status: NotRequired[TaskTemplateStatusType],  # (3)
    Fields: NotRequired[Sequence[TaskTemplateFieldTypeDef]],  # (4)
```

1. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
3. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
4. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
## UpdateTaskTemplateResponseTypeDef

```python
# UpdateTaskTemplateResponseTypeDef definition

class UpdateTaskTemplateResponseTypeDef(TypedDict):
    InstanceId: str,
    Id: str,
    Arn: str,
    Name: str,
    Description: str,
    ContactFlowId: str,
    Constraints: TaskTemplateConstraintsTypeDef,  # (1)
    Defaults: TaskTemplateDefaultsTypeDef,  # (2)
    Fields: List[TaskTemplateFieldTypeDef],  # (3)
    Status: TaskTemplateStatusType,  # (4)
    LastModifiedTime: datetime,
    CreatedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
3. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricResultV2TypeDef

```python
# MetricResultV2TypeDef definition

class MetricResultV2TypeDef(TypedDict):
    Dimensions: NotRequired[Dict[str, str]],
    MetricInterval: NotRequired[MetricIntervalTypeDef],  # (1)
    Collections: NotRequired[List[MetricDataV2TypeDef]],  # (2)
```

1. See [:material-code-braces: MetricIntervalTypeDef](./type_defs.md#metricintervaltypedef) 
2. See [:material-code-braces: MetricDataV2TypeDef](./type_defs.md#metricdatav2typedef) 
## UpdateParticipantRoleConfigChannelInfoTypeDef

```python
# UpdateParticipantRoleConfigChannelInfoTypeDef definition

class UpdateParticipantRoleConfigChannelInfoTypeDef(TypedDict):
    Chat: NotRequired[ChatParticipantRoleConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ChatParticipantRoleConfigTypeDef](./type_defs.md#chatparticipantroleconfigtypedef) 
## DescribeQuickConnectResponseTypeDef

```python
# DescribeQuickConnectResponseTypeDef definition

class DescribeQuickConnectResponseTypeDef(TypedDict):
    QuickConnect: QuickConnectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickConnectTypeDef](./type_defs.md#quickconnecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchQuickConnectsResponseTypeDef

```python
# SearchQuickConnectsResponseTypeDef definition

class SearchQuickConnectsResponseTypeDef(TypedDict):
    QuickConnects: List[QuickConnectTypeDef],  # (1)
    NextToken: str,
    ApproximateTotalCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickConnectTypeDef](./type_defs.md#quickconnecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RealTimeContactAnalysisCategoryDetailsTypeDef

```python
# RealTimeContactAnalysisCategoryDetailsTypeDef definition

class RealTimeContactAnalysisCategoryDetailsTypeDef(TypedDict):
    PointsOfInterest: List[RealTimeContactAnalysisPointOfInterestTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisPointOfInterestTypeDef](./type_defs.md#realtimecontactanalysispointofinteresttypedef) 
## RealTimeContactAnalysisSegmentIssuesTypeDef

```python
# RealTimeContactAnalysisSegmentIssuesTypeDef definition

class RealTimeContactAnalysisSegmentIssuesTypeDef(TypedDict):
    IssuesDetected: List[RealTimeContactAnalysisIssueDetectedTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisIssueDetectedTypeDef](./type_defs.md#realtimecontactanalysisissuedetectedtypedef) 
## SearchCriteriaTypeDef

```python
# SearchCriteriaTypeDef definition

class SearchCriteriaTypeDef(TypedDict):
    AgentIds: NotRequired[Sequence[str]],
    AgentHierarchyGroups: NotRequired[AgentHierarchyGroupsTypeDef],  # (1)
    Channels: NotRequired[Sequence[ChannelType]],  # (2)
    ContactAnalysis: NotRequired[ContactAnalysisTypeDef],  # (3)
    InitiationMethods: NotRequired[Sequence[ContactInitiationMethodType]],  # (4)
    QueueIds: NotRequired[Sequence[str]],
    SearchableContactAttributes: NotRequired[SearchableContactAttributesTypeDef],  # (5)
```

1. See [:material-code-braces: AgentHierarchyGroupsTypeDef](./type_defs.md#agenthierarchygroupstypedef) 
2. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
3. See [:material-code-braces: ContactAnalysisTypeDef](./type_defs.md#contactanalysistypedef) 
4. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
5. See [:material-code-braces: SearchableContactAttributesTypeDef](./type_defs.md#searchablecontactattributestypedef) 
## StartWebRTCContactResponseTypeDef

```python
# StartWebRTCContactResponseTypeDef definition

class StartWebRTCContactResponseTypeDef(TypedDict):
    ConnectionData: ConnectionDataTypeDef,  # (1)
    ContactId: str,
    ParticipantId: str,
    ParticipantToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionDataTypeDef](./type_defs.md#connectiondatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationFormQuestionTypePropertiesTypeDef

```python
# EvaluationFormQuestionTypePropertiesTypeDef definition

class EvaluationFormQuestionTypePropertiesTypeDef(TypedDict):
    Numeric: NotRequired[EvaluationFormNumericQuestionPropertiesTypeDef],  # (1)
    SingleSelect: NotRequired[EvaluationFormSingleSelectQuestionPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationFormNumericQuestionPropertiesTypeDef](./type_defs.md#evaluationformnumericquestionpropertiestypedef) 
2. See [:material-code-braces: EvaluationFormSingleSelectQuestionPropertiesTypeDef](./type_defs.md#evaluationformsingleselectquestionpropertiestypedef) 
## CreateRuleRequestRequestTypeDef

```python
# CreateRuleRequestRequestTypeDef definition

class CreateRuleRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Name: str,
    TriggerEventSource: RuleTriggerEventSourceTypeDef,  # (1)
    Function: str,
    Actions: Sequence[RuleActionTypeDef],  # (2)
    PublishStatus: RulePublishStatusType,  # (3)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: RuleTriggerEventSourceTypeDef](./type_defs.md#ruletriggereventsourcetypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
3. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Name: str,
    RuleId: str,
    RuleArn: str,
    TriggerEventSource: RuleTriggerEventSourceTypeDef,  # (1)
    Function: str,
    Actions: List[RuleActionTypeDef],  # (2)
    PublishStatus: RulePublishStatusType,  # (3)
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    LastUpdatedBy: str,
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RuleTriggerEventSourceTypeDef](./type_defs.md#ruletriggereventsourcetypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
3. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
## UpdateRuleRequestRequestTypeDef

```python
# UpdateRuleRequestRequestTypeDef definition

class UpdateRuleRequestRequestTypeDef(TypedDict):
    RuleId: str,
    InstanceId: str,
    Name: str,
    Function: str,
    Actions: Sequence[RuleActionTypeDef],  # (1)
    PublishStatus: RulePublishStatusType,  # (2)
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
## GetMetricDataResponseTypeDef

```python
# GetMetricDataResponseTypeDef definition

class GetMetricDataResponseTypeDef(TypedDict):
    NextToken: str,
    MetricResults: List[HistoricalMetricResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HistoricalMetricResultTypeDef](./type_defs.md#historicalmetricresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMetricDataV2ResponseTypeDef

```python
# GetMetricDataV2ResponseTypeDef definition

class GetMetricDataV2ResponseTypeDef(TypedDict):
    NextToken: str,
    MetricResults: List[MetricResultV2TypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricResultV2TypeDef](./type_defs.md#metricresultv2typedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateParticipantRoleConfigRequestRequestTypeDef

```python
# UpdateParticipantRoleConfigRequestRequestTypeDef definition

class UpdateParticipantRoleConfigRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ContactId: str,
    ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateParticipantRoleConfigChannelInfoTypeDef](./type_defs.md#updateparticipantroleconfigchannelinfotypedef) 
## RealTimeContactAnalysisSegmentCategoriesTypeDef

```python
# RealTimeContactAnalysisSegmentCategoriesTypeDef definition

class RealTimeContactAnalysisSegmentCategoriesTypeDef(TypedDict):
    MatchedDetails: Dict[str, RealTimeContactAnalysisCategoryDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: RealTimeContactAnalysisCategoryDetailsTypeDef](./type_defs.md#realtimecontactanalysiscategorydetailstypedef) 
## SearchContactsRequestRequestTypeDef

```python
# SearchContactsRequestRequestTypeDef definition

class SearchContactsRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    TimeRange: SearchContactsTimeRangeTypeDef,  # (1)
    SearchCriteria: NotRequired[SearchCriteriaTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Sort: NotRequired[SortTypeDef],  # (3)
```

1. See [:material-code-braces: SearchContactsTimeRangeTypeDef](./type_defs.md#searchcontactstimerangetypedef) 
2. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchContactsRequestSearchContactsPaginateTypeDef

```python
# SearchContactsRequestSearchContactsPaginateTypeDef definition

class SearchContactsRequestSearchContactsPaginateTypeDef(TypedDict):
    InstanceId: str,
    TimeRange: SearchContactsTimeRangeTypeDef,  # (1)
    SearchCriteria: NotRequired[SearchCriteriaTypeDef],  # (2)
    Sort: NotRequired[SortTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: SearchContactsTimeRangeTypeDef](./type_defs.md#searchcontactstimerangetypedef) 
2. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## EvaluationFormQuestionTypeDef

```python
# EvaluationFormQuestionTypeDef definition

class EvaluationFormQuestionTypeDef(TypedDict):
    Title: str,
    RefId: str,
    QuestionType: EvaluationFormQuestionTypeType,  # (1)
    Instructions: NotRequired[str],
    NotApplicableEnabled: NotRequired[bool],
    QuestionTypeProperties: NotRequired[EvaluationFormQuestionTypePropertiesTypeDef],  # (2)
    Weight: NotRequired[float],
```

1. See [:material-code-brackets: EvaluationFormQuestionTypeType](./literals.md#evaluationformquestiontypetype) 
2. See [:material-code-braces: EvaluationFormQuestionTypePropertiesTypeDef](./type_defs.md#evaluationformquestiontypepropertiestypedef) 
## DescribeRuleResponseTypeDef

```python
# DescribeRuleResponseTypeDef definition

class DescribeRuleResponseTypeDef(TypedDict):
    Rule: RuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RealtimeContactAnalysisSegmentTypeDef

```python
# RealtimeContactAnalysisSegmentTypeDef definition

class RealtimeContactAnalysisSegmentTypeDef(TypedDict):
    Transcript: NotRequired[RealTimeContactAnalysisSegmentTranscriptTypeDef],  # (1)
    Categories: NotRequired[RealTimeContactAnalysisSegmentCategoriesTypeDef],  # (2)
    Issues: NotRequired[RealTimeContactAnalysisSegmentIssuesTypeDef],  # (3)
    Event: NotRequired[RealTimeContactAnalysisSegmentEventTypeDef],  # (4)
    Attachments: NotRequired[RealTimeContactAnalysisSegmentAttachmentsTypeDef],  # (5)
```

1. See [:material-code-braces: RealTimeContactAnalysisSegmentTranscriptTypeDef](./type_defs.md#realtimecontactanalysissegmenttranscripttypedef) 
2. See [:material-code-braces: RealTimeContactAnalysisSegmentCategoriesTypeDef](./type_defs.md#realtimecontactanalysissegmentcategoriestypedef) 
3. See [:material-code-braces: RealTimeContactAnalysisSegmentIssuesTypeDef](./type_defs.md#realtimecontactanalysissegmentissuestypedef) 
4. See [:material-code-braces: RealTimeContactAnalysisSegmentEventTypeDef](./type_defs.md#realtimecontactanalysissegmenteventtypedef) 
5. See [:material-code-braces: RealTimeContactAnalysisSegmentAttachmentsTypeDef](./type_defs.md#realtimecontactanalysissegmentattachmentstypedef) 
## EvaluationFormItemTypeDef

```python
# EvaluationFormItemTypeDef definition

class EvaluationFormItemTypeDef(TypedDict):
    Section: NotRequired[Dict[str, Any]],
    Question: NotRequired[EvaluationFormQuestionTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationFormQuestionTypeDef](./type_defs.md#evaluationformquestiontypedef) 
## ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef

```python
# ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef definition

class ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef(TypedDict):
    Channel: RealTimeContactAnalysisSupportedChannelType,  # (1)
    Status: RealTimeContactAnalysisStatusType,  # (2)
    Segments: List[RealtimeContactAnalysisSegmentTypeDef],  # (3)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: RealTimeContactAnalysisSupportedChannelType](./literals.md#realtimecontactanalysissupportedchanneltype) 
2. See [:material-code-brackets: RealTimeContactAnalysisStatusType](./literals.md#realtimecontactanalysisstatustype) 
3. See [:material-code-braces: RealtimeContactAnalysisSegmentTypeDef](./type_defs.md#realtimecontactanalysissegmenttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
