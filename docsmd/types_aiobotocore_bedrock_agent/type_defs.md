# Type definitions

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).



## S3IdentifierTypeDef

```python
# S3IdentifierTypeDef definition

class S3IdentifierTypeDef(TypedDict):
    s3BucketName: NotRequired[str],
    s3ObjectKey: NotRequired[str],
```

## ActionGroupExecutorTypeDef

```python
# ActionGroupExecutorTypeDef definition

class ActionGroupExecutorTypeDef(TypedDict):
    lambda: NotRequired[str],
```

## ActionGroupSummaryTypeDef

```python
# ActionGroupSummaryTypeDef definition

class ActionGroupSummaryTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    actionGroupState: ActionGroupStateType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
## AgentAliasRoutingConfigurationListItemTypeDef

```python
# AgentAliasRoutingConfigurationListItemTypeDef definition

class AgentAliasRoutingConfigurationListItemTypeDef(TypedDict):
    agentVersion: str,
```

## AgentKnowledgeBaseSummaryTypeDef

```python
# AgentKnowledgeBaseSummaryTypeDef definition

class AgentKnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    knowledgeBaseState: KnowledgeBaseStateType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## AgentKnowledgeBaseTypeDef

```python
# AgentKnowledgeBaseTypeDef definition

class AgentKnowledgeBaseTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: str,
    createdAt: datetime,
    updatedAt: datetime,
    knowledgeBaseState: KnowledgeBaseStateType,  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## AgentSummaryTypeDef

```python
# AgentSummaryTypeDef definition

class AgentSummaryTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentStatus: AgentStatusType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
    latestAgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
## AgentVersionSummaryTypeDef

```python
# AgentVersionSummaryTypeDef definition

class AgentVersionSummaryTypeDef(TypedDict):
    agentName: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
## AssociateAgentKnowledgeBaseRequestRequestTypeDef

```python
# AssociateAgentKnowledgeBaseRequestRequestTypeDef definition

class AssociateAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: str,
    knowledgeBaseState: NotRequired[KnowledgeBaseStateType],  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
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

## FixedSizeChunkingConfigurationTypeDef

```python
# FixedSizeChunkingConfigurationTypeDef definition

class FixedSizeChunkingConfigurationTypeDef(TypedDict):
    maxTokens: int,
    overlapPercentage: int,
```

## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    kmsKeyArn: NotRequired[str],
```

## S3DataSourceConfigurationTypeDef

```python
# S3DataSourceConfigurationTypeDef definition

class S3DataSourceConfigurationTypeDef(TypedDict):
    bucketArn: str,
    inclusionPrefixes: NotRequired[Sequence[str]],
```

## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    name: str,
    status: DataSourceStatusType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## DeleteAgentActionGroupRequestRequestTypeDef

```python
# DeleteAgentActionGroupRequestRequestTypeDef definition

class DeleteAgentActionGroupRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteAgentAliasRequestRequestTypeDef

```python
# DeleteAgentAliasRequestRequestTypeDef definition

class DeleteAgentAliasRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentAliasId: str,
```

## DeleteAgentRequestRequestTypeDef

```python
# DeleteAgentRequestRequestTypeDef definition

class DeleteAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteAgentVersionRequestRequestTypeDef

```python
# DeleteAgentVersionRequestRequestTypeDef definition

class DeleteAgentVersionRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteDataSourceRequestRequestTypeDef

```python
# DeleteDataSourceRequestRequestTypeDef definition

class DeleteDataSourceRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
```

## DeleteKnowledgeBaseRequestRequestTypeDef

```python
# DeleteKnowledgeBaseRequestRequestTypeDef definition

class DeleteKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## DisassociateAgentKnowledgeBaseRequestRequestTypeDef

```python
# DisassociateAgentKnowledgeBaseRequestRequestTypeDef definition

class DisassociateAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
```

## GetAgentActionGroupRequestRequestTypeDef

```python
# GetAgentActionGroupRequestRequestTypeDef definition

class GetAgentActionGroupRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
```

## GetAgentAliasRequestRequestTypeDef

```python
# GetAgentAliasRequestRequestTypeDef definition

class GetAgentAliasRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentAliasId: str,
```

## GetAgentKnowledgeBaseRequestRequestTypeDef

```python
# GetAgentKnowledgeBaseRequestRequestTypeDef definition

class GetAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
```

## GetAgentRequestRequestTypeDef

```python
# GetAgentRequestRequestTypeDef definition

class GetAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
```

## GetAgentVersionRequestRequestTypeDef

```python
# GetAgentVersionRequestRequestTypeDef definition

class GetAgentVersionRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
```

## GetDataSourceRequestRequestTypeDef

```python
# GetDataSourceRequestRequestTypeDef definition

class GetDataSourceRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
```

## GetIngestionJobRequestRequestTypeDef

```python
# GetIngestionJobRequestRequestTypeDef definition

class GetIngestionJobRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    ingestionJobId: str,
```

## GetKnowledgeBaseRequestRequestTypeDef

```python
# GetKnowledgeBaseRequestRequestTypeDef definition

class GetKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    temperature: NotRequired[float],
    topP: NotRequired[float],
    topK: NotRequired[int],
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
```

## IngestionJobFilterTypeDef

```python
# IngestionJobFilterTypeDef definition

class IngestionJobFilterTypeDef(TypedDict):
    attribute: IngestionJobFilterAttributeType,  # (1)
    operator: IngestionJobFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: IngestionJobFilterAttributeType](./literals.md#ingestionjobfilterattributetype) 
2. See [:material-code-brackets: IngestionJobFilterOperatorType](./literals.md#ingestionjobfilteroperatortype) 
## IngestionJobSortByTypeDef

```python
# IngestionJobSortByTypeDef definition

class IngestionJobSortByTypeDef(TypedDict):
    attribute: IngestionJobSortByAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: IngestionJobSortByAttributeType](./literals.md#ingestionjobsortbyattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## IngestionJobStatisticsTypeDef

```python
# IngestionJobStatisticsTypeDef definition

class IngestionJobStatisticsTypeDef(TypedDict):
    numberOfDocumentsScanned: NotRequired[int],
    numberOfNewDocumentsIndexed: NotRequired[int],
    numberOfModifiedDocumentsIndexed: NotRequired[int],
    numberOfDocumentsDeleted: NotRequired[int],
    numberOfDocumentsFailed: NotRequired[int],
```

## VectorKnowledgeBaseConfigurationTypeDef

```python
# VectorKnowledgeBaseConfigurationTypeDef definition

class VectorKnowledgeBaseConfigurationTypeDef(TypedDict):
    embeddingModelArn: str,
```

## KnowledgeBaseSummaryTypeDef

```python
# KnowledgeBaseSummaryTypeDef definition

class KnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    status: KnowledgeBaseStatusType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAgentActionGroupsRequestRequestTypeDef

```python
# ListAgentActionGroupsRequestRequestTypeDef definition

class ListAgentActionGroupsRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentAliasesRequestRequestTypeDef

```python
# ListAgentAliasesRequestRequestTypeDef definition

class ListAgentAliasesRequestRequestTypeDef(TypedDict):
    agentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentKnowledgeBasesRequestRequestTypeDef

```python
# ListAgentKnowledgeBasesRequestRequestTypeDef definition

class ListAgentKnowledgeBasesRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentVersionsRequestRequestTypeDef

```python
# ListAgentVersionsRequestRequestTypeDef definition

class ListAgentVersionsRequestRequestTypeDef(TypedDict):
    agentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentsRequestRequestTypeDef

```python
# ListAgentsRequestRequestTypeDef definition

class ListAgentsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataSourcesRequestRequestTypeDef

```python
# ListDataSourcesRequestRequestTypeDef definition

class ListDataSourcesRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListKnowledgeBasesRequestRequestTypeDef

```python
# ListKnowledgeBasesRequestRequestTypeDef definition

class ListKnowledgeBasesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## OpenSearchServerlessFieldMappingTypeDef

```python
# OpenSearchServerlessFieldMappingTypeDef definition

class OpenSearchServerlessFieldMappingTypeDef(TypedDict):
    vectorField: str,
    textField: str,
    metadataField: str,
```

## PineconeFieldMappingTypeDef

```python
# PineconeFieldMappingTypeDef definition

class PineconeFieldMappingTypeDef(TypedDict):
    textField: str,
    metadataField: str,
```

## PrepareAgentRequestRequestTypeDef

```python
# PrepareAgentRequestRequestTypeDef definition

class PrepareAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
```

## RdsFieldMappingTypeDef

```python
# RdsFieldMappingTypeDef definition

class RdsFieldMappingTypeDef(TypedDict):
    primaryKeyField: str,
    vectorField: str,
    textField: str,
    metadataField: str,
```

## RedisEnterpriseCloudFieldMappingTypeDef

```python
# RedisEnterpriseCloudFieldMappingTypeDef definition

class RedisEnterpriseCloudFieldMappingTypeDef(TypedDict):
    vectorField: str,
    textField: str,
    metadataField: str,
```

## StartIngestionJobRequestRequestTypeDef

```python
# StartIngestionJobRequestRequestTypeDef definition

class StartIngestionJobRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAgentKnowledgeBaseRequestRequestTypeDef

```python
# UpdateAgentKnowledgeBaseRequestRequestTypeDef definition

class UpdateAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: NotRequired[str],
    knowledgeBaseState: NotRequired[KnowledgeBaseStateType],  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## APISchemaTypeDef

```python
# APISchemaTypeDef definition

class APISchemaTypeDef(TypedDict):
    s3: NotRequired[S3IdentifierTypeDef],  # (1)
    payload: NotRequired[str],
```

1. See [:material-code-braces: S3IdentifierTypeDef](./type_defs.md#s3identifiertypedef) 
## AgentAliasHistoryEventTypeDef

```python
# AgentAliasHistoryEventTypeDef definition

class AgentAliasHistoryEventTypeDef(TypedDict):
    routingConfiguration: NotRequired[List[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
    endDate: NotRequired[datetime],
    startDate: NotRequired[datetime],
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## AgentAliasSummaryTypeDef

```python
# AgentAliasSummaryTypeDef definition

class AgentAliasSummaryTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasName: str,
    agentAliasStatus: AgentAliasStatusType,  # (2)
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    routingConfiguration: NotRequired[List[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype) 
## CreateAgentAliasRequestRequestTypeDef

```python
# CreateAgentAliasRequestRequestTypeDef definition

class CreateAgentAliasRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentAliasName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## UpdateAgentAliasRequestRequestTypeDef

```python
# UpdateAgentAliasRequestRequestTypeDef definition

class UpdateAgentAliasRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentAliasId: str,
    agentAliasName: str,
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## AssociateAgentKnowledgeBaseResponseTypeDef

```python
# AssociateAgentKnowledgeBaseResponseTypeDef definition

class AssociateAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAgentAliasResponseTypeDef

```python
# DeleteAgentAliasResponseTypeDef definition

class DeleteAgentAliasResponseTypeDef(TypedDict):
    agentId: str,
    agentAliasId: str,
    agentAliasStatus: AgentAliasStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAgentResponseTypeDef

```python
# DeleteAgentResponseTypeDef definition

class DeleteAgentResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAgentVersionResponseTypeDef

```python
# DeleteAgentVersionResponseTypeDef definition

class DeleteAgentVersionResponseTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    agentStatus: AgentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSourceResponseTypeDef

```python
# DeleteDataSourceResponseTypeDef definition

class DeleteDataSourceResponseTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    status: DataSourceStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKnowledgeBaseResponseTypeDef

```python
# DeleteKnowledgeBaseResponseTypeDef definition

class DeleteKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBaseId: str,
    status: KnowledgeBaseStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentKnowledgeBaseResponseTypeDef

```python
# GetAgentKnowledgeBaseResponseTypeDef definition

class GetAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentActionGroupsResponseTypeDef

```python
# ListAgentActionGroupsResponseTypeDef definition

class ListAgentActionGroupsResponseTypeDef(TypedDict):
    actionGroupSummaries: List[ActionGroupSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionGroupSummaryTypeDef](./type_defs.md#actiongroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentKnowledgeBasesResponseTypeDef

```python
# ListAgentKnowledgeBasesResponseTypeDef definition

class ListAgentKnowledgeBasesResponseTypeDef(TypedDict):
    agentKnowledgeBaseSummaries: List[AgentKnowledgeBaseSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseSummaryTypeDef](./type_defs.md#agentknowledgebasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentVersionsResponseTypeDef

```python
# ListAgentVersionsResponseTypeDef definition

class ListAgentVersionsResponseTypeDef(TypedDict):
    agentVersionSummaries: List[AgentVersionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentVersionSummaryTypeDef](./type_defs.md#agentversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentsResponseTypeDef

```python
# ListAgentsResponseTypeDef definition

class ListAgentsResponseTypeDef(TypedDict):
    agentSummaries: List[AgentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentSummaryTypeDef](./type_defs.md#agentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrepareAgentResponseTypeDef

```python
# PrepareAgentResponseTypeDef definition

class PrepareAgentResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    preparedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentKnowledgeBaseResponseTypeDef

```python
# UpdateAgentKnowledgeBaseResponseTypeDef definition

class UpdateAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChunkingConfigurationTypeDef

```python
# ChunkingConfigurationTypeDef definition

class ChunkingConfigurationTypeDef(TypedDict):
    chunkingStrategy: ChunkingStrategyType,  # (1)
    fixedSizeChunkingConfiguration: NotRequired[FixedSizeChunkingConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ChunkingStrategyType](./literals.md#chunkingstrategytype) 
2. See [:material-code-braces: FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef) 
## DataSourceConfigurationTypeDef

```python
# DataSourceConfigurationTypeDef definition

class DataSourceConfigurationTypeDef(TypedDict):
    type: DataSourceTypeType,  # (1)
    s3Configuration: NotRequired[S3DataSourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef) 
## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    dataSourceSummaries: List[DataSourceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromptConfigurationTypeDef

```python
# PromptConfigurationTypeDef definition

class PromptConfigurationTypeDef(TypedDict):
    promptType: NotRequired[PromptTypeType],  # (1)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    promptState: NotRequired[PromptStateType],  # (3)
    basePromptTemplate: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationTypeDef],  # (4)
    parserMode: NotRequired[CreationModeType],  # (2)
```

1. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
3. See [:material-code-brackets: PromptStateType](./literals.md#promptstatetype) 
4. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
5. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
## ListIngestionJobsRequestRequestTypeDef

```python
# ListIngestionJobsRequestRequestTypeDef definition

class ListIngestionJobsRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    filters: NotRequired[Sequence[IngestionJobFilterTypeDef]],  # (1)
    sortBy: NotRequired[IngestionJobSortByTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef) 
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef) 
## IngestionJobSummaryTypeDef

```python
# IngestionJobSummaryTypeDef definition

class IngestionJobSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    ingestionJobId: str,
    status: IngestionJobStatusType,  # (1)
    startedAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    statistics: NotRequired[IngestionJobStatisticsTypeDef],  # (2)
```

1. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
2. See [:material-code-braces: IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef) 
## IngestionJobTypeDef

```python
# IngestionJobTypeDef definition

class IngestionJobTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    ingestionJobId: str,
    status: IngestionJobStatusType,  # (1)
    startedAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    statistics: NotRequired[IngestionJobStatisticsTypeDef],  # (2)
    failureReasons: NotRequired[List[str]],
```

1. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
2. See [:material-code-braces: IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef) 
## KnowledgeBaseConfigurationTypeDef

```python
# KnowledgeBaseConfigurationTypeDef definition

class KnowledgeBaseConfigurationTypeDef(TypedDict):
    type: KnowledgeBaseTypeType,  # (1)
    vectorKnowledgeBaseConfiguration: NotRequired[VectorKnowledgeBaseConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
2. See [:material-code-braces: VectorKnowledgeBaseConfigurationTypeDef](./type_defs.md#vectorknowledgebaseconfigurationtypedef) 
## ListKnowledgeBasesResponseTypeDef

```python
# ListKnowledgeBasesResponseTypeDef definition

class ListKnowledgeBasesResponseTypeDef(TypedDict):
    knowledgeBaseSummaries: List[KnowledgeBaseSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef

```python
# ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef definition

class ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentAliasesRequestListAgentAliasesPaginateTypeDef

```python
# ListAgentAliasesRequestListAgentAliasesPaginateTypeDef definition

class ListAgentAliasesRequestListAgentAliasesPaginateTypeDef(TypedDict):
    agentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef

```python
# ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef definition

class ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentVersionsRequestListAgentVersionsPaginateTypeDef

```python
# ListAgentVersionsRequestListAgentVersionsPaginateTypeDef definition

class ListAgentVersionsRequestListAgentVersionsPaginateTypeDef(TypedDict):
    agentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentsRequestListAgentsPaginateTypeDef

```python
# ListAgentsRequestListAgentsPaginateTypeDef definition

class ListAgentsRequestListAgentsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesRequestListDataSourcesPaginateTypeDef

```python
# ListDataSourcesRequestListDataSourcesPaginateTypeDef definition

class ListDataSourcesRequestListDataSourcesPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIngestionJobsRequestListIngestionJobsPaginateTypeDef

```python
# ListIngestionJobsRequestListIngestionJobsPaginateTypeDef definition

class ListIngestionJobsRequestListIngestionJobsPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    filters: NotRequired[Sequence[IngestionJobFilterTypeDef]],  # (1)
    sortBy: NotRequired[IngestionJobSortByTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef) 
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef

```python
# ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef definition

class ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## OpenSearchServerlessConfigurationTypeDef

```python
# OpenSearchServerlessConfigurationTypeDef definition

class OpenSearchServerlessConfigurationTypeDef(TypedDict):
    collectionArn: str,
    vectorIndexName: str,
    fieldMapping: OpenSearchServerlessFieldMappingTypeDef,  # (1)
```

1. See [:material-code-braces: OpenSearchServerlessFieldMappingTypeDef](./type_defs.md#opensearchserverlessfieldmappingtypedef) 
## PineconeConfigurationTypeDef

```python
# PineconeConfigurationTypeDef definition

class PineconeConfigurationTypeDef(TypedDict):
    connectionString: str,
    credentialsSecretArn: str,
    fieldMapping: PineconeFieldMappingTypeDef,  # (1)
    namespace: NotRequired[str],
```

1. See [:material-code-braces: PineconeFieldMappingTypeDef](./type_defs.md#pineconefieldmappingtypedef) 
## RdsConfigurationTypeDef

```python
# RdsConfigurationTypeDef definition

class RdsConfigurationTypeDef(TypedDict):
    resourceArn: str,
    credentialsSecretArn: str,
    databaseName: str,
    tableName: str,
    fieldMapping: RdsFieldMappingTypeDef,  # (1)
```

1. See [:material-code-braces: RdsFieldMappingTypeDef](./type_defs.md#rdsfieldmappingtypedef) 
## RedisEnterpriseCloudConfigurationTypeDef

```python
# RedisEnterpriseCloudConfigurationTypeDef definition

class RedisEnterpriseCloudConfigurationTypeDef(TypedDict):
    endpoint: str,
    vectorIndexName: str,
    credentialsSecretArn: str,
    fieldMapping: RedisEnterpriseCloudFieldMappingTypeDef,  # (1)
```

1. See [:material-code-braces: RedisEnterpriseCloudFieldMappingTypeDef](./type_defs.md#redisenterprisecloudfieldmappingtypedef) 
## AgentActionGroupTypeDef

```python
# AgentActionGroupTypeDef definition

class AgentActionGroupTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
    actionGroupName: str,
    createdAt: datetime,
    updatedAt: datetime,
    actionGroupState: ActionGroupStateType,  # (4)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    parentActionSignature: NotRequired[ActionGroupSignatureType],  # (1)
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (2)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
```

1. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
2. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
## CreateAgentActionGroupRequestRequestTypeDef

```python
# CreateAgentActionGroupRequestRequestTypeDef definition

class CreateAgentActionGroupRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    actionGroupName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (1)
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (2)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    actionGroupState: NotRequired[ActionGroupStateType],  # (4)
```

1. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
2. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
## UpdateAgentActionGroupRequestRequestTypeDef

```python
# UpdateAgentActionGroupRequestRequestTypeDef definition

class UpdateAgentActionGroupRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    actionGroupId: str,
    actionGroupName: str,
    description: NotRequired[str],
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (1)
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (2)
    actionGroupState: NotRequired[ActionGroupStateType],  # (3)
    apiSchema: NotRequired[APISchemaTypeDef],  # (4)
```

1. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
2. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
3. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
4. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
## AgentAliasTypeDef

```python
# AgentAliasTypeDef definition

class AgentAliasTypeDef(TypedDict):
    agentId: str,
    agentAliasId: str,
    agentAliasName: str,
    agentAliasArn: str,
    routingConfiguration: List[AgentAliasRoutingConfigurationListItemTypeDef],  # (1)
    createdAt: datetime,
    updatedAt: datetime,
    agentAliasStatus: AgentAliasStatusType,  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    agentAliasHistoryEvents: NotRequired[List[AgentAliasHistoryEventTypeDef]],  # (2)
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: AgentAliasHistoryEventTypeDef](./type_defs.md#agentaliashistoryeventtypedef) 
3. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype) 
## ListAgentAliasesResponseTypeDef

```python
# ListAgentAliasesResponseTypeDef definition

class ListAgentAliasesResponseTypeDef(TypedDict):
    agentAliasSummaries: List[AgentAliasSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasSummaryTypeDef](./type_defs.md#agentaliassummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VectorIngestionConfigurationTypeDef

```python
# VectorIngestionConfigurationTypeDef definition

class VectorIngestionConfigurationTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef) 
## PromptOverrideConfigurationTypeDef

```python
# PromptOverrideConfigurationTypeDef definition

class PromptOverrideConfigurationTypeDef(TypedDict):
    promptConfigurations: Sequence[PromptConfigurationTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See [:material-code-braces: PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef) 
## ListIngestionJobsResponseTypeDef

```python
# ListIngestionJobsResponseTypeDef definition

class ListIngestionJobsResponseTypeDef(TypedDict):
    ingestionJobSummaries: List[IngestionJobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobSummaryTypeDef](./type_defs.md#ingestionjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIngestionJobResponseTypeDef

```python
# GetIngestionJobResponseTypeDef definition

class GetIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartIngestionJobResponseTypeDef

```python
# StartIngestionJobResponseTypeDef definition

class StartIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    type: KnowledgeBaseStorageTypeType,  # (1)
    opensearchServerlessConfiguration: NotRequired[OpenSearchServerlessConfigurationTypeDef],  # (2)
    pineconeConfiguration: NotRequired[PineconeConfigurationTypeDef],  # (3)
    redisEnterpriseCloudConfiguration: NotRequired[RedisEnterpriseCloudConfigurationTypeDef],  # (4)
    rdsConfiguration: NotRequired[RdsConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: KnowledgeBaseStorageTypeType](./literals.md#knowledgebasestoragetypetype) 
2. See [:material-code-braces: OpenSearchServerlessConfigurationTypeDef](./type_defs.md#opensearchserverlessconfigurationtypedef) 
3. See [:material-code-braces: PineconeConfigurationTypeDef](./type_defs.md#pineconeconfigurationtypedef) 
4. See [:material-code-braces: RedisEnterpriseCloudConfigurationTypeDef](./type_defs.md#redisenterprisecloudconfigurationtypedef) 
5. See [:material-code-braces: RdsConfigurationTypeDef](./type_defs.md#rdsconfigurationtypedef) 
## CreateAgentActionGroupResponseTypeDef

```python
# CreateAgentActionGroupResponseTypeDef definition

class CreateAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentActionGroupResponseTypeDef

```python
# GetAgentActionGroupResponseTypeDef definition

class GetAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentActionGroupResponseTypeDef

```python
# UpdateAgentActionGroupResponseTypeDef definition

class UpdateAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAgentAliasResponseTypeDef

```python
# CreateAgentAliasResponseTypeDef definition

class CreateAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentAliasResponseTypeDef

```python
# GetAgentAliasResponseTypeDef definition

class GetAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentAliasResponseTypeDef

```python
# UpdateAgentAliasResponseTypeDef definition

class UpdateAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceRequestRequestTypeDef

```python
# CreateDataSourceRequestRequestTypeDef definition

class CreateDataSourceRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (2)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    name: str,
    status: DataSourceStatusType,  # (1)
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (2)
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
## UpdateDataSourceRequestRequestTypeDef

```python
# UpdateDataSourceRequestRequestTypeDef definition

class UpdateDataSourceRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    dataSourceId: str,
    name: str,
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (2)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
## AgentTypeDef

```python
# AgentTypeDef definition

class AgentTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentArn: str,
    agentVersion: str,
    agentStatus: AgentStatusType,  # (1)
    idleSessionTTLInSeconds: int,
    agentResourceRoleArn: str,
    createdAt: datetime,
    updatedAt: datetime,
    clientToken: NotRequired[str],
    instruction: NotRequired[str],
    foundationModel: NotRequired[str],
    description: NotRequired[str],
    customerEncryptionKeyArn: NotRequired[str],
    preparedAt: NotRequired[datetime],
    failureReasons: NotRequired[List[str]],
    recommendedActions: NotRequired[List[str]],
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## AgentVersionTypeDef

```python
# AgentVersionTypeDef definition

class AgentVersionTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentArn: str,
    version: str,
    agentStatus: AgentStatusType,  # (1)
    idleSessionTTLInSeconds: int,
    agentResourceRoleArn: str,
    createdAt: datetime,
    updatedAt: datetime,
    instruction: NotRequired[str],
    foundationModel: NotRequired[str],
    description: NotRequired[str],
    customerEncryptionKeyArn: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    recommendedActions: NotRequired[List[str]],
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## CreateAgentRequestRequestTypeDef

```python
# CreateAgentRequestRequestTypeDef definition

class CreateAgentRequestRequestTypeDef(TypedDict):
    agentName: str,
    agentResourceRoleArn: str,
    clientToken: NotRequired[str],
    instruction: NotRequired[str],
    foundationModel: NotRequired[str],
    description: NotRequired[str],
    idleSessionTTLInSeconds: NotRequired[int],
    customerEncryptionKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## UpdateAgentRequestRequestTypeDef

```python
# UpdateAgentRequestRequestTypeDef definition

class UpdateAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    instruction: NotRequired[str],
    foundationModel: NotRequired[str],
    description: NotRequired[str],
    idleSessionTTLInSeconds: NotRequired[int],
    customerEncryptionKeyArn: NotRequired[str],
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## CreateKnowledgeBaseRequestRequestTypeDef

```python
# CreateKnowledgeBaseRequestRequestTypeDef definition

class CreateKnowledgeBaseRequestRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## KnowledgeBaseTypeDef

```python
# KnowledgeBaseTypeDef definition

class KnowledgeBaseTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    knowledgeBaseArn: str,
    roleArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    status: KnowledgeBaseStatusType,  # (3)
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
3. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
## UpdateKnowledgeBaseRequestRequestTypeDef

```python
# UpdateKnowledgeBaseRequestRequestTypeDef definition

class UpdateKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataSourceResponseTypeDef

```python
# GetDataSourceResponseTypeDef definition

class GetDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourceResponseTypeDef

```python
# UpdateDataSourceResponseTypeDef definition

class UpdateDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAgentResponseTypeDef

```python
# CreateAgentResponseTypeDef definition

class CreateAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentResponseTypeDef

```python
# GetAgentResponseTypeDef definition

class GetAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentResponseTypeDef

```python
# UpdateAgentResponseTypeDef definition

class UpdateAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentVersionResponseTypeDef

```python
# GetAgentVersionResponseTypeDef definition

class GetAgentVersionResponseTypeDef(TypedDict):
    agentVersion: AgentVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentVersionTypeDef](./type_defs.md#agentversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKnowledgeBaseResponseTypeDef

```python
# CreateKnowledgeBaseResponseTypeDef definition

class CreateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKnowledgeBaseResponseTypeDef

```python
# GetKnowledgeBaseResponseTypeDef definition

class GetKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKnowledgeBaseResponseTypeDef

```python
# UpdateKnowledgeBaseResponseTypeDef definition

class UpdateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
