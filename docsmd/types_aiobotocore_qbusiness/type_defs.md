# Type definitions

> [Index](../README.md) > [QBusiness](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

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




## ActionExecutionPayloadFieldPaginatorTypeDef

```python
# ActionExecutionPayloadFieldPaginatorTypeDef definition

class ActionExecutionPayloadFieldPaginatorTypeDef(TypedDict):
    value: Dict[str, Any],
```

## ActionExecutionPayloadFieldTypeDef

```python
# ActionExecutionPayloadFieldTypeDef definition

class ActionExecutionPayloadFieldTypeDef(TypedDict):
    value: Mapping[str, Any],
```

## ActionReviewPayloadFieldAllowedValueTypeDef

```python
# ActionReviewPayloadFieldAllowedValueTypeDef definition

class ActionReviewPayloadFieldAllowedValueTypeDef(TypedDict):
    displayValue: NotRequired[Dict[str, Any]],
    value: NotRequired[Dict[str, Any]],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    applicationId: NotRequired[str],
    createdAt: NotRequired[datetime],
    displayName: NotRequired[str],
    status: NotRequired[ApplicationStatusType],  # (1)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
## AppliedAttachmentsConfigurationTypeDef

```python
# AppliedAttachmentsConfigurationTypeDef definition

class AppliedAttachmentsConfigurationTypeDef(TypedDict):
    attachmentsControlMode: NotRequired[AttachmentsControlModeType],  # (1)
```

1. See [:material-code-brackets: AttachmentsControlModeType](./literals.md#attachmentscontrolmodetype) 
## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## AttachmentsConfigurationTypeDef

```python
# AttachmentsConfigurationTypeDef definition

class AttachmentsConfigurationTypeDef(TypedDict):
    attachmentsControlMode: AttachmentsControlModeType,  # (1)
```

1. See [:material-code-brackets: AttachmentsControlModeType](./literals.md#attachmentscontrolmodetype) 
## BasicAuthConfigurationTypeDef

```python
# BasicAuthConfigurationTypeDef definition

class BasicAuthConfigurationTypeDef(TypedDict):
    roleArn: str,
    secretArn: str,
```

## DeleteDocumentTypeDef

```python
# DeleteDocumentTypeDef definition

class DeleteDocumentTypeDef(TypedDict):
    documentId: str,
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

## BlockedPhrasesConfigurationTypeDef

```python
# BlockedPhrasesConfigurationTypeDef definition

class BlockedPhrasesConfigurationTypeDef(TypedDict):
    blockedPhrases: NotRequired[List[str]],
    systemMessageOverride: NotRequired[str],
```

## BlockedPhrasesConfigurationUpdateTypeDef

```python
# BlockedPhrasesConfigurationUpdateTypeDef definition

class BlockedPhrasesConfigurationUpdateTypeDef(TypedDict):
    blockedPhrasesToCreateOrUpdate: NotRequired[Sequence[str]],
    blockedPhrasesToDelete: NotRequired[Sequence[str]],
    systemMessageOverride: NotRequired[str],
```

## ContentBlockerRuleTypeDef

```python
# ContentBlockerRuleTypeDef definition

class ContentBlockerRuleTypeDef(TypedDict):
    systemMessageOverride: NotRequired[str],
```

## EligibleDataSourceTypeDef

```python
# EligibleDataSourceTypeDef definition

class EligibleDataSourceTypeDef(TypedDict):
    dataSourceId: NotRequired[str],
    indexId: NotRequired[str],
```

## ConversationTypeDef

```python
# ConversationTypeDef definition

class ConversationTypeDef(TypedDict):
    conversationId: NotRequired[str],
    startTime: NotRequired[datetime],
    title: NotRequired[str],
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## DataSourceVpcConfigurationTypeDef

```python
# DataSourceVpcConfigurationTypeDef definition

class DataSourceVpcConfigurationTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
```

## IndexCapacityConfigurationTypeDef

```python
# IndexCapacityConfigurationTypeDef definition

class IndexCapacityConfigurationTypeDef(TypedDict):
    units: NotRequired[int],
```

## UserAliasTypeDef

```python
# UserAliasTypeDef definition

class UserAliasTypeDef(TypedDict):
    userId: str,
    dataSourceId: NotRequired[str],
    indexId: NotRequired[str],
```

## DataSourceSyncJobMetricsTypeDef

```python
# DataSourceSyncJobMetricsTypeDef definition

class DataSourceSyncJobMetricsTypeDef(TypedDict):
    documentsAdded: NotRequired[str],
    documentsDeleted: NotRequired[str],
    documentsFailed: NotRequired[str],
    documentsModified: NotRequired[str],
    documentsScanned: NotRequired[str],
```

## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    dataSourceId: NotRequired[str],
    displayName: NotRequired[str],
    status: NotRequired[DataSourceStatusType],  # (1)
    type: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## DeleteChatControlsConfigurationRequestRequestTypeDef

```python
# DeleteChatControlsConfigurationRequestRequestTypeDef definition

class DeleteChatControlsConfigurationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## DeleteConversationRequestRequestTypeDef

```python
# DeleteConversationRequestRequestTypeDef definition

class DeleteConversationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    conversationId: str,
    userId: str,
```

## DeleteDataSourceRequestRequestTypeDef

```python
# DeleteDataSourceRequestRequestTypeDef definition

class DeleteDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    applicationId: str,
    groupName: str,
    indexId: str,
    dataSourceId: NotRequired[str],
```

## DeleteIndexRequestRequestTypeDef

```python
# DeleteIndexRequestRequestTypeDef definition

class DeleteIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
```

## DeletePluginRequestRequestTypeDef

```python
# DeletePluginRequestRequestTypeDef definition

class DeletePluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
```

## DeleteRetrieverRequestRequestTypeDef

```python
# DeleteRetrieverRequestRequestTypeDef definition

class DeleteRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
```

## DeleteWebExperienceRequestRequestTypeDef

```python
# DeleteWebExperienceRequestRequestTypeDef definition

class DeleteWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
```

## DocumentAttributeConfigurationTypeDef

```python
# DocumentAttributeConfigurationTypeDef definition

class DocumentAttributeConfigurationTypeDef(TypedDict):
    name: NotRequired[str],
    search: NotRequired[StatusType],  # (1)
    type: NotRequired[AttributeTypeType],  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: AttributeTypeType](./literals.md#attributetypetype) 
## S3TypeDef

```python
# S3TypeDef definition

class S3TypeDef(TypedDict):
    bucket: str,
    key: str,
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetChatControlsConfigurationRequestRequestTypeDef

```python
# GetChatControlsConfigurationRequestRequestTypeDef definition

class GetChatControlsConfigurationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetDataSourceRequestRequestTypeDef

```python
# GetDataSourceRequestRequestTypeDef definition

class GetDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
```

## GetGroupRequestRequestTypeDef

```python
# GetGroupRequestRequestTypeDef definition

class GetGroupRequestRequestTypeDef(TypedDict):
    applicationId: str,
    groupName: str,
    indexId: str,
    dataSourceId: NotRequired[str],
```

## GetIndexRequestRequestTypeDef

```python
# GetIndexRequestRequestTypeDef definition

class GetIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
```

## GetPluginRequestRequestTypeDef

```python
# GetPluginRequestRequestTypeDef definition

class GetPluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
```

## GetRetrieverRequestRequestTypeDef

```python
# GetRetrieverRequestRequestTypeDef definition

class GetRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
```

## GetUserRequestRequestTypeDef

```python
# GetUserRequestRequestTypeDef definition

class GetUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
```

## GetWebExperienceRequestRequestTypeDef

```python
# GetWebExperienceRequestRequestTypeDef definition

class GetWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
```

## MemberGroupTypeDef

```python
# MemberGroupTypeDef definition

class MemberGroupTypeDef(TypedDict):
    groupName: str,
    type: NotRequired[MembershipTypeType],  # (1)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## MemberUserTypeDef

```python
# MemberUserTypeDef definition

class MemberUserTypeDef(TypedDict):
    userId: str,
    type: NotRequired[MembershipTypeType],  # (1)
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## GroupSummaryTypeDef

```python
# GroupSummaryTypeDef definition

class GroupSummaryTypeDef(TypedDict):
    groupName: NotRequired[str],
```

## TextDocumentStatisticsTypeDef

```python
# TextDocumentStatisticsTypeDef definition

class TextDocumentStatisticsTypeDef(TypedDict):
    indexedTextBytes: NotRequired[int],
    indexedTextDocumentCount: NotRequired[int],
```

## IndexTypeDef

```python
# IndexTypeDef definition

class IndexTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    displayName: NotRequired[str],
    indexId: NotRequired[str],
    status: NotRequired[IndexStatusType],  # (1)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## KendraIndexConfigurationTypeDef

```python
# KendraIndexConfigurationTypeDef definition

class KendraIndexConfigurationTypeDef(TypedDict):
    indexId: str,
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListConversationsRequestRequestTypeDef

```python
# ListConversationsRequestRequestTypeDef definition

class ListConversationsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataSourcesRequestRequestTypeDef

```python
# ListDataSourcesRequestRequestTypeDef definition

class ListDataSourcesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDocumentsRequestRequestTypeDef

```python
# ListDocumentsRequestRequestTypeDef definition

class ListDocumentsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIndicesRequestRequestTypeDef

```python
# ListIndicesRequestRequestTypeDef definition

class ListIndicesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMessagesRequestRequestTypeDef

```python
# ListMessagesRequestRequestTypeDef definition

class ListMessagesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    conversationId: str,
    userId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPluginsRequestRequestTypeDef

```python
# ListPluginsRequestRequestTypeDef definition

class ListPluginsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PluginTypeDef

```python
# PluginTypeDef definition

class PluginTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    displayName: NotRequired[str],
    pluginId: NotRequired[str],
    serverUrl: NotRequired[str],
    state: NotRequired[PluginStateType],  # (1)
    type: NotRequired[PluginTypeType],  # (2)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
2. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
## ListRetrieversRequestRequestTypeDef

```python
# ListRetrieversRequestRequestTypeDef definition

class ListRetrieversRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RetrieverTypeDef

```python
# RetrieverTypeDef definition

class RetrieverTypeDef(TypedDict):
    applicationId: NotRequired[str],
    displayName: NotRequired[str],
    retrieverId: NotRequired[str],
    status: NotRequired[RetrieverStatusType],  # (1)
    type: NotRequired[RetrieverTypeType],  # (2)
```

1. See [:material-code-brackets: RetrieverStatusType](./literals.md#retrieverstatustype) 
2. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
```

## ListWebExperiencesRequestRequestTypeDef

```python
# ListWebExperiencesRequestRequestTypeDef definition

class ListWebExperiencesRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WebExperienceTypeDef

```python
# WebExperienceTypeDef definition

class WebExperienceTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    defaultEndpoint: NotRequired[str],
    status: NotRequired[WebExperienceStatusType],  # (1)
    updatedAt: NotRequired[datetime],
    webExperienceId: NotRequired[str],
```

1. See [:material-code-brackets: WebExperienceStatusType](./literals.md#webexperiencestatustype) 
## NativeIndexConfigurationTypeDef

```python
# NativeIndexConfigurationTypeDef definition

class NativeIndexConfigurationTypeDef(TypedDict):
    indexId: str,
```

## OAuth2ClientCredentialConfigurationTypeDef

```python
# OAuth2ClientCredentialConfigurationTypeDef definition

class OAuth2ClientCredentialConfigurationTypeDef(TypedDict):
    roleArn: str,
    secretArn: str,
```

## PrincipalGroupTypeDef

```python
# PrincipalGroupTypeDef definition

class PrincipalGroupTypeDef(TypedDict):
    access: ReadAccessTypeType,  # (1)
    membershipType: NotRequired[MembershipTypeType],  # (2)
    name: NotRequired[str],
```

1. See [:material-code-brackets: ReadAccessTypeType](./literals.md#readaccesstypetype) 
2. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## PrincipalUserTypeDef

```python
# PrincipalUserTypeDef definition

class PrincipalUserTypeDef(TypedDict):
    access: ReadAccessTypeType,  # (1)
    id: NotRequired[str],
    membershipType: NotRequired[MembershipTypeType],  # (2)
```

1. See [:material-code-brackets: ReadAccessTypeType](./literals.md#readaccesstypetype) 
2. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## UsersAndGroupsTypeDef

```python
# UsersAndGroupsTypeDef definition

class UsersAndGroupsTypeDef(TypedDict):
    userGroups: NotRequired[List[str]],
    userIds: NotRequired[List[str]],
```

## SamlConfigurationTypeDef

```python
# SamlConfigurationTypeDef definition

class SamlConfigurationTypeDef(TypedDict):
    metadataXML: str,
    roleArn: str,
    userIdAttribute: str,
    userGroupAttribute: NotRequired[str],
```

## TextSegmentTypeDef

```python
# TextSegmentTypeDef definition

class TextSegmentTypeDef(TypedDict):
    beginOffset: NotRequired[int],
    endOffset: NotRequired[int],
```

## StartDataSourceSyncJobRequestRequestTypeDef

```python
# StartDataSourceSyncJobRequestRequestTypeDef definition

class StartDataSourceSyncJobRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
```

## StopDataSourceSyncJobRequestRequestTypeDef

```python
# StopDataSourceSyncJobRequestRequestTypeDef definition

class StopDataSourceSyncJobRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## ActionExecutionPaginatorTypeDef

```python
# ActionExecutionPaginatorTypeDef definition

class ActionExecutionPaginatorTypeDef(TypedDict):
    payload: Dict[str, ActionExecutionPayloadFieldPaginatorTypeDef],  # (1)
    payloadFieldNameSeparator: str,
    pluginId: str,
```

1. See [:material-code-braces: ActionExecutionPayloadFieldPaginatorTypeDef](./type_defs.md#actionexecutionpayloadfieldpaginatortypedef) 
## ActionExecutionTypeDef

```python
# ActionExecutionTypeDef definition

class ActionExecutionTypeDef(TypedDict):
    payload: Mapping[str, ActionExecutionPayloadFieldTypeDef],  # (1)
    payloadFieldNameSeparator: str,
    pluginId: str,
```

1. See [:material-code-braces: ActionExecutionPayloadFieldTypeDef](./type_defs.md#actionexecutionpayloadfieldtypedef) 
## ActionReviewPayloadFieldTypeDef

```python
# ActionReviewPayloadFieldTypeDef definition

class ActionReviewPayloadFieldTypeDef(TypedDict):
    allowedValues: NotRequired[List[ActionReviewPayloadFieldAllowedValueTypeDef]],  # (1)
    displayName: NotRequired[str],
    displayOrder: NotRequired[int],
    required: NotRequired[bool],
    type: NotRequired[ActionPayloadFieldTypeType],  # (2)
    value: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: ActionReviewPayloadFieldAllowedValueTypeDef](./type_defs.md#actionreviewpayloadfieldallowedvaluetypedef) 
2. See [:material-code-brackets: ActionPayloadFieldTypeType](./literals.md#actionpayloadfieldtypetype) 
## AttachmentInputTypeDef

```python
# AttachmentInputTypeDef definition

class AttachmentInputTypeDef(TypedDict):
    data: Union[str, bytes, IO[Any], StreamingBody],
    name: str,
```

## AttachmentOutputTypeDef

```python
# AttachmentOutputTypeDef definition

class AttachmentOutputTypeDef(TypedDict):
    error: NotRequired[ErrorDetailTypeDef],  # (1)
    name: NotRequired[str],
    status: NotRequired[AttachmentStatusType],  # (2)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-brackets: AttachmentStatusType](./literals.md#attachmentstatustype) 
## DocumentDetailsTypeDef

```python
# DocumentDetailsTypeDef definition

class DocumentDetailsTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    documentId: NotRequired[str],
    error: NotRequired[ErrorDetailTypeDef],  # (1)
    status: NotRequired[DocumentStatusType],  # (2)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
## FailedDocumentTypeDef

```python
# FailedDocumentTypeDef definition

class FailedDocumentTypeDef(TypedDict):
    dataSourceId: NotRequired[str],
    error: NotRequired[ErrorDetailTypeDef],  # (1)
    id: NotRequired[str],
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## GroupStatusDetailTypeDef

```python
# GroupStatusDetailTypeDef definition

class GroupStatusDetailTypeDef(TypedDict):
    errorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    status: NotRequired[GroupStatusType],  # (2)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-brackets: GroupStatusType](./literals.md#groupstatustype) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    attachmentsConfiguration: NotRequired[AttachmentsConfigurationTypeDef],  # (1)
    description: NotRequired[str],
    displayName: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef) 
## BatchDeleteDocumentRequestRequestTypeDef

```python
# BatchDeleteDocumentRequestRequestTypeDef definition

class BatchDeleteDocumentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    documents: Sequence[DeleteDocumentTypeDef],  # (1)
    indexId: str,
    dataSourceSyncId: NotRequired[str],
```

1. See [:material-code-braces: DeleteDocumentTypeDef](./type_defs.md#deletedocumenttypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    applicationArn: str,
    applicationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    dataSourceArn: str,
    dataSourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIndexResponseTypeDef

```python
# CreateIndexResponseTypeDef definition

class CreateIndexResponseTypeDef(TypedDict):
    indexArn: str,
    indexId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePluginResponseTypeDef

```python
# CreatePluginResponseTypeDef definition

class CreatePluginResponseTypeDef(TypedDict):
    pluginArn: str,
    pluginId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRetrieverResponseTypeDef

```python
# CreateRetrieverResponseTypeDef definition

class CreateRetrieverResponseTypeDef(TypedDict):
    retrieverArn: str,
    retrieverId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWebExperienceResponseTypeDef

```python
# CreateWebExperienceResponseTypeDef definition

class CreateWebExperienceResponseTypeDef(TypedDict):
    webExperienceArn: str,
    webExperienceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    applications: List[ApplicationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataSourceSyncJobResponseTypeDef

```python
# StartDataSourceSyncJobResponseTypeDef definition

class StartDataSourceSyncJobResponseTypeDef(TypedDict):
    executionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContentRetrievalRuleTypeDef

```python
# ContentRetrievalRuleTypeDef definition

class ContentRetrievalRuleTypeDef(TypedDict):
    eligibleDataSources: NotRequired[List[EligibleDataSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: EligibleDataSourceTypeDef](./type_defs.md#eligibledatasourcetypedef) 
## ListConversationsResponseTypeDef

```python
# ListConversationsResponseTypeDef definition

class ListConversationsResponseTypeDef(TypedDict):
    conversations: List[ConversationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConversationTypeDef](./type_defs.md#conversationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    applicationArn: str,
    applicationId: str,
    attachmentsConfiguration: AppliedAttachmentsConfigurationTypeDef,  # (1)
    createdAt: datetime,
    description: str,
    displayName: str,
    encryptionConfiguration: EncryptionConfigurationTypeDef,  # (2)
    error: ErrorDetailTypeDef,  # (3)
    roleArn: str,
    status: ApplicationStatusType,  # (4)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AppliedAttachmentsConfigurationTypeDef](./type_defs.md#appliedattachmentsconfigurationtypedef) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
4. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    displayName: str,
    roleArn: str,
    attachmentsConfiguration: NotRequired[AttachmentsConfigurationTypeDef],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateWebExperienceRequestRequestTypeDef

```python
# CreateWebExperienceRequestRequestTypeDef definition

class CreateWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    clientToken: NotRequired[str],
    samplePromptsControlMode: NotRequired[WebExperienceSamplePromptsControlModeType],  # (1)
    subtitle: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    title: NotRequired[str],
    welcomeMessage: NotRequired[str],
```

1. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIndexRequestRequestTypeDef

```python
# CreateIndexRequestRequestTypeDef definition

class CreateIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    displayName: str,
    capacityConfiguration: NotRequired[IndexCapacityConfigurationTypeDef],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    clientToken: NotRequired[str],
    userAliases: NotRequired[Sequence[UserAliasTypeDef]],  # (1)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    userAliases: List[UserAliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    userAliasesToDelete: NotRequired[Sequence[UserAliasTypeDef]],  # (1)
    userAliasesToUpdate: NotRequired[Sequence[UserAliasTypeDef]],  # (1)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    userAliasesAdded: List[UserAliasTypeDef],  # (1)
    userAliasesDeleted: List[UserAliasTypeDef],  # (1)
    userAliasesUpdated: List[UserAliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
3. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceSyncJobTypeDef

```python
# DataSourceSyncJobTypeDef definition

class DataSourceSyncJobTypeDef(TypedDict):
    dataSourceErrorCode: NotRequired[str],
    endTime: NotRequired[datetime],
    error: NotRequired[ErrorDetailTypeDef],  # (1)
    executionId: NotRequired[str],
    metrics: NotRequired[DataSourceSyncJobMetricsTypeDef],  # (2)
    startTime: NotRequired[datetime],
    status: NotRequired[DataSourceSyncJobStatusType],  # (3)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-braces: DataSourceSyncJobMetricsTypeDef](./type_defs.md#datasourcesyncjobmetricstypedef) 
3. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    dataSources: List[DataSourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIndexRequestRequestTypeDef

```python
# UpdateIndexRequestRequestTypeDef definition

class UpdateIndexRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    capacityConfiguration: NotRequired[IndexCapacityConfigurationTypeDef],  # (1)
    description: NotRequired[str],
    displayName: NotRequired[str],
    documentAttributeConfigurations: NotRequired[Sequence[DocumentAttributeConfigurationTypeDef]],  # (2)
```

1. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
2. See [:material-code-braces: DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef) 
## DocumentAttributeValueTypeDef

```python
# DocumentAttributeValueTypeDef definition

class DocumentAttributeValueTypeDef(TypedDict):
    dateValue: NotRequired[Union[datetime, str]],
    longValue: NotRequired[int],
    stringListValue: NotRequired[Sequence[str]],
    stringValue: NotRequired[str],
```

## ListDataSourceSyncJobsRequestRequestTypeDef

```python
# ListDataSourceSyncJobsRequestRequestTypeDef definition

class ListDataSourceSyncJobsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
    endTime: NotRequired[Union[datetime, str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
    statusFilter: NotRequired[DataSourceSyncJobStatusType],  # (1)
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    updatedEarlierThan: Union[datetime, str],
    dataSourceId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MessageUsefulnessFeedbackTypeDef

```python
# MessageUsefulnessFeedbackTypeDef definition

class MessageUsefulnessFeedbackTypeDef(TypedDict):
    submittedAt: Union[datetime, str],
    usefulness: MessageUsefulnessType,  # (2)
    comment: NotRequired[str],
    reason: NotRequired[MessageUsefulnessReasonType],  # (1)
```

1. See [:material-code-brackets: MessageUsefulnessReasonType](./literals.md#messageusefulnessreasontype) 
2. See [:material-code-brackets: MessageUsefulnessType](./literals.md#messageusefulnesstype) 
## DocumentContentTypeDef

```python
# DocumentContentTypeDef definition

class DocumentContentTypeDef(TypedDict):
    blob: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    s3: NotRequired[S3TypeDef],  # (1)
```

1. See [:material-code-braces: S3TypeDef](./type_defs.md#s3typedef) 
## GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef

```python
# GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef definition

class GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConversationsRequestListConversationsPaginateTypeDef

```python
# ListConversationsRequestListConversationsPaginateTypeDef definition

class ListConversationsRequestListConversationsPaginateTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef

```python
# ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef definition

class ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
    endTime: NotRequired[Union[datetime, str]],
    startTime: NotRequired[Union[datetime, str]],
    statusFilter: NotRequired[DataSourceSyncJobStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesRequestListDataSourcesPaginateTypeDef

```python
# ListDataSourcesRequestListDataSourcesPaginateTypeDef definition

class ListDataSourcesRequestListDataSourcesPaginateTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDocumentsRequestListDocumentsPaginateTypeDef

```python
# ListDocumentsRequestListDocumentsPaginateTypeDef definition

class ListDocumentsRequestListDocumentsPaginateTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    dataSourceIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestListGroupsPaginateTypeDef

```python
# ListGroupsRequestListGroupsPaginateTypeDef definition

class ListGroupsRequestListGroupsPaginateTypeDef(TypedDict):
    applicationId: str,
    indexId: str,
    updatedEarlierThan: Union[datetime, str],
    dataSourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndicesRequestListIndicesPaginateTypeDef

```python
# ListIndicesRequestListIndicesPaginateTypeDef definition

class ListIndicesRequestListIndicesPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessagesRequestListMessagesPaginateTypeDef

```python
# ListMessagesRequestListMessagesPaginateTypeDef definition

class ListMessagesRequestListMessagesPaginateTypeDef(TypedDict):
    applicationId: str,
    conversationId: str,
    userId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPluginsRequestListPluginsPaginateTypeDef

```python
# ListPluginsRequestListPluginsPaginateTypeDef definition

class ListPluginsRequestListPluginsPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRetrieversRequestListRetrieversPaginateTypeDef

```python
# ListRetrieversRequestListRetrieversPaginateTypeDef definition

class ListRetrieversRequestListRetrieversPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWebExperiencesRequestListWebExperiencesPaginateTypeDef

```python
# ListWebExperiencesRequestListWebExperiencesPaginateTypeDef definition

class ListWebExperiencesRequestListWebExperiencesPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GroupMembersTypeDef

```python
# GroupMembersTypeDef definition

class GroupMembersTypeDef(TypedDict):
    memberGroups: NotRequired[Sequence[MemberGroupTypeDef]],  # (1)
    memberUsers: NotRequired[Sequence[MemberUserTypeDef]],  # (2)
```

1. See [:material-code-braces: MemberGroupTypeDef](./type_defs.md#membergrouptypedef) 
2. See [:material-code-braces: MemberUserTypeDef](./type_defs.md#memberusertypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    items: List[GroupSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IndexStatisticsTypeDef

```python
# IndexStatisticsTypeDef definition

class IndexStatisticsTypeDef(TypedDict):
    textDocumentStatistics: NotRequired[TextDocumentStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: TextDocumentStatisticsTypeDef](./type_defs.md#textdocumentstatisticstypedef) 
## ListIndicesResponseTypeDef

```python
# ListIndicesResponseTypeDef definition

class ListIndicesResponseTypeDef(TypedDict):
    indices: List[IndexTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IndexTypeDef](./type_defs.md#indextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPluginsResponseTypeDef

```python
# ListPluginsResponseTypeDef definition

class ListPluginsResponseTypeDef(TypedDict):
    nextToken: str,
    plugins: List[PluginTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PluginTypeDef](./type_defs.md#plugintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRetrieversResponseTypeDef

```python
# ListRetrieversResponseTypeDef definition

class ListRetrieversResponseTypeDef(TypedDict):
    nextToken: str,
    retrievers: List[RetrieverTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetrieverTypeDef](./type_defs.md#retrievertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebExperiencesResponseTypeDef

```python
# ListWebExperiencesResponseTypeDef definition

class ListWebExperiencesResponseTypeDef(TypedDict):
    nextToken: str,
    webExperiences: List[WebExperienceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebExperienceTypeDef](./type_defs.md#webexperiencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetrieverConfigurationTypeDef

```python
# RetrieverConfigurationTypeDef definition

class RetrieverConfigurationTypeDef(TypedDict):
    kendraIndexConfiguration: NotRequired[KendraIndexConfigurationTypeDef],  # (1)
    nativeIndexConfiguration: NotRequired[NativeIndexConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: KendraIndexConfigurationTypeDef](./type_defs.md#kendraindexconfigurationtypedef) 
2. See [:material-code-braces: NativeIndexConfigurationTypeDef](./type_defs.md#nativeindexconfigurationtypedef) 
## PluginAuthConfigurationTypeDef

```python
# PluginAuthConfigurationTypeDef definition

class PluginAuthConfigurationTypeDef(TypedDict):
    basicAuthConfiguration: NotRequired[BasicAuthConfigurationTypeDef],  # (1)
    oAuth2ClientCredentialConfiguration: NotRequired[OAuth2ClientCredentialConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: BasicAuthConfigurationTypeDef](./type_defs.md#basicauthconfigurationtypedef) 
2. See [:material-code-braces: OAuth2ClientCredentialConfigurationTypeDef](./type_defs.md#oauth2clientcredentialconfigurationtypedef) 
## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    group: NotRequired[PrincipalGroupTypeDef],  # (1)
    user: NotRequired[PrincipalUserTypeDef],  # (2)
```

1. See [:material-code-braces: PrincipalGroupTypeDef](./type_defs.md#principalgrouptypedef) 
2. See [:material-code-braces: PrincipalUserTypeDef](./type_defs.md#principalusertypedef) 
## WebExperienceAuthConfigurationTypeDef

```python
# WebExperienceAuthConfigurationTypeDef definition

class WebExperienceAuthConfigurationTypeDef(TypedDict):
    samlConfiguration: NotRequired[SamlConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef) 
## SourceAttributionTypeDef

```python
# SourceAttributionTypeDef definition

class SourceAttributionTypeDef(TypedDict):
    citationNumber: NotRequired[int],
    snippet: NotRequired[str],
    textMessageSegments: NotRequired[List[TextSegmentTypeDef]],  # (1)
    title: NotRequired[str],
    updatedAt: NotRequired[datetime],
    url: NotRequired[str],
```

1. See [:material-code-braces: TextSegmentTypeDef](./type_defs.md#textsegmenttypedef) 
## ActionReviewTypeDef

```python
# ActionReviewTypeDef definition

class ActionReviewTypeDef(TypedDict):
    payload: NotRequired[Dict[str, ActionReviewPayloadFieldTypeDef]],  # (1)
    payloadFieldNameSeparator: NotRequired[str],
    pluginId: NotRequired[str],
    pluginType: NotRequired[PluginTypeType],  # (2)
```

1. See [:material-code-braces: ActionReviewPayloadFieldTypeDef](./type_defs.md#actionreviewpayloadfieldtypedef) 
2. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
## ChatSyncInputRequestTypeDef

```python
# ChatSyncInputRequestTypeDef definition

class ChatSyncInputRequestTypeDef(TypedDict):
    applicationId: str,
    userId: str,
    actionExecution: NotRequired[ActionExecutionTypeDef],  # (1)
    attachments: NotRequired[Sequence[AttachmentInputTypeDef]],  # (2)
    attributeFilter: NotRequired[AttributeFilterTypeDef],  # (3)
    clientToken: NotRequired[str],
    conversationId: NotRequired[str],
    parentMessageId: NotRequired[str],
    userGroups: NotRequired[Sequence[str]],
    userMessage: NotRequired[str],
```

1. See [:material-code-braces: ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef) 
2. See [:material-code-braces: AttachmentInputTypeDef](./type_defs.md#attachmentinputtypedef) 
3. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
## ListDocumentsResponseTypeDef

```python
# ListDocumentsResponseTypeDef definition

class ListDocumentsResponseTypeDef(TypedDict):
    documentDetailList: List[DocumentDetailsTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentDetailsTypeDef](./type_defs.md#documentdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteDocumentResponseTypeDef

```python
# BatchDeleteDocumentResponseTypeDef definition

class BatchDeleteDocumentResponseTypeDef(TypedDict):
    failedDocuments: List[FailedDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutDocumentResponseTypeDef

```python
# BatchPutDocumentResponseTypeDef definition

class BatchPutDocumentResponseTypeDef(TypedDict):
    failedDocuments: List[FailedDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResponseTypeDef

```python
# GetGroupResponseTypeDef definition

class GetGroupResponseTypeDef(TypedDict):
    status: GroupStatusDetailTypeDef,  # (1)
    statusHistory: List[GroupStatusDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef) 
2. See [:material-code-braces: GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleConfigurationTypeDef

```python
# RuleConfigurationTypeDef definition

class RuleConfigurationTypeDef(TypedDict):
    contentBlockerRule: NotRequired[ContentBlockerRuleTypeDef],  # (1)
    contentRetrievalRule: NotRequired[ContentRetrievalRuleTypeDef],  # (2)
```

1. See [:material-code-braces: ContentBlockerRuleTypeDef](./type_defs.md#contentblockerruletypedef) 
2. See [:material-code-braces: ContentRetrievalRuleTypeDef](./type_defs.md#contentretrievalruletypedef) 
## ListDataSourceSyncJobsResponseTypeDef

```python
# ListDataSourceSyncJobsResponseTypeDef definition

class ListDataSourceSyncJobsResponseTypeDef(TypedDict):
    history: List[DataSourceSyncJobTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceSyncJobTypeDef](./type_defs.md#datasourcesyncjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentAttributeConditionTypeDef

```python
# DocumentAttributeConditionTypeDef definition

class DocumentAttributeConditionTypeDef(TypedDict):
    key: str,
    operator: DocumentEnrichmentConditionOperatorType,  # (1)
    value: NotRequired[DocumentAttributeValueTypeDef],  # (2)
```

1. See [:material-code-brackets: DocumentEnrichmentConditionOperatorType](./literals.md#documentenrichmentconditionoperatortype) 
2. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) 
## DocumentAttributeTargetTypeDef

```python
# DocumentAttributeTargetTypeDef definition

class DocumentAttributeTargetTypeDef(TypedDict):
    key: str,
    attributeValueOperator: NotRequired[AttributeValueOperatorType],  # (1)
    value: NotRequired[DocumentAttributeValueTypeDef],  # (2)
```

1. See [:material-code-brackets: AttributeValueOperatorType](./literals.md#attributevalueoperatortype) 
2. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) 
## DocumentAttributeTypeDef

```python
# DocumentAttributeTypeDef definition

class DocumentAttributeTypeDef(TypedDict):
    name: str,
    value: DocumentAttributeValueTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) 
## PutFeedbackRequestRequestTypeDef

```python
# PutFeedbackRequestRequestTypeDef definition

class PutFeedbackRequestRequestTypeDef(TypedDict):
    applicationId: str,
    conversationId: str,
    messageId: str,
    userId: str,
    messageCopiedAt: NotRequired[Union[datetime, str]],
    messageUsefulness: NotRequired[MessageUsefulnessFeedbackTypeDef],  # (1)
```

1. See [:material-code-braces: MessageUsefulnessFeedbackTypeDef](./type_defs.md#messageusefulnessfeedbacktypedef) 
## PutGroupRequestRequestTypeDef

```python
# PutGroupRequestRequestTypeDef definition

class PutGroupRequestRequestTypeDef(TypedDict):
    applicationId: str,
    groupMembers: GroupMembersTypeDef,  # (1)
    groupName: str,
    indexId: str,
    type: MembershipTypeType,  # (2)
    dataSourceId: NotRequired[str],
```

1. See [:material-code-braces: GroupMembersTypeDef](./type_defs.md#groupmemberstypedef) 
2. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
## GetIndexResponseTypeDef

```python
# GetIndexResponseTypeDef definition

class GetIndexResponseTypeDef(TypedDict):
    applicationId: str,
    capacityConfiguration: IndexCapacityConfigurationTypeDef,  # (1)
    createdAt: datetime,
    description: str,
    displayName: str,
    documentAttributeConfigurations: List[DocumentAttributeConfigurationTypeDef],  # (2)
    error: ErrorDetailTypeDef,  # (3)
    indexArn: str,
    indexId: str,
    indexStatistics: IndexStatisticsTypeDef,  # (4)
    status: IndexStatusType,  # (5)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
2. See [:material-code-braces: DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
4. See [:material-code-braces: IndexStatisticsTypeDef](./type_defs.md#indexstatisticstypedef) 
5. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRetrieverRequestRequestTypeDef

```python
# CreateRetrieverRequestRequestTypeDef definition

class CreateRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    configuration: RetrieverConfigurationTypeDef,  # (1)
    displayName: str,
    type: RetrieverTypeType,  # (2)
    clientToken: NotRequired[str],
    roleArn: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 
2. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetRetrieverResponseTypeDef

```python
# GetRetrieverResponseTypeDef definition

class GetRetrieverResponseTypeDef(TypedDict):
    applicationId: str,
    configuration: RetrieverConfigurationTypeDef,  # (1)
    createdAt: datetime,
    displayName: str,
    retrieverArn: str,
    retrieverId: str,
    roleArn: str,
    status: RetrieverStatusType,  # (2)
    type: RetrieverTypeType,  # (3)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 
2. See [:material-code-brackets: RetrieverStatusType](./literals.md#retrieverstatustype) 
3. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRetrieverRequestRequestTypeDef

```python
# UpdateRetrieverRequestRequestTypeDef definition

class UpdateRetrieverRequestRequestTypeDef(TypedDict):
    applicationId: str,
    retrieverId: str,
    configuration: NotRequired[RetrieverConfigurationTypeDef],  # (1)
    displayName: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 
## CreatePluginRequestRequestTypeDef

```python
# CreatePluginRequestRequestTypeDef definition

class CreatePluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    authConfiguration: PluginAuthConfigurationTypeDef,  # (1)
    displayName: str,
    serverUrl: str,
    type: PluginTypeType,  # (2)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 
2. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetPluginResponseTypeDef

```python
# GetPluginResponseTypeDef definition

class GetPluginResponseTypeDef(TypedDict):
    applicationId: str,
    authConfiguration: PluginAuthConfigurationTypeDef,  # (1)
    createdAt: datetime,
    displayName: str,
    pluginArn: str,
    pluginId: str,
    serverUrl: str,
    state: PluginStateType,  # (2)
    type: PluginTypeType,  # (3)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 
2. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
3. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePluginRequestRequestTypeDef

```python
# UpdatePluginRequestRequestTypeDef definition

class UpdatePluginRequestRequestTypeDef(TypedDict):
    applicationId: str,
    pluginId: str,
    authConfiguration: NotRequired[PluginAuthConfigurationTypeDef],  # (1)
    displayName: NotRequired[str],
    serverUrl: NotRequired[str],
    state: NotRequired[PluginStateType],  # (2)
```

1. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 
2. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
## AccessControlTypeDef

```python
# AccessControlTypeDef definition

class AccessControlTypeDef(TypedDict):
    principals: Sequence[PrincipalTypeDef],  # (2)
    memberRelation: NotRequired[MemberRelationType],  # (1)
```

1. See [:material-code-brackets: MemberRelationType](./literals.md#memberrelationtype) 
2. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
## GetWebExperienceResponseTypeDef

```python
# GetWebExperienceResponseTypeDef definition

class GetWebExperienceResponseTypeDef(TypedDict):
    applicationId: str,
    authenticationConfiguration: WebExperienceAuthConfigurationTypeDef,  # (1)
    createdAt: datetime,
    defaultEndpoint: str,
    error: ErrorDetailTypeDef,  # (2)
    samplePromptsControlMode: WebExperienceSamplePromptsControlModeType,  # (3)
    status: WebExperienceStatusType,  # (4)
    subtitle: str,
    title: str,
    updatedAt: datetime,
    webExperienceArn: str,
    webExperienceId: str,
    welcomeMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
3. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
4. See [:material-code-brackets: WebExperienceStatusType](./literals.md#webexperiencestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebExperienceRequestRequestTypeDef

```python
# UpdateWebExperienceRequestRequestTypeDef definition

class UpdateWebExperienceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    webExperienceId: str,
    authenticationConfiguration: NotRequired[WebExperienceAuthConfigurationTypeDef],  # (1)
    samplePromptsControlMode: NotRequired[WebExperienceSamplePromptsControlModeType],  # (2)
    subtitle: NotRequired[str],
    title: NotRequired[str],
    welcomeMessage: NotRequired[str],
```

1. See [:material-code-braces: WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef) 
2. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
## ChatSyncOutputTypeDef

```python
# ChatSyncOutputTypeDef definition

class ChatSyncOutputTypeDef(TypedDict):
    actionReview: ActionReviewTypeDef,  # (1)
    conversationId: str,
    failedAttachments: List[AttachmentOutputTypeDef],  # (2)
    sourceAttributions: List[SourceAttributionTypeDef],  # (3)
    systemMessage: str,
    systemMessageId: str,
    userMessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ActionReviewTypeDef](./type_defs.md#actionreviewtypedef) 
2. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
3. See [:material-code-braces: SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessagePaginatorTypeDef

```python
# MessagePaginatorTypeDef definition

class MessagePaginatorTypeDef(TypedDict):
    actionExecution: NotRequired[ActionExecutionPaginatorTypeDef],  # (1)
    actionReview: NotRequired[ActionReviewTypeDef],  # (2)
    attachments: NotRequired[List[AttachmentOutputTypeDef]],  # (3)
    body: NotRequired[str],
    messageId: NotRequired[str],
    sourceAttribution: NotRequired[List[SourceAttributionTypeDef]],  # (4)
    time: NotRequired[datetime],
    type: NotRequired[MessageTypeType],  # (5)
```

1. See [:material-code-braces: ActionExecutionPaginatorTypeDef](./type_defs.md#actionexecutionpaginatortypedef) 
2. See [:material-code-braces: ActionReviewTypeDef](./type_defs.md#actionreviewtypedef) 
3. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
4. See [:material-code-braces: SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef) 
5. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    actionExecution: NotRequired[ActionExecutionTypeDef],  # (1)
    actionReview: NotRequired[ActionReviewTypeDef],  # (2)
    attachments: NotRequired[List[AttachmentOutputTypeDef]],  # (3)
    body: NotRequired[str],
    messageId: NotRequired[str],
    sourceAttribution: NotRequired[List[SourceAttributionTypeDef]],  # (4)
    time: NotRequired[datetime],
    type: NotRequired[MessageTypeType],  # (5)
```

1. See [:material-code-braces: ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef) 
2. See [:material-code-braces: ActionReviewTypeDef](./type_defs.md#actionreviewtypedef) 
3. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
4. See [:material-code-braces: SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef) 
5. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    ruleType: RuleTypeType,  # (4)
    excludedUsersAndGroups: NotRequired[UsersAndGroupsTypeDef],  # (1)
    includedUsersAndGroups: NotRequired[UsersAndGroupsTypeDef],  # (1)
    ruleConfiguration: NotRequired[RuleConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef) 
2. See [:material-code-braces: UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef) 
3. See [:material-code-braces: RuleConfigurationTypeDef](./type_defs.md#ruleconfigurationtypedef) 
4. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## HookConfigurationTypeDef

```python
# HookConfigurationTypeDef definition

class HookConfigurationTypeDef(TypedDict):
    invocationCondition: NotRequired[DocumentAttributeConditionTypeDef],  # (1)
    lambdaArn: NotRequired[str],
    roleArn: NotRequired[str],
    s3BucketName: NotRequired[str],
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) 
## InlineDocumentEnrichmentConfigurationTypeDef

```python
# InlineDocumentEnrichmentConfigurationTypeDef definition

class InlineDocumentEnrichmentConfigurationTypeDef(TypedDict):
    condition: NotRequired[DocumentAttributeConditionTypeDef],  # (1)
    documentContentOperator: NotRequired[DocumentContentOperatorType],  # (2)
    target: NotRequired[DocumentAttributeTargetTypeDef],  # (3)
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) 
2. See [:material-code-brackets: DocumentContentOperatorType](./literals.md#documentcontentoperatortype) 
3. See [:material-code-braces: DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef) 
## AttributeFilterTypeDef

```python
# AttributeFilterTypeDef definition

class AttributeFilterTypeDef(TypedDict):
    andAllFilters: NotRequired[Sequence[Dict[str, Any]]],
    containsAll: NotRequired[DocumentAttributeTypeDef],  # (1)
    containsAny: NotRequired[DocumentAttributeTypeDef],  # (1)
    equalsTo: NotRequired[DocumentAttributeTypeDef],  # (1)
    greaterThan: NotRequired[DocumentAttributeTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[DocumentAttributeTypeDef],  # (1)
    lessThan: NotRequired[DocumentAttributeTypeDef],  # (1)
    lessThanOrEquals: NotRequired[DocumentAttributeTypeDef],  # (1)
    notFilter: NotRequired[Dict[str, Any]],
    orAllFilters: NotRequired[Sequence[Dict[str, Any]]],
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
2. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
3. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
4. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
5. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
6. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
7. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
## AccessConfigurationTypeDef

```python
# AccessConfigurationTypeDef definition

class AccessConfigurationTypeDef(TypedDict):
    accessControls: Sequence[AccessControlTypeDef],  # (1)
    memberRelation: NotRequired[MemberRelationType],  # (2)
```

1. See [:material-code-braces: AccessControlTypeDef](./type_defs.md#accesscontroltypedef) 
2. See [:material-code-brackets: MemberRelationType](./literals.md#memberrelationtype) 
## ListMessagesResponsePaginatorTypeDef

```python
# ListMessagesResponsePaginatorTypeDef definition

class ListMessagesResponsePaginatorTypeDef(TypedDict):
    messages: List[MessagePaginatorTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessagePaginatorTypeDef](./type_defs.md#messagepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMessagesResponseTypeDef

```python
# ListMessagesResponseTypeDef definition

class ListMessagesResponseTypeDef(TypedDict):
    messages: List[MessageTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TopicConfigurationTypeDef

```python
# TopicConfigurationTypeDef definition

class TopicConfigurationTypeDef(TypedDict):
    name: str,
    rules: List[RuleTypeDef],  # (1)
    description: NotRequired[str],
    exampleChatMessages: NotRequired[List[str]],
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## DocumentEnrichmentConfigurationTypeDef

```python
# DocumentEnrichmentConfigurationTypeDef definition

class DocumentEnrichmentConfigurationTypeDef(TypedDict):
    inlineConfigurations: NotRequired[Sequence[InlineDocumentEnrichmentConfigurationTypeDef]],  # (1)
    postExtractionHookConfiguration: NotRequired[HookConfigurationTypeDef],  # (2)
    preExtractionHookConfiguration: NotRequired[HookConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: InlineDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) 
3. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) 
## GetChatControlsConfigurationResponseTypeDef

```python
# GetChatControlsConfigurationResponseTypeDef definition

class GetChatControlsConfigurationResponseTypeDef(TypedDict):
    blockedPhrases: BlockedPhrasesConfigurationTypeDef,  # (1)
    nextToken: str,
    responseScope: ResponseScopeType,  # (2)
    topicConfigurations: List[TopicConfigurationTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: BlockedPhrasesConfigurationTypeDef](./type_defs.md#blockedphrasesconfigurationtypedef) 
2. See [:material-code-brackets: ResponseScopeType](./literals.md#responsescopetype) 
3. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChatControlsConfigurationRequestRequestTypeDef

```python
# UpdateChatControlsConfigurationRequestRequestTypeDef definition

class UpdateChatControlsConfigurationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    blockedPhrasesConfigurationUpdate: NotRequired[BlockedPhrasesConfigurationUpdateTypeDef],  # (1)
    clientToken: NotRequired[str],
    responseScope: NotRequired[ResponseScopeType],  # (2)
    topicConfigurationsToCreateOrUpdate: NotRequired[Sequence[TopicConfigurationTypeDef]],  # (3)
    topicConfigurationsToDelete: NotRequired[Sequence[TopicConfigurationTypeDef]],  # (3)
```

1. See [:material-code-braces: BlockedPhrasesConfigurationUpdateTypeDef](./type_defs.md#blockedphrasesconfigurationupdatetypedef) 
2. See [:material-code-brackets: ResponseScopeType](./literals.md#responsescopetype) 
3. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
4. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
## CreateDataSourceRequestRequestTypeDef

```python
# CreateDataSourceRequestRequestTypeDef definition

class CreateDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    configuration: Mapping[str, Any],
    displayName: str,
    indexId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    documentEnrichmentConfiguration: NotRequired[DocumentEnrichmentConfigurationTypeDef],  # (1)
    roleArn: NotRequired[str],
    syncSchedule: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    vpcConfiguration: NotRequired[DataSourceVpcConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    id: str,
    accessConfiguration: NotRequired[AccessConfigurationTypeDef],  # (1)
    attributes: NotRequired[Sequence[DocumentAttributeTypeDef]],  # (2)
    content: NotRequired[DocumentContentTypeDef],  # (3)
    contentType: NotRequired[ContentTypeType],  # (4)
    documentEnrichmentConfiguration: NotRequired[DocumentEnrichmentConfigurationTypeDef],  # (5)
    title: NotRequired[str],
```

1. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
2. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
3. See [:material-code-braces: DocumentContentTypeDef](./type_defs.md#documentcontenttypedef) 
4. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
5. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
## GetDataSourceResponseTypeDef

```python
# GetDataSourceResponseTypeDef definition

class GetDataSourceResponseTypeDef(TypedDict):
    applicationId: str,
    configuration: Dict[str, Any],
    createdAt: datetime,
    dataSourceArn: str,
    dataSourceId: str,
    description: str,
    displayName: str,
    documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef,  # (1)
    error: ErrorDetailTypeDef,  # (2)
    indexId: str,
    roleArn: str,
    status: DataSourceStatusType,  # (3)
    syncSchedule: str,
    type: str,
    updatedAt: datetime,
    vpcConfiguration: DataSourceVpcConfigurationTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
3. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
4. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourceRequestRequestTypeDef

```python
# UpdateDataSourceRequestRequestTypeDef definition

class UpdateDataSourceRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSourceId: str,
    indexId: str,
    configuration: NotRequired[Mapping[str, Any]],
    description: NotRequired[str],
    displayName: NotRequired[str],
    documentEnrichmentConfiguration: NotRequired[DocumentEnrichmentConfigurationTypeDef],  # (1)
    roleArn: NotRequired[str],
    syncSchedule: NotRequired[str],
    vpcConfiguration: NotRequired[DataSourceVpcConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
## BatchPutDocumentRequestRequestTypeDef

```python
# BatchPutDocumentRequestRequestTypeDef definition

class BatchPutDocumentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    documents: Sequence[DocumentTypeDef],  # (1)
    indexId: str,
    dataSourceSyncId: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
