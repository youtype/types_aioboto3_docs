# AgentsforBedrock module

> [Index](../README.md) > AgentsforBedrock


!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `AgentsforBedrock` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[bedrock-agent]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[bedrock-agent]'


# standalone installation
python -m pip install types-aiobotocore-bedrock-agent
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-agent
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AgentsforBedrockClient

Type annotations and code completion for  `#!python session.client("bedrock-agent")` as [AgentsforBedrockClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client)

```python
# AgentsforBedrockClient usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient


session = Session()
async with session.client("bedrock-agent") as client:
    client: AgentsforBedrockClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.client("bedrock-agent").get_paginator("...")`.

```python
# ListAgentActionGroupsPaginator usage example

from types_aiobotocore_bedrock_agent.paginator import ListAgentActionGroupsPaginator

def get_list_agent_action_groups_paginator() -> ListAgentActionGroupsPaginator:
    return client.get_paginator("list_agent_action_groups"))
```

- [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
- [ListAgentAliasesPaginator](./paginators.md#listagentaliasespaginator)
- [ListAgentKnowledgeBasesPaginator](./paginators.md#listagentknowledgebasespaginator)
- [ListAgentVersionsPaginator](./paginators.md#listagentversionspaginator)
- [ListAgentsPaginator](./paginators.md#listagentspaginator)
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListIngestionJobsPaginator](./paginators.md#listingestionjobspaginator)
- [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionGroupSignatureType usage example

from types_aiobotocore_bedrock_agent.literals import ActionGroupSignatureType

def get_value() -> ActionGroupSignatureType:
    return "AMAZON.UserInput"
```

- [ActionGroupSignatureType](./literals.md#actiongroupsignaturetype)
- [ActionGroupStateType](./literals.md#actiongroupstatetype)
- [AgentAliasStatusType](./literals.md#agentaliasstatustype)
- [AgentStatusType](./literals.md#agentstatustype)
- [ChunkingStrategyType](./literals.md#chunkingstrategytype)
- [CreationModeType](./literals.md#creationmodetype)
- [DataSourceStatusType](./literals.md#datasourcestatustype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [IngestionJobFilterAttributeType](./literals.md#ingestionjobfilterattributetype)
- [IngestionJobFilterOperatorType](./literals.md#ingestionjobfilteroperatortype)
- [IngestionJobSortByAttributeType](./literals.md#ingestionjobsortbyattributetype)
- [IngestionJobStatusType](./literals.md#ingestionjobstatustype)
- [KnowledgeBaseStateType](./literals.md#knowledgebasestatetype)
- [KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)
- [KnowledgeBaseStorageTypeType](./literals.md#knowledgebasestoragetypetype)
- [KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype)
- [ListAgentActionGroupsPaginatorName](./literals.md#listagentactiongroupspaginatorname)
- [ListAgentAliasesPaginatorName](./literals.md#listagentaliasespaginatorname)
- [ListAgentKnowledgeBasesPaginatorName](./literals.md#listagentknowledgebasespaginatorname)
- [ListAgentVersionsPaginatorName](./literals.md#listagentversionspaginatorname)
- [ListAgentsPaginatorName](./literals.md#listagentspaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListIngestionJobsPaginatorName](./literals.md#listingestionjobspaginatorname)
- [ListKnowledgeBasesPaginatorName](./literals.md#listknowledgebasespaginatorname)
- [PromptStateType](./literals.md#promptstatetype)
- [PromptTypeType](./literals.md#prompttypetype)
- [SortOrderType](./literals.md#sortordertype)
- [AgentsforBedrockServiceName](./literals.md#agentsforbedrockservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [S3IdentifierTypeDef](./type_defs.md#s3identifiertypedef)
- [ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef)
- [ActionGroupSummaryTypeDef](./type_defs.md#actiongroupsummarytypedef)
- [AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef)
- [AgentKnowledgeBaseSummaryTypeDef](./type_defs.md#agentknowledgebasesummarytypedef)
- [AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef)
- [AgentSummaryTypeDef](./type_defs.md#agentsummarytypedef)
- [AgentVersionSummaryTypeDef](./type_defs.md#agentversionsummarytypedef)
- [AssociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#associateagentknowledgebaserequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef)
- [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- [S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef)
- [DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef)
- [DeleteAgentActionGroupRequestRequestTypeDef](./type_defs.md#deleteagentactiongrouprequestrequesttypedef)
- [DeleteAgentAliasRequestRequestTypeDef](./type_defs.md#deleteagentaliasrequestrequesttypedef)
- [DeleteAgentRequestRequestTypeDef](./type_defs.md#deleteagentrequestrequesttypedef)
- [DeleteAgentVersionRequestRequestTypeDef](./type_defs.md#deleteagentversionrequestrequesttypedef)
- [DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef)
- [DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef)
- [DisassociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#disassociateagentknowledgebaserequestrequesttypedef)
- [GetAgentActionGroupRequestRequestTypeDef](./type_defs.md#getagentactiongrouprequestrequesttypedef)
- [GetAgentAliasRequestRequestTypeDef](./type_defs.md#getagentaliasrequestrequesttypedef)
- [GetAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getagentknowledgebaserequestrequesttypedef)
- [GetAgentRequestRequestTypeDef](./type_defs.md#getagentrequestrequesttypedef)
- [GetAgentVersionRequestRequestTypeDef](./type_defs.md#getagentversionrequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetIngestionJobRequestRequestTypeDef](./type_defs.md#getingestionjobrequestrequesttypedef)
- [GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef)
- [InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
- [IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef)
- [IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef)
- [IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef)
- [VectorKnowledgeBaseConfigurationTypeDef](./type_defs.md#vectorknowledgebaseconfigurationtypedef)
- [KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAgentActionGroupsRequestRequestTypeDef](./type_defs.md#listagentactiongroupsrequestrequesttypedef)
- [ListAgentAliasesRequestRequestTypeDef](./type_defs.md#listagentaliasesrequestrequesttypedef)
- [ListAgentKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listagentknowledgebasesrequestrequesttypedef)
- [ListAgentVersionsRequestRequestTypeDef](./type_defs.md#listagentversionsrequestrequesttypedef)
- [ListAgentsRequestRequestTypeDef](./type_defs.md#listagentsrequestrequesttypedef)
- [ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef)
- [ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [OpenSearchServerlessFieldMappingTypeDef](./type_defs.md#opensearchserverlessfieldmappingtypedef)
- [PineconeFieldMappingTypeDef](./type_defs.md#pineconefieldmappingtypedef)
- [PrepareAgentRequestRequestTypeDef](./type_defs.md#prepareagentrequestrequesttypedef)
- [RdsFieldMappingTypeDef](./type_defs.md#rdsfieldmappingtypedef)
- [RedisEnterpriseCloudFieldMappingTypeDef](./type_defs.md#redisenterprisecloudfieldmappingtypedef)
- [StartIngestionJobRequestRequestTypeDef](./type_defs.md#startingestionjobrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateagentknowledgebaserequestrequesttypedef)
- [APISchemaTypeDef](./type_defs.md#apischematypedef)
- [AgentAliasHistoryEventTypeDef](./type_defs.md#agentaliashistoryeventtypedef)
- [AgentAliasSummaryTypeDef](./type_defs.md#agentaliassummarytypedef)
- [CreateAgentAliasRequestRequestTypeDef](./type_defs.md#createagentaliasrequestrequesttypedef)
- [UpdateAgentAliasRequestRequestTypeDef](./type_defs.md#updateagentaliasrequestrequesttypedef)
- [AssociateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#associateagentknowledgebaseresponsetypedef)
- [DeleteAgentAliasResponseTypeDef](./type_defs.md#deleteagentaliasresponsetypedef)
- [DeleteAgentResponseTypeDef](./type_defs.md#deleteagentresponsetypedef)
- [DeleteAgentVersionResponseTypeDef](./type_defs.md#deleteagentversionresponsetypedef)
- [DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef)
- [DeleteKnowledgeBaseResponseTypeDef](./type_defs.md#deleteknowledgebaseresponsetypedef)
- [GetAgentKnowledgeBaseResponseTypeDef](./type_defs.md#getagentknowledgebaseresponsetypedef)
- [ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef)
- [ListAgentKnowledgeBasesResponseTypeDef](./type_defs.md#listagentknowledgebasesresponsetypedef)
- [ListAgentVersionsResponseTypeDef](./type_defs.md#listagentversionsresponsetypedef)
- [ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PrepareAgentResponseTypeDef](./type_defs.md#prepareagentresponsetypedef)
- [UpdateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#updateagentknowledgebaseresponsetypedef)
- [ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef)
- [DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef)
- [ListIngestionJobsRequestRequestTypeDef](./type_defs.md#listingestionjobsrequestrequesttypedef)
- [IngestionJobSummaryTypeDef](./type_defs.md#ingestionjobsummarytypedef)
- [IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef)
- [KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef)
- [ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef)
- [ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef](./type_defs.md#listagentactiongroupsrequestlistagentactiongroupspaginatetypedef)
- [ListAgentAliasesRequestListAgentAliasesPaginateTypeDef](./type_defs.md#listagentaliasesrequestlistagentaliasespaginatetypedef)
- [ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef](./type_defs.md#listagentknowledgebasesrequestlistagentknowledgebasespaginatetypedef)
- [ListAgentVersionsRequestListAgentVersionsPaginateTypeDef](./type_defs.md#listagentversionsrequestlistagentversionspaginatetypedef)
- [ListAgentsRequestListAgentsPaginateTypeDef](./type_defs.md#listagentsrequestlistagentspaginatetypedef)
- [ListDataSourcesRequestListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesrequestlistdatasourcespaginatetypedef)
- [ListIngestionJobsRequestListIngestionJobsPaginateTypeDef](./type_defs.md#listingestionjobsrequestlistingestionjobspaginatetypedef)
- [ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef](./type_defs.md#listknowledgebasesrequestlistknowledgebasespaginatetypedef)
- [OpenSearchServerlessConfigurationTypeDef](./type_defs.md#opensearchserverlessconfigurationtypedef)
- [PineconeConfigurationTypeDef](./type_defs.md#pineconeconfigurationtypedef)
- [RdsConfigurationTypeDef](./type_defs.md#rdsconfigurationtypedef)
- [RedisEnterpriseCloudConfigurationTypeDef](./type_defs.md#redisenterprisecloudconfigurationtypedef)
- [AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef)
- [CreateAgentActionGroupRequestRequestTypeDef](./type_defs.md#createagentactiongrouprequestrequesttypedef)
- [UpdateAgentActionGroupRequestRequestTypeDef](./type_defs.md#updateagentactiongrouprequestrequesttypedef)
- [AgentAliasTypeDef](./type_defs.md#agentaliastypedef)
- [ListAgentAliasesResponseTypeDef](./type_defs.md#listagentaliasesresponsetypedef)
- [VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef)
- [PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef)
- [ListIngestionJobsResponseTypeDef](./type_defs.md#listingestionjobsresponsetypedef)
- [GetIngestionJobResponseTypeDef](./type_defs.md#getingestionjobresponsetypedef)
- [StartIngestionJobResponseTypeDef](./type_defs.md#startingestionjobresponsetypedef)
- [StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)
- [CreateAgentActionGroupResponseTypeDef](./type_defs.md#createagentactiongroupresponsetypedef)
- [GetAgentActionGroupResponseTypeDef](./type_defs.md#getagentactiongroupresponsetypedef)
- [UpdateAgentActionGroupResponseTypeDef](./type_defs.md#updateagentactiongroupresponsetypedef)
- [CreateAgentAliasResponseTypeDef](./type_defs.md#createagentaliasresponsetypedef)
- [GetAgentAliasResponseTypeDef](./type_defs.md#getagentaliasresponsetypedef)
- [UpdateAgentAliasResponseTypeDef](./type_defs.md#updateagentaliasresponsetypedef)
- [CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [AgentTypeDef](./type_defs.md#agenttypedef)
- [AgentVersionTypeDef](./type_defs.md#agentversiontypedef)
- [CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef)
- [UpdateAgentRequestRequestTypeDef](./type_defs.md#updateagentrequestrequesttypedef)
- [CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef)
- [KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef)
- [UpdateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateknowledgebaserequestrequesttypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef)
- [CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef)
- [GetAgentResponseTypeDef](./type_defs.md#getagentresponsetypedef)
- [UpdateAgentResponseTypeDef](./type_defs.md#updateagentresponsetypedef)
- [GetAgentVersionResponseTypeDef](./type_defs.md#getagentversionresponsetypedef)
- [CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef)
- [GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef)
- [UpdateKnowledgeBaseResponseTypeDef](./type_defs.md#updateknowledgebaseresponsetypedef)

