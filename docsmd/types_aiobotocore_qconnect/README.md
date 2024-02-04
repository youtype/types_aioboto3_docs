# QConnect module

> [Index](../README.md) > QConnect


!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `QConnect` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[qconnect]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[qconnect]'


# standalone installation
python -m pip install types-aiobotocore-qconnect
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qconnect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QConnectClient

Type annotations and code completion for  `#!python session.client("qconnect")` as [QConnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client)

```python
# QConnectClient usage example

from aioboto3.session import Session

from types_aiobotocore_qconnect.client import QConnectClient


session = Session()
async with session.client("qconnect") as client:
    client: QConnectClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("qconnect").get_paginator("...")`.

```python
# ListAssistantAssociationsPaginator usage example

from types_aiobotocore_qconnect.paginator import ListAssistantAssociationsPaginator

def get_list_assistant_associations_paginator() -> ListAssistantAssociationsPaginator:
    return client.get_paginator("list_assistant_associations"))
```

- [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
- [ListAssistantsPaginator](./paginators.md#listassistantspaginator)
- [ListContentsPaginator](./paginators.md#listcontentspaginator)
- [ListImportJobsPaginator](./paginators.md#listimportjobspaginator)
- [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
- [ListQuickResponsesPaginator](./paginators.md#listquickresponsespaginator)
- [QueryAssistantPaginator](./paginators.md#queryassistantpaginator)
- [SearchContentPaginator](./paginators.md#searchcontentpaginator)
- [SearchQuickResponsesPaginator](./paginators.md#searchquickresponsespaginator)
- [SearchSessionsPaginator](./paginators.md#searchsessionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AssistantCapabilityTypeType usage example

from types_aiobotocore_qconnect.literals import AssistantCapabilityTypeType

def get_value() -> AssistantCapabilityTypeType:
    return "V1"
```

- [AssistantCapabilityTypeType](./literals.md#assistantcapabilitytypetype)
- [AssistantStatusType](./literals.md#assistantstatustype)
- [AssistantTypeType](./literals.md#assistanttypetype)
- [AssociationTypeType](./literals.md#associationtypetype)
- [ContentStatusType](./literals.md#contentstatustype)
- [ExternalSourceType](./literals.md#externalsourcetype)
- [FilterFieldType](./literals.md#filterfieldtype)
- [FilterOperatorType](./literals.md#filteroperatortype)
- [ImportJobStatusType](./literals.md#importjobstatustype)
- [ImportJobTypeType](./literals.md#importjobtypetype)
- [KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)
- [KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype)
- [ListAssistantAssociationsPaginatorName](./literals.md#listassistantassociationspaginatorname)
- [ListAssistantsPaginatorName](./literals.md#listassistantspaginatorname)
- [ListContentsPaginatorName](./literals.md#listcontentspaginatorname)
- [ListImportJobsPaginatorName](./literals.md#listimportjobspaginatorname)
- [ListKnowledgeBasesPaginatorName](./literals.md#listknowledgebasespaginatorname)
- [ListQuickResponsesPaginatorName](./literals.md#listquickresponsespaginatorname)
- [OrderType](./literals.md#ordertype)
- [PriorityType](./literals.md#prioritytype)
- [QueryAssistantPaginatorName](./literals.md#queryassistantpaginatorname)
- [QueryConditionComparisonOperatorType](./literals.md#queryconditioncomparisonoperatortype)
- [QueryConditionFieldNameType](./literals.md#queryconditionfieldnametype)
- [QueryResultTypeType](./literals.md#queryresulttypetype)
- [QuickResponseFilterOperatorType](./literals.md#quickresponsefilteroperatortype)
- [QuickResponseQueryOperatorType](./literals.md#quickresponsequeryoperatortype)
- [QuickResponseStatusType](./literals.md#quickresponsestatustype)
- [RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype)
- [RecommendationTriggerTypeType](./literals.md#recommendationtriggertypetype)
- [RecommendationTypeType](./literals.md#recommendationtypetype)
- [RelevanceLevelType](./literals.md#relevanceleveltype)
- [RelevanceType](./literals.md#relevancetype)
- [SearchContentPaginatorName](./literals.md#searchcontentpaginatorname)
- [SearchQuickResponsesPaginatorName](./literals.md#searchquickresponsespaginatorname)
- [SearchSessionsPaginatorName](./literals.md#searchsessionspaginatorname)
- [SourceContentTypeType](./literals.md#sourcecontenttypetype)
- [TargetTypeType](./literals.md#targettypetype)
- [QConnectServiceName](./literals.md#qconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AppIntegrationsConfigurationPaginatorTypeDef](./type_defs.md#appintegrationsconfigurationpaginatortypedef)
- [AppIntegrationsConfigurationTypeDef](./type_defs.md#appintegrationsconfigurationtypedef)
- [AssistantAssociationInputDataTypeDef](./type_defs.md#assistantassociationinputdatatypedef)
- [KnowledgeBaseAssociationDataTypeDef](./type_defs.md#knowledgebaseassociationdatatypedef)
- [AssistantCapabilityConfigurationTypeDef](./type_defs.md#assistantcapabilityconfigurationtypedef)
- [AssistantIntegrationConfigurationTypeDef](./type_defs.md#assistantintegrationconfigurationtypedef)
- [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- [ConnectConfigurationTypeDef](./type_defs.md#connectconfigurationtypedef)
- [RankingDataTypeDef](./type_defs.md#rankingdatatypedef)
- [ContentDataTypeDef](./type_defs.md#contentdatatypedef)
- [GenerativeContentFeedbackDataTypeDef](./type_defs.md#generativecontentfeedbackdatatypedef)
- [ContentReferenceTypeDef](./type_defs.md#contentreferencetypedef)
- [ContentSummaryTypeDef](./type_defs.md#contentsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateContentRequestRequestTypeDef](./type_defs.md#createcontentrequestrequesttypedef)
- [RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef)
- [GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef)
- [QuickResponseDataProviderTypeDef](./type_defs.md#quickresponsedataprovidertypedef)
- [CreateSessionRequestRequestTypeDef](./type_defs.md#createsessionrequestrequesttypedef)
- [GenerativeReferenceTypeDef](./type_defs.md#generativereferencetypedef)
- [DeleteAssistantAssociationRequestRequestTypeDef](./type_defs.md#deleteassistantassociationrequestrequesttypedef)
- [DeleteAssistantRequestRequestTypeDef](./type_defs.md#deleteassistantrequestrequesttypedef)
- [DeleteContentRequestRequestTypeDef](./type_defs.md#deletecontentrequestrequesttypedef)
- [DeleteImportJobRequestRequestTypeDef](./type_defs.md#deleteimportjobrequestrequesttypedef)
- [DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef)
- [DeleteQuickResponseRequestRequestTypeDef](./type_defs.md#deletequickresponserequestrequesttypedef)
- [HighlightTypeDef](./type_defs.md#highlighttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetAssistantAssociationRequestRequestTypeDef](./type_defs.md#getassistantassociationrequestrequesttypedef)
- [GetAssistantRequestRequestTypeDef](./type_defs.md#getassistantrequestrequesttypedef)
- [GetContentRequestRequestTypeDef](./type_defs.md#getcontentrequestrequesttypedef)
- [GetContentSummaryRequestRequestTypeDef](./type_defs.md#getcontentsummaryrequestrequesttypedef)
- [GetImportJobRequestRequestTypeDef](./type_defs.md#getimportjobrequestrequesttypedef)
- [GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef)
- [GetQuickResponseRequestRequestTypeDef](./type_defs.md#getquickresponserequestrequesttypedef)
- [GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [GroupingConfigurationPaginatorTypeDef](./type_defs.md#groupingconfigurationpaginatortypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAssistantAssociationsRequestRequestTypeDef](./type_defs.md#listassistantassociationsrequestrequesttypedef)
- [ListAssistantsRequestRequestTypeDef](./type_defs.md#listassistantsrequestrequesttypedef)
- [ListContentsRequestRequestTypeDef](./type_defs.md#listcontentsrequestrequesttypedef)
- [ListImportJobsRequestRequestTypeDef](./type_defs.md#listimportjobsrequestrequesttypedef)
- [ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef)
- [ListQuickResponsesRequestRequestTypeDef](./type_defs.md#listquickresponsesrequestrequesttypedef)
- [QuickResponseSummaryTypeDef](./type_defs.md#quickresponsesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [NotifyRecommendationsReceivedErrorTypeDef](./type_defs.md#notifyrecommendationsreceivederrortypedef)
- [NotifyRecommendationsReceivedRequestRequestTypeDef](./type_defs.md#notifyrecommendationsreceivedrequestrequesttypedef)
- [QueryConditionItemTypeDef](./type_defs.md#queryconditionitemtypedef)
- [QueryRecommendationTriggerDataTypeDef](./type_defs.md#queryrecommendationtriggerdatatypedef)
- [QuickResponseContentProviderTypeDef](./type_defs.md#quickresponsecontentprovidertypedef)
- [QuickResponseFilterFieldTypeDef](./type_defs.md#quickresponsefilterfieldtypedef)
- [QuickResponseOrderFieldTypeDef](./type_defs.md#quickresponseorderfieldtypedef)
- [QuickResponseQueryFieldTypeDef](./type_defs.md#quickresponsequeryfieldtypedef)
- [RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#removeknowledgebasetemplateurirequestrequesttypedef)
- [SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef)
- [SessionIntegrationConfigurationTypeDef](./type_defs.md#sessionintegrationconfigurationtypedef)
- [StartContentUploadRequestRequestTypeDef](./type_defs.md#startcontentuploadrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateContentRequestRequestTypeDef](./type_defs.md#updatecontentrequestrequesttypedef)
- [UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#updateknowledgebasetemplateurirequestrequesttypedef)
- [SourceConfigurationPaginatorTypeDef](./type_defs.md#sourceconfigurationpaginatortypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [CreateAssistantAssociationRequestRequestTypeDef](./type_defs.md#createassistantassociationrequestrequesttypedef)
- [AssistantAssociationOutputDataTypeDef](./type_defs.md#assistantassociationoutputdatatypedef)
- [AssistantDataTypeDef](./type_defs.md#assistantdatatypedef)
- [AssistantSummaryTypeDef](./type_defs.md#assistantsummarytypedef)
- [CreateAssistantRequestRequestTypeDef](./type_defs.md#createassistantrequestrequesttypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [GenerativeDataDetailsTypeDef](./type_defs.md#generativedatadetailstypedef)
- [ContentFeedbackDataTypeDef](./type_defs.md#contentfeedbackdatatypedef)
- [CreateContentResponseTypeDef](./type_defs.md#createcontentresponsetypedef)
- [GetContentResponseTypeDef](./type_defs.md#getcontentresponsetypedef)
- [GetContentSummaryResponseTypeDef](./type_defs.md#getcontentsummaryresponsetypedef)
- [ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef)
- [StartContentUploadResponseTypeDef](./type_defs.md#startcontentuploadresponsetypedef)
- [UpdateContentResponseTypeDef](./type_defs.md#updatecontentresponsetypedef)
- [CreateQuickResponseRequestRequestTypeDef](./type_defs.md#createquickresponserequestrequesttypedef)
- [UpdateQuickResponseRequestRequestTypeDef](./type_defs.md#updatequickresponserequestrequesttypedef)
- [DataReferenceTypeDef](./type_defs.md#datareferencetypedef)
- [DocumentTextTypeDef](./type_defs.md#documenttexttypedef)
- [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
- [ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef](./type_defs.md#listassistantassociationsrequestlistassistantassociationspaginatetypedef)
- [ListAssistantsRequestListAssistantsPaginateTypeDef](./type_defs.md#listassistantsrequestlistassistantspaginatetypedef)
- [ListContentsRequestListContentsPaginateTypeDef](./type_defs.md#listcontentsrequestlistcontentspaginatetypedef)
- [ListImportJobsRequestListImportJobsPaginateTypeDef](./type_defs.md#listimportjobsrequestlistimportjobspaginatetypedef)
- [ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef](./type_defs.md#listknowledgebasesrequestlistknowledgebasespaginatetypedef)
- [ListQuickResponsesRequestListQuickResponsesPaginateTypeDef](./type_defs.md#listquickresponsesrequestlistquickresponsespaginatetypedef)
- [ListQuickResponsesResponseTypeDef](./type_defs.md#listquickresponsesresponsetypedef)
- [NotifyRecommendationsReceivedResponseTypeDef](./type_defs.md#notifyrecommendationsreceivedresponsetypedef)
- [QueryConditionTypeDef](./type_defs.md#queryconditiontypedef)
- [RecommendationTriggerDataTypeDef](./type_defs.md#recommendationtriggerdatatypedef)
- [QuickResponseContentsTypeDef](./type_defs.md#quickresponsecontentstypedef)
- [QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef)
- [SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef)
- [SessionDataTypeDef](./type_defs.md#sessiondatatypedef)
- [KnowledgeBaseSummaryPaginatorTypeDef](./type_defs.md#knowledgebasesummarypaginatortypedef)
- [CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef)
- [KnowledgeBaseDataTypeDef](./type_defs.md#knowledgebasedatatypedef)
- [KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef)
- [AssistantAssociationDataTypeDef](./type_defs.md#assistantassociationdatatypedef)
- [AssistantAssociationSummaryTypeDef](./type_defs.md#assistantassociationsummarytypedef)
- [CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef)
- [GetAssistantResponseTypeDef](./type_defs.md#getassistantresponsetypedef)
- [ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef)
- [ExternalSourceConfigurationTypeDef](./type_defs.md#externalsourceconfigurationtypedef)
- [PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef)
- [PutFeedbackResponseTypeDef](./type_defs.md#putfeedbackresponsetypedef)
- [DataSummaryTypeDef](./type_defs.md#datasummarytypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [TextDataTypeDef](./type_defs.md#textdatatypedef)
- [SearchContentRequestRequestTypeDef](./type_defs.md#searchcontentrequestrequesttypedef)
- [SearchContentRequestSearchContentPaginateTypeDef](./type_defs.md#searchcontentrequestsearchcontentpaginatetypedef)
- [SearchSessionsRequestRequestTypeDef](./type_defs.md#searchsessionsrequestrequesttypedef)
- [SearchSessionsRequestSearchSessionsPaginateTypeDef](./type_defs.md#searchsessionsrequestsearchsessionspaginatetypedef)
- [QueryAssistantRequestQueryAssistantPaginateTypeDef](./type_defs.md#queryassistantrequestqueryassistantpaginatetypedef)
- [QueryAssistantRequestRequestTypeDef](./type_defs.md#queryassistantrequestrequesttypedef)
- [RecommendationTriggerTypeDef](./type_defs.md#recommendationtriggertypedef)
- [QuickResponseDataTypeDef](./type_defs.md#quickresponsedatatypedef)
- [QuickResponseSearchResultDataPaginatorTypeDef](./type_defs.md#quickresponsesearchresultdatapaginatortypedef)
- [QuickResponseSearchResultDataTypeDef](./type_defs.md#quickresponsesearchresultdatatypedef)
- [SearchQuickResponsesRequestRequestTypeDef](./type_defs.md#searchquickresponsesrequestrequesttypedef)
- [SearchQuickResponsesRequestSearchQuickResponsesPaginateTypeDef](./type_defs.md#searchquickresponsesrequestsearchquickresponsespaginatetypedef)
- [CreateSessionResponseTypeDef](./type_defs.md#createsessionresponsetypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [ListKnowledgeBasesResponsePaginatorTypeDef](./type_defs.md#listknowledgebasesresponsepaginatortypedef)
- [CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef)
- [GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef)
- [UpdateKnowledgeBaseTemplateUriResponseTypeDef](./type_defs.md#updateknowledgebasetemplateuriresponsetypedef)
- [ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef)
- [CreateAssistantAssociationResponseTypeDef](./type_defs.md#createassistantassociationresponsetypedef)
- [GetAssistantAssociationResponseTypeDef](./type_defs.md#getassistantassociationresponsetypedef)
- [ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef)
- [ImportJobDataTypeDef](./type_defs.md#importjobdatatypedef)
- [ImportJobSummaryTypeDef](./type_defs.md#importjobsummarytypedef)
- [StartImportJobRequestRequestTypeDef](./type_defs.md#startimportjobrequestrequesttypedef)
- [RecommendationDataTypeDef](./type_defs.md#recommendationdatatypedef)
- [ResultDataTypeDef](./type_defs.md#resultdatatypedef)
- [ContentDataDetailsTypeDef](./type_defs.md#contentdatadetailstypedef)
- [SourceContentDataDetailsTypeDef](./type_defs.md#sourcecontentdatadetailstypedef)
- [CreateQuickResponseResponseTypeDef](./type_defs.md#createquickresponseresponsetypedef)
- [GetQuickResponseResponseTypeDef](./type_defs.md#getquickresponseresponsetypedef)
- [UpdateQuickResponseResponseTypeDef](./type_defs.md#updatequickresponseresponsetypedef)
- [SearchQuickResponsesResponsePaginatorTypeDef](./type_defs.md#searchquickresponsesresponsepaginatortypedef)
- [SearchQuickResponsesResponseTypeDef](./type_defs.md#searchquickresponsesresponsetypedef)
- [GetImportJobResponseTypeDef](./type_defs.md#getimportjobresponsetypedef)
- [StartImportJobResponseTypeDef](./type_defs.md#startimportjobresponsetypedef)
- [ListImportJobsResponseTypeDef](./type_defs.md#listimportjobsresponsetypedef)
- [GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef)
- [QueryAssistantResponseTypeDef](./type_defs.md#queryassistantresponsetypedef)
- [DataDetailsTypeDef](./type_defs.md#datadetailstypedef)

