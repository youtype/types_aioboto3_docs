# QBusiness module

> [Index](../README.md) > QBusiness


!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `QBusiness` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[qbusiness]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[qbusiness]'


# standalone installation
python -m pip install types-aiobotocore-qbusiness
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qbusiness
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QBusinessClient

Type annotations and code completion for  `#!python session.client("qbusiness")` as [QBusinessClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client)

```python
# QBusinessClient usage example

from aioboto3.session import Session

from types_aiobotocore_qbusiness.client import QBusinessClient


session = Session()
async with session.client("qbusiness") as client:
    client: QBusinessClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("qbusiness").get_paginator("...")`.

```python
# GetChatControlsConfigurationPaginator usage example

from types_aiobotocore_qbusiness.paginator import GetChatControlsConfigurationPaginator

def get_get_chat_controls_configuration_paginator() -> GetChatControlsConfigurationPaginator:
    return client.get_paginator("get_chat_controls_configuration"))
```

- [GetChatControlsConfigurationPaginator](./paginators.md#getchatcontrolsconfigurationpaginator)
- [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- [ListConversationsPaginator](./paginators.md#listconversationspaginator)
- [ListDataSourceSyncJobsPaginator](./paginators.md#listdatasourcesyncjobspaginator)
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListDocumentsPaginator](./paginators.md#listdocumentspaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListIndicesPaginator](./paginators.md#listindicespaginator)
- [ListMessagesPaginator](./paginators.md#listmessagespaginator)
- [ListPluginsPaginator](./paginators.md#listpluginspaginator)
- [ListRetrieversPaginator](./paginators.md#listretrieverspaginator)
- [ListWebExperiencesPaginator](./paginators.md#listwebexperiencespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionPayloadFieldTypeType usage example

from types_aiobotocore_qbusiness.literals import ActionPayloadFieldTypeType

def get_value() -> ActionPayloadFieldTypeType:
    return "ARRAY"
```

- [ActionPayloadFieldTypeType](./literals.md#actionpayloadfieldtypetype)
- [ApplicationStatusType](./literals.md#applicationstatustype)
- [AttachmentStatusType](./literals.md#attachmentstatustype)
- [AttachmentsControlModeType](./literals.md#attachmentscontrolmodetype)
- [AttributeTypeType](./literals.md#attributetypetype)
- [AttributeValueOperatorType](./literals.md#attributevalueoperatortype)
- [ContentTypeType](./literals.md#contenttypetype)
- [DataSourceStatusType](./literals.md#datasourcestatustype)
- [DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype)
- [DocumentContentOperatorType](./literals.md#documentcontentoperatortype)
- [DocumentEnrichmentConditionOperatorType](./literals.md#documentenrichmentconditionoperatortype)
- [DocumentStatusType](./literals.md#documentstatustype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [GetChatControlsConfigurationPaginatorName](./literals.md#getchatcontrolsconfigurationpaginatorname)
- [GroupStatusType](./literals.md#groupstatustype)
- [IndexStatusType](./literals.md#indexstatustype)
- [ListApplicationsPaginatorName](./literals.md#listapplicationspaginatorname)
- [ListConversationsPaginatorName](./literals.md#listconversationspaginatorname)
- [ListDataSourceSyncJobsPaginatorName](./literals.md#listdatasourcesyncjobspaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListDocumentsPaginatorName](./literals.md#listdocumentspaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListIndicesPaginatorName](./literals.md#listindicespaginatorname)
- [ListMessagesPaginatorName](./literals.md#listmessagespaginatorname)
- [ListPluginsPaginatorName](./literals.md#listpluginspaginatorname)
- [ListRetrieversPaginatorName](./literals.md#listretrieverspaginatorname)
- [ListWebExperiencesPaginatorName](./literals.md#listwebexperiencespaginatorname)
- [MemberRelationType](./literals.md#memberrelationtype)
- [MembershipTypeType](./literals.md#membershiptypetype)
- [MessageTypeType](./literals.md#messagetypetype)
- [MessageUsefulnessReasonType](./literals.md#messageusefulnessreasontype)
- [MessageUsefulnessType](./literals.md#messageusefulnesstype)
- [PluginStateType](./literals.md#pluginstatetype)
- [PluginTypeType](./literals.md#plugintypetype)
- [ReadAccessTypeType](./literals.md#readaccesstypetype)
- [ResponseScopeType](./literals.md#responsescopetype)
- [RetrieverStatusType](./literals.md#retrieverstatustype)
- [RetrieverTypeType](./literals.md#retrievertypetype)
- [RuleTypeType](./literals.md#ruletypetype)
- [StatusType](./literals.md#statustype)
- [WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype)
- [WebExperienceStatusType](./literals.md#webexperiencestatustype)
- [QBusinessServiceName](./literals.md#qbusinessservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionExecutionPayloadFieldPaginatorTypeDef](./type_defs.md#actionexecutionpayloadfieldpaginatortypedef)
- [ActionExecutionPayloadFieldTypeDef](./type_defs.md#actionexecutionpayloadfieldtypedef)
- [ActionReviewPayloadFieldAllowedValueTypeDef](./type_defs.md#actionreviewpayloadfieldallowedvaluetypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [AppliedAttachmentsConfigurationTypeDef](./type_defs.md#appliedattachmentsconfigurationtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef)
- [BasicAuthConfigurationTypeDef](./type_defs.md#basicauthconfigurationtypedef)
- [DeleteDocumentTypeDef](./type_defs.md#deletedocumenttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BlockedPhrasesConfigurationTypeDef](./type_defs.md#blockedphrasesconfigurationtypedef)
- [BlockedPhrasesConfigurationUpdateTypeDef](./type_defs.md#blockedphrasesconfigurationupdatetypedef)
- [ContentBlockerRuleTypeDef](./type_defs.md#contentblockerruletypedef)
- [EligibleDataSourceTypeDef](./type_defs.md#eligibledatasourcetypedef)
- [ConversationTypeDef](./type_defs.md#conversationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef)
- [IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef)
- [UserAliasTypeDef](./type_defs.md#useraliastypedef)
- [DataSourceSyncJobMetricsTypeDef](./type_defs.md#datasourcesyncjobmetricstypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef)
- [DeleteChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#deletechatcontrolsconfigurationrequestrequesttypedef)
- [DeleteConversationRequestRequestTypeDef](./type_defs.md#deleteconversationrequestrequesttypedef)
- [DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DeleteIndexRequestRequestTypeDef](./type_defs.md#deleteindexrequestrequesttypedef)
- [DeletePluginRequestRequestTypeDef](./type_defs.md#deletepluginrequestrequesttypedef)
- [DeleteRetrieverRequestRequestTypeDef](./type_defs.md#deleteretrieverrequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeleteWebExperienceRequestRequestTypeDef](./type_defs.md#deletewebexperiencerequestrequesttypedef)
- [DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [S3TypeDef](./type_defs.md#s3typedef)
- [GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef)
- [GetIndexRequestRequestTypeDef](./type_defs.md#getindexrequestrequesttypedef)
- [GetPluginRequestRequestTypeDef](./type_defs.md#getpluginrequestrequesttypedef)
- [GetRetrieverRequestRequestTypeDef](./type_defs.md#getretrieverrequestrequesttypedef)
- [GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef)
- [GetWebExperienceRequestRequestTypeDef](./type_defs.md#getwebexperiencerequestrequesttypedef)
- [MemberGroupTypeDef](./type_defs.md#membergrouptypedef)
- [MemberUserTypeDef](./type_defs.md#memberusertypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [TextDocumentStatisticsTypeDef](./type_defs.md#textdocumentstatisticstypedef)
- [IndexTypeDef](./type_defs.md#indextypedef)
- [KendraIndexConfigurationTypeDef](./type_defs.md#kendraindexconfigurationtypedef)
- [ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef)
- [ListConversationsRequestRequestTypeDef](./type_defs.md#listconversationsrequestrequesttypedef)
- [ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef)
- [ListDocumentsRequestRequestTypeDef](./type_defs.md#listdocumentsrequestrequesttypedef)
- [ListIndicesRequestRequestTypeDef](./type_defs.md#listindicesrequestrequesttypedef)
- [ListMessagesRequestRequestTypeDef](./type_defs.md#listmessagesrequestrequesttypedef)
- [ListPluginsRequestRequestTypeDef](./type_defs.md#listpluginsrequestrequesttypedef)
- [PluginTypeDef](./type_defs.md#plugintypedef)
- [ListRetrieversRequestRequestTypeDef](./type_defs.md#listretrieversrequestrequesttypedef)
- [RetrieverTypeDef](./type_defs.md#retrievertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWebExperiencesRequestRequestTypeDef](./type_defs.md#listwebexperiencesrequestrequesttypedef)
- [WebExperienceTypeDef](./type_defs.md#webexperiencetypedef)
- [NativeIndexConfigurationTypeDef](./type_defs.md#nativeindexconfigurationtypedef)
- [OAuth2ClientCredentialConfigurationTypeDef](./type_defs.md#oauth2clientcredentialconfigurationtypedef)
- [PrincipalGroupTypeDef](./type_defs.md#principalgrouptypedef)
- [PrincipalUserTypeDef](./type_defs.md#principalusertypedef)
- [UsersAndGroupsTypeDef](./type_defs.md#usersandgroupstypedef)
- [SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef)
- [TextSegmentTypeDef](./type_defs.md#textsegmenttypedef)
- [StartDataSourceSyncJobRequestRequestTypeDef](./type_defs.md#startdatasourcesyncjobrequestrequesttypedef)
- [StopDataSourceSyncJobRequestRequestTypeDef](./type_defs.md#stopdatasourcesyncjobrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ActionExecutionPaginatorTypeDef](./type_defs.md#actionexecutionpaginatortypedef)
- [ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef)
- [ActionReviewPayloadFieldTypeDef](./type_defs.md#actionreviewpayloadfieldtypedef)
- [AttachmentInputTypeDef](./type_defs.md#attachmentinputtypedef)
- [AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef)
- [DocumentDetailsTypeDef](./type_defs.md#documentdetailstypedef)
- [FailedDocumentTypeDef](./type_defs.md#faileddocumenttypedef)
- [GroupStatusDetailTypeDef](./type_defs.md#groupstatusdetailtypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [BatchDeleteDocumentRequestRequestTypeDef](./type_defs.md#batchdeletedocumentrequestrequesttypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [CreateIndexResponseTypeDef](./type_defs.md#createindexresponsetypedef)
- [CreatePluginResponseTypeDef](./type_defs.md#createpluginresponsetypedef)
- [CreateRetrieverResponseTypeDef](./type_defs.md#createretrieverresponsetypedef)
- [CreateWebExperienceResponseTypeDef](./type_defs.md#createwebexperienceresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)
- [StartDataSourceSyncJobResponseTypeDef](./type_defs.md#startdatasourcesyncjobresponsetypedef)
- [ContentRetrievalRuleTypeDef](./type_defs.md#contentretrievalruletypedef)
- [ListConversationsResponseTypeDef](./type_defs.md#listconversationsresponsetypedef)
- [GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [CreateWebExperienceRequestRequestTypeDef](./type_defs.md#createwebexperiencerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateIndexRequestRequestTypeDef](./type_defs.md#createindexrequestrequesttypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef)
- [DataSourceSyncJobTypeDef](./type_defs.md#datasourcesyncjobtypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [UpdateIndexRequestRequestTypeDef](./type_defs.md#updateindexrequestrequesttypedef)
- [DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef)
- [ListDataSourceSyncJobsRequestRequestTypeDef](./type_defs.md#listdatasourcesyncjobsrequestrequesttypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [MessageUsefulnessFeedbackTypeDef](./type_defs.md#messageusefulnessfeedbacktypedef)
- [DocumentContentTypeDef](./type_defs.md#documentcontenttypedef)
- [GetChatControlsConfigurationRequestGetChatControlsConfigurationPaginateTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestgetchatcontrolsconfigurationpaginatetypedef)
- [ListApplicationsRequestListApplicationsPaginateTypeDef](./type_defs.md#listapplicationsrequestlistapplicationspaginatetypedef)
- [ListConversationsRequestListConversationsPaginateTypeDef](./type_defs.md#listconversationsrequestlistconversationspaginatetypedef)
- [ListDataSourceSyncJobsRequestListDataSourceSyncJobsPaginateTypeDef](./type_defs.md#listdatasourcesyncjobsrequestlistdatasourcesyncjobspaginatetypedef)
- [ListDataSourcesRequestListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesrequestlistdatasourcespaginatetypedef)
- [ListDocumentsRequestListDocumentsPaginateTypeDef](./type_defs.md#listdocumentsrequestlistdocumentspaginatetypedef)
- [ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef)
- [ListIndicesRequestListIndicesPaginateTypeDef](./type_defs.md#listindicesrequestlistindicespaginatetypedef)
- [ListMessagesRequestListMessagesPaginateTypeDef](./type_defs.md#listmessagesrequestlistmessagespaginatetypedef)
- [ListPluginsRequestListPluginsPaginateTypeDef](./type_defs.md#listpluginsrequestlistpluginspaginatetypedef)
- [ListRetrieversRequestListRetrieversPaginateTypeDef](./type_defs.md#listretrieversrequestlistretrieverspaginatetypedef)
- [ListWebExperiencesRequestListWebExperiencesPaginateTypeDef](./type_defs.md#listwebexperiencesrequestlistwebexperiencespaginatetypedef)
- [GroupMembersTypeDef](./type_defs.md#groupmemberstypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [IndexStatisticsTypeDef](./type_defs.md#indexstatisticstypedef)
- [ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef)
- [ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef)
- [ListRetrieversResponseTypeDef](./type_defs.md#listretrieversresponsetypedef)
- [ListWebExperiencesResponseTypeDef](./type_defs.md#listwebexperiencesresponsetypedef)
- [RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef)
- [PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef)
- [PrincipalTypeDef](./type_defs.md#principaltypedef)
- [WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef)
- [SourceAttributionTypeDef](./type_defs.md#sourceattributiontypedef)
- [ActionReviewTypeDef](./type_defs.md#actionreviewtypedef)
- [ChatSyncInputRequestTypeDef](./type_defs.md#chatsyncinputrequesttypedef)
- [ListDocumentsResponseTypeDef](./type_defs.md#listdocumentsresponsetypedef)
- [BatchDeleteDocumentResponseTypeDef](./type_defs.md#batchdeletedocumentresponsetypedef)
- [BatchPutDocumentResponseTypeDef](./type_defs.md#batchputdocumentresponsetypedef)
- [GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef)
- [RuleConfigurationTypeDef](./type_defs.md#ruleconfigurationtypedef)
- [ListDataSourceSyncJobsResponseTypeDef](./type_defs.md#listdatasourcesyncjobsresponsetypedef)
- [DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef)
- [DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef)
- [DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef)
- [PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef)
- [PutGroupRequestRequestTypeDef](./type_defs.md#putgrouprequestrequesttypedef)
- [GetIndexResponseTypeDef](./type_defs.md#getindexresponsetypedef)
- [CreateRetrieverRequestRequestTypeDef](./type_defs.md#createretrieverrequestrequesttypedef)
- [GetRetrieverResponseTypeDef](./type_defs.md#getretrieverresponsetypedef)
- [UpdateRetrieverRequestRequestTypeDef](./type_defs.md#updateretrieverrequestrequesttypedef)
- [CreatePluginRequestRequestTypeDef](./type_defs.md#createpluginrequestrequesttypedef)
- [GetPluginResponseTypeDef](./type_defs.md#getpluginresponsetypedef)
- [UpdatePluginRequestRequestTypeDef](./type_defs.md#updatepluginrequestrequesttypedef)
- [AccessControlTypeDef](./type_defs.md#accesscontroltypedef)
- [GetWebExperienceResponseTypeDef](./type_defs.md#getwebexperienceresponsetypedef)
- [UpdateWebExperienceRequestRequestTypeDef](./type_defs.md#updatewebexperiencerequestrequesttypedef)
- [ChatSyncOutputTypeDef](./type_defs.md#chatsyncoutputtypedef)
- [MessagePaginatorTypeDef](./type_defs.md#messagepaginatortypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef)
- [InlineDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinedocumentenrichmentconfigurationtypedef)
- [AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef)
- [AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef)
- [ListMessagesResponsePaginatorTypeDef](./type_defs.md#listmessagesresponsepaginatortypedef)
- [ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef)
- [TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef)
- [DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef)
- [GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef)
- [UpdateChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#updatechatcontrolsconfigurationrequestrequesttypedef)
- [CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [BatchPutDocumentRequestRequestTypeDef](./type_defs.md#batchputdocumentrequestrequesttypedef)

