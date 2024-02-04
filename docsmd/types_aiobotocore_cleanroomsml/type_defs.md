# Type definitions

> [Index](../README.md) > [CleanRoomsML](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## S3ConfigMapTypeDef

```python
# S3ConfigMapTypeDef definition

class S3ConfigMapTypeDef(TypedDict):
    s3Uri: str,
```

## AudienceSizeTypeDef

```python
# AudienceSizeTypeDef definition

class AudienceSizeTypeDef(TypedDict):
    type: AudienceSizeTypeType,  # (1)
    value: int,
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## StatusDetailsTypeDef

```python
# StatusDetailsTypeDef definition

class StatusDetailsTypeDef(TypedDict):
    message: NotRequired[str],
    statusCode: NotRequired[str],
```

## AudienceGenerationJobSummaryTypeDef

```python
# AudienceGenerationJobSummaryTypeDef definition

class AudienceGenerationJobSummaryTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    configuredAudienceModelArn: str,
    createTime: datetime,
    name: str,
    status: AudienceGenerationJobStatusType,  # (1)
    updateTime: datetime,
    collaborationId: NotRequired[str],
    description: NotRequired[str],
    startedBy: NotRequired[str],
```

1. See [:material-code-brackets: AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype) 
## AudienceModelMetricTypeDef

```python
# AudienceModelMetricTypeDef definition

class AudienceModelMetricTypeDef(TypedDict):
    forTopKItemPredictions: int,
    type: AudienceModelMetricTypeType,  # (1)
    value: float,
```

1. See [:material-code-brackets: AudienceModelMetricTypeType](./literals.md#audiencemodelmetrictypetype) 
## AudienceModelSummaryTypeDef

```python
# AudienceModelSummaryTypeDef definition

class AudienceModelSummaryTypeDef(TypedDict):
    audienceModelArn: str,
    createTime: datetime,
    name: str,
    status: AudienceModelStatusType,  # (1)
    trainingDatasetArn: str,
    updateTime: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: AudienceModelStatusType](./literals.md#audiencemodelstatustype) 
## AudienceSizeConfigTypeDef

```python
# AudienceSizeConfigTypeDef definition

class AudienceSizeConfigTypeDef(TypedDict):
    audienceSizeBins: Sequence[int],
    audienceSizeType: AudienceSizeTypeType,  # (1)
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## ColumnSchemaTypeDef

```python
# ColumnSchemaTypeDef definition

class ColumnSchemaTypeDef(TypedDict):
    columnName: str,
    columnTypes: Sequence[ColumnTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnTypeType](./literals.md#columntypetype) 
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

## GlueDataSourceTypeDef

```python
# GlueDataSourceTypeDef definition

class GlueDataSourceTypeDef(TypedDict):
    databaseName: str,
    tableName: str,
    catalogId: NotRequired[str],
```

## DeleteAudienceGenerationJobRequestRequestTypeDef

```python
# DeleteAudienceGenerationJobRequestRequestTypeDef definition

class DeleteAudienceGenerationJobRequestRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
```

## DeleteAudienceModelRequestRequestTypeDef

```python
# DeleteAudienceModelRequestRequestTypeDef definition

class DeleteAudienceModelRequestRequestTypeDef(TypedDict):
    audienceModelArn: str,
```

## DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef

```python
# DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef definition

class DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## DeleteConfiguredAudienceModelRequestRequestTypeDef

```python
# DeleteConfiguredAudienceModelRequestRequestTypeDef definition

class DeleteConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## DeleteTrainingDatasetRequestRequestTypeDef

```python
# DeleteTrainingDatasetRequestRequestTypeDef definition

class DeleteTrainingDatasetRequestRequestTypeDef(TypedDict):
    trainingDatasetArn: str,
```

## GetAudienceGenerationJobRequestRequestTypeDef

```python
# GetAudienceGenerationJobRequestRequestTypeDef definition

class GetAudienceGenerationJobRequestRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
```

## GetAudienceModelRequestRequestTypeDef

```python
# GetAudienceModelRequestRequestTypeDef definition

class GetAudienceModelRequestRequestTypeDef(TypedDict):
    audienceModelArn: str,
```

## GetConfiguredAudienceModelPolicyRequestRequestTypeDef

```python
# GetConfiguredAudienceModelPolicyRequestRequestTypeDef definition

class GetConfiguredAudienceModelPolicyRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## GetConfiguredAudienceModelRequestRequestTypeDef

```python
# GetConfiguredAudienceModelRequestRequestTypeDef definition

class GetConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## GetTrainingDatasetRequestRequestTypeDef

```python
# GetTrainingDatasetRequestRequestTypeDef definition

class GetTrainingDatasetRequestRequestTypeDef(TypedDict):
    trainingDatasetArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAudienceExportJobsRequestRequestTypeDef

```python
# ListAudienceExportJobsRequestRequestTypeDef definition

class ListAudienceExportJobsRequestRequestTypeDef(TypedDict):
    audienceGenerationJobArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAudienceGenerationJobsRequestRequestTypeDef

```python
# ListAudienceGenerationJobsRequestRequestTypeDef definition

class ListAudienceGenerationJobsRequestRequestTypeDef(TypedDict):
    collaborationId: NotRequired[str],
    configuredAudienceModelArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAudienceModelsRequestRequestTypeDef

```python
# ListAudienceModelsRequestRequestTypeDef definition

class ListAudienceModelsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListConfiguredAudienceModelsRequestRequestTypeDef

```python
# ListConfiguredAudienceModelsRequestRequestTypeDef definition

class ListConfiguredAudienceModelsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTrainingDatasetsRequestRequestTypeDef

```python
# ListTrainingDatasetsRequestRequestTypeDef definition

class ListTrainingDatasetsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TrainingDatasetSummaryTypeDef

```python
# TrainingDatasetSummaryTypeDef definition

class TrainingDatasetSummaryTypeDef(TypedDict):
    createTime: datetime,
    name: str,
    status: TrainingDatasetStatusType,  # (1)
    trainingDatasetArn: str,
    updateTime: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype) 
## PutConfiguredAudienceModelPolicyRequestRequestTypeDef

```python
# PutConfiguredAudienceModelPolicyRequestRequestTypeDef definition

class PutConfiguredAudienceModelPolicyRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    policyExistenceCondition: NotRequired[PolicyExistenceConditionType],  # (1)
    previousPolicyHash: NotRequired[str],
```

1. See [:material-code-brackets: PolicyExistenceConditionType](./literals.md#policyexistenceconditiontype) 
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

## AudienceDestinationTypeDef

```python
# AudienceDestinationTypeDef definition

class AudienceDestinationTypeDef(TypedDict):
    s3Destination: S3ConfigMapTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
## AudienceGenerationJobDataSourceTypeDef

```python
# AudienceGenerationJobDataSourceTypeDef definition

class AudienceGenerationJobDataSourceTypeDef(TypedDict):
    dataSource: S3ConfigMapTypeDef,  # (1)
    roleArn: str,
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
## RelevanceMetricTypeDef

```python
# RelevanceMetricTypeDef definition

class RelevanceMetricTypeDef(TypedDict):
    audienceSize: AudienceSizeTypeDef,  # (1)
    score: NotRequired[float],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
## StartAudienceExportJobRequestRequestTypeDef

```python
# StartAudienceExportJobRequestRequestTypeDef definition

class StartAudienceExportJobRequestRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
## AudienceExportJobSummaryTypeDef

```python
# AudienceExportJobSummaryTypeDef definition

class AudienceExportJobSummaryTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    createTime: datetime,
    name: str,
    status: AudienceExportJobStatusType,  # (2)
    updateTime: datetime,
    description: NotRequired[str],
    outputLocation: NotRequired[str],
    statusDetails: NotRequired[StatusDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
2. See [:material-code-brackets: AudienceExportJobStatusType](./literals.md#audienceexportjobstatustype) 
3. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
## CreateAudienceModelRequestRequestTypeDef

```python
# CreateAudienceModelRequestRequestTypeDef definition

class CreateAudienceModelRequestRequestTypeDef(TypedDict):
    name: str,
    trainingDatasetArn: str,
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    trainingDataEndTime: NotRequired[Union[datetime, str]],
    trainingDataStartTime: NotRequired[Union[datetime, str]],
```

## CreateAudienceModelResponseTypeDef

```python
# CreateAudienceModelResponseTypeDef definition

class CreateAudienceModelResponseTypeDef(TypedDict):
    audienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredAudienceModelResponseTypeDef

```python
# CreateConfiguredAudienceModelResponseTypeDef definition

class CreateConfiguredAudienceModelResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainingDatasetResponseTypeDef

```python
# CreateTrainingDatasetResponseTypeDef definition

class CreateTrainingDatasetResponseTypeDef(TypedDict):
    trainingDatasetArn: str,
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
## GetAudienceModelResponseTypeDef

```python
# GetAudienceModelResponseTypeDef definition

class GetAudienceModelResponseTypeDef(TypedDict):
    audienceModelArn: str,
    createTime: datetime,
    description: str,
    kmsKeyArn: str,
    metrics: List[AudienceModelMetricTypeDef],  # (1)
    name: str,
    status: AudienceModelStatusType,  # (2)
    statusDetails: StatusDetailsTypeDef,  # (3)
    tags: Dict[str, str],
    trainingDataEndTime: datetime,
    trainingDataStartTime: datetime,
    trainingDatasetArn: str,
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AudienceModelMetricTypeDef](./type_defs.md#audiencemodelmetrictypedef) 
2. See [:material-code-brackets: AudienceModelStatusType](./literals.md#audiencemodelstatustype) 
3. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredAudienceModelPolicyResponseTypeDef

```python
# GetConfiguredAudienceModelPolicyResponseTypeDef definition

class GetConfiguredAudienceModelPolicyResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    policyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAudienceGenerationJobsResponseTypeDef

```python
# ListAudienceGenerationJobsResponseTypeDef definition

class ListAudienceGenerationJobsResponseTypeDef(TypedDict):
    audienceGenerationJobs: List[AudienceGenerationJobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AudienceGenerationJobSummaryTypeDef](./type_defs.md#audiencegenerationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAudienceModelsResponseTypeDef

```python
# ListAudienceModelsResponseTypeDef definition

class ListAudienceModelsResponseTypeDef(TypedDict):
    audienceModels: List[AudienceModelSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AudienceModelSummaryTypeDef](./type_defs.md#audiencemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfiguredAudienceModelPolicyResponseTypeDef

```python
# PutConfiguredAudienceModelPolicyResponseTypeDef definition

class PutConfiguredAudienceModelPolicyResponseTypeDef(TypedDict):
    configuredAudienceModelPolicy: str,
    policyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAudienceGenerationJobResponseTypeDef

```python
# StartAudienceGenerationJobResponseTypeDef definition

class StartAudienceGenerationJobResponseTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelResponseTypeDef

```python
# UpdateConfiguredAudienceModelResponseTypeDef definition

class UpdateConfiguredAudienceModelResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    glueDataSource: GlueDataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: GlueDataSourceTypeDef](./type_defs.md#gluedatasourcetypedef) 
## ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef

```python
# ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef definition

class ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef(TypedDict):
    audienceGenerationJobArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef

```python
# ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef definition

class ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef(TypedDict):
    collaborationId: NotRequired[str],
    configuredAudienceModelArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAudienceModelsRequestListAudienceModelsPaginateTypeDef

```python
# ListAudienceModelsRequestListAudienceModelsPaginateTypeDef definition

class ListAudienceModelsRequestListAudienceModelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef

```python
# ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef definition

class ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef

```python
# ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef definition

class ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingDatasetsResponseTypeDef

```python
# ListTrainingDatasetsResponseTypeDef definition

class ListTrainingDatasetsResponseTypeDef(TypedDict):
    nextToken: str,
    trainingDatasets: List[TrainingDatasetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrainingDatasetSummaryTypeDef](./type_defs.md#trainingdatasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfiguredAudienceModelOutputConfigTypeDef

```python
# ConfiguredAudienceModelOutputConfigTypeDef definition

class ConfiguredAudienceModelOutputConfigTypeDef(TypedDict):
    destination: AudienceDestinationTypeDef,  # (1)
    roleArn: str,
```

1. See [:material-code-braces: AudienceDestinationTypeDef](./type_defs.md#audiencedestinationtypedef) 
## StartAudienceGenerationJobRequestRequestTypeDef

```python
# StartAudienceGenerationJobRequestRequestTypeDef definition

class StartAudienceGenerationJobRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    name: str,
    seedAudience: AudienceGenerationJobDataSourceTypeDef,  # (1)
    collaborationId: NotRequired[str],
    description: NotRequired[str],
    includeSeedInOutput: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef) 
## AudienceQualityMetricsTypeDef

```python
# AudienceQualityMetricsTypeDef definition

class AudienceQualityMetricsTypeDef(TypedDict):
    relevanceMetrics: List[RelevanceMetricTypeDef],  # (1)
```

1. See [:material-code-braces: RelevanceMetricTypeDef](./type_defs.md#relevancemetrictypedef) 
## ListAudienceExportJobsResponseTypeDef

```python
# ListAudienceExportJobsResponseTypeDef definition

class ListAudienceExportJobsResponseTypeDef(TypedDict):
    audienceExportJobs: List[AudienceExportJobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AudienceExportJobSummaryTypeDef](./type_defs.md#audienceexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetInputConfigTypeDef

```python
# DatasetInputConfigTypeDef definition

class DatasetInputConfigTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    schema: Sequence[ColumnSchemaTypeDef],  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ColumnSchemaTypeDef](./type_defs.md#columnschematypedef) 
## ConfiguredAudienceModelSummaryTypeDef

```python
# ConfiguredAudienceModelSummaryTypeDef definition

class ConfiguredAudienceModelSummaryTypeDef(TypedDict):
    audienceModelArn: str,
    configuredAudienceModelArn: str,
    createTime: datetime,
    name: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    status: ConfiguredAudienceModelStatusType,  # (2)
    updateTime: datetime,
    description: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype) 
## CreateConfiguredAudienceModelRequestRequestTypeDef

```python
# CreateConfiguredAudienceModelRequestRequestTypeDef definition

class CreateConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    audienceModelArn: str,
    name: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],  # (2)
    audienceSizeConfig: NotRequired[AudienceSizeConfigTypeDef],  # (3)
    childResourceTagOnCreatePolicy: NotRequired[TagOnCreatePolicyType],  # (4)
    description: NotRequired[str],
    minMatchingSeedSize: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
4. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
## GetConfiguredAudienceModelResponseTypeDef

```python
# GetConfiguredAudienceModelResponseTypeDef definition

class GetConfiguredAudienceModelResponseTypeDef(TypedDict):
    audienceModelArn: str,
    audienceSizeConfig: AudienceSizeConfigTypeDef,  # (1)
    childResourceTagOnCreatePolicy: TagOnCreatePolicyType,  # (2)
    configuredAudienceModelArn: str,
    createTime: datetime,
    description: str,
    minMatchingSeedSize: int,
    name: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (3)
    sharedAudienceMetrics: List[SharedAudienceMetricsType],  # (4)
    status: ConfiguredAudienceModelStatusType,  # (5)
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
2. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
3. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
4. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
5. See [:material-code-brackets: ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelRequestRequestTypeDef

```python
# UpdateConfiguredAudienceModelRequestRequestTypeDef definition

class UpdateConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    audienceModelArn: NotRequired[str],
    audienceSizeConfig: NotRequired[AudienceSizeConfigTypeDef],  # (1)
    description: NotRequired[str],
    minMatchingSeedSize: NotRequired[int],
    outputConfig: NotRequired[ConfiguredAudienceModelOutputConfigTypeDef],  # (2)
    sharedAudienceMetrics: NotRequired[Sequence[SharedAudienceMetricsType]],  # (3)
```

1. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
2. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
3. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
## GetAudienceGenerationJobResponseTypeDef

```python
# GetAudienceGenerationJobResponseTypeDef definition

class GetAudienceGenerationJobResponseTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    collaborationId: str,
    configuredAudienceModelArn: str,
    createTime: datetime,
    description: str,
    includeSeedInOutput: bool,
    metrics: AudienceQualityMetricsTypeDef,  # (1)
    name: str,
    seedAudience: AudienceGenerationJobDataSourceTypeDef,  # (2)
    startedBy: str,
    status: AudienceGenerationJobStatusType,  # (3)
    statusDetails: StatusDetailsTypeDef,  # (4)
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AudienceQualityMetricsTypeDef](./type_defs.md#audiencequalitymetricstypedef) 
2. See [:material-code-braces: AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef) 
3. See [:material-code-brackets: AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype) 
4. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetTypeDef

```python
# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    inputConfig: DatasetInputConfigTypeDef,  # (1)
    type: DatasetTypeType,  # (2)
```

1. See [:material-code-braces: DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef) 
2. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
## ListConfiguredAudienceModelsResponseTypeDef

```python
# ListConfiguredAudienceModelsResponseTypeDef definition

class ListConfiguredAudienceModelsResponseTypeDef(TypedDict):
    configuredAudienceModels: List[ConfiguredAudienceModelSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelSummaryTypeDef](./type_defs.md#configuredaudiencemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainingDatasetRequestRequestTypeDef

```python
# CreateTrainingDatasetRequestRequestTypeDef definition

class CreateTrainingDatasetRequestRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    trainingData: Sequence[DatasetTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
## GetTrainingDatasetResponseTypeDef

```python
# GetTrainingDatasetResponseTypeDef definition

class GetTrainingDatasetResponseTypeDef(TypedDict):
    createTime: datetime,
    description: str,
    name: str,
    roleArn: str,
    status: TrainingDatasetStatusType,  # (1)
    tags: Dict[str, str],
    trainingData: List[DatasetTypeDef],  # (2)
    trainingDatasetArn: str,
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype) 
2. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
