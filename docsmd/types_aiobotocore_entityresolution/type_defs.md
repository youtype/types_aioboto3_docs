# Type definitions

> [Index](../README.md) > [EntityResolution](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).



## IdMappingWorkflowInputSourceTypeDef

```python
# IdMappingWorkflowInputSourceTypeDef definition

class IdMappingWorkflowInputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: str,
```

## IdMappingWorkflowOutputSourceTypeDef

```python
# IdMappingWorkflowOutputSourceTypeDef definition

class IdMappingWorkflowOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    KMSArn: NotRequired[str],
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

## IncrementalRunConfigTypeDef

```python
# IncrementalRunConfigTypeDef definition

class IncrementalRunConfigTypeDef(TypedDict):
    incrementalRunType: NotRequired[IncrementalRunTypeType],  # (1)
```

1. See [:material-code-brackets: IncrementalRunTypeType](./literals.md#incrementalruntypetype) 
## InputSourceTypeDef

```python
# InputSourceTypeDef definition

class InputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: str,
    applyNormalization: NotRequired[bool],
```

## SchemaInputAttributeTypeDef

```python
# SchemaInputAttributeTypeDef definition

class SchemaInputAttributeTypeDef(TypedDict):
    fieldName: str,
    type: SchemaAttributeTypeType,  # (1)
    groupName: NotRequired[str],
    matchKey: NotRequired[str],
    subType: NotRequired[str],
```

1. See [:material-code-brackets: SchemaAttributeTypeType](./literals.md#schemaattributetypetype) 
## DeleteIdMappingWorkflowInputRequestTypeDef

```python
# DeleteIdMappingWorkflowInputRequestTypeDef definition

class DeleteIdMappingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## DeleteMatchingWorkflowInputRequestTypeDef

```python
# DeleteMatchingWorkflowInputRequestTypeDef definition

class DeleteMatchingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## DeleteSchemaMappingInputRequestTypeDef

```python
# DeleteSchemaMappingInputRequestTypeDef definition

class DeleteSchemaMappingInputRequestTypeDef(TypedDict):
    schemaName: str,
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    errorMessage: NotRequired[str],
```

## GetIdMappingJobInputRequestTypeDef

```python
# GetIdMappingJobInputRequestTypeDef definition

class GetIdMappingJobInputRequestTypeDef(TypedDict):
    jobId: str,
    workflowName: str,
```

## IdMappingJobMetricsTypeDef

```python
# IdMappingJobMetricsTypeDef definition

class IdMappingJobMetricsTypeDef(TypedDict):
    inputRecords: NotRequired[int],
    recordsNotProcessed: NotRequired[int],
    totalRecordsProcessed: NotRequired[int],
```

## GetIdMappingWorkflowInputRequestTypeDef

```python
# GetIdMappingWorkflowInputRequestTypeDef definition

class GetIdMappingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## GetMatchIdInputRequestTypeDef

```python
# GetMatchIdInputRequestTypeDef definition

class GetMatchIdInputRequestTypeDef(TypedDict):
    record: Mapping[str, str],
    workflowName: str,
```

## GetMatchingJobInputRequestTypeDef

```python
# GetMatchingJobInputRequestTypeDef definition

class GetMatchingJobInputRequestTypeDef(TypedDict):
    jobId: str,
    workflowName: str,
```

## JobMetricsTypeDef

```python
# JobMetricsTypeDef definition

class JobMetricsTypeDef(TypedDict):
    inputRecords: NotRequired[int],
    matchIDs: NotRequired[int],
    recordsNotProcessed: NotRequired[int],
    totalRecordsProcessed: NotRequired[int],
```

## GetMatchingWorkflowInputRequestTypeDef

```python
# GetMatchingWorkflowInputRequestTypeDef definition

class GetMatchingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## GetProviderServiceInputRequestTypeDef

```python
# GetProviderServiceInputRequestTypeDef definition

class GetProviderServiceInputRequestTypeDef(TypedDict):
    providerName: str,
    providerServiceName: str,
```

## ProviderIntermediateDataAccessConfigurationTypeDef

```python
# ProviderIntermediateDataAccessConfigurationTypeDef definition

class ProviderIntermediateDataAccessConfigurationTypeDef(TypedDict):
    awsAccountIds: NotRequired[List[str]],
    requiredBucketActions: NotRequired[List[str]],
```

## GetSchemaMappingInputRequestTypeDef

```python
# GetSchemaMappingInputRequestTypeDef definition

class GetSchemaMappingInputRequestTypeDef(TypedDict):
    schemaName: str,
```

## IdMappingWorkflowSummaryTypeDef

```python
# IdMappingWorkflowSummaryTypeDef definition

class IdMappingWorkflowSummaryTypeDef(TypedDict):
    createdAt: datetime,
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

## IntermediateSourceConfigurationTypeDef

```python
# IntermediateSourceConfigurationTypeDef definition

class IntermediateSourceConfigurationTypeDef(TypedDict):
    intermediateS3Path: str,
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    jobId: str,
    startTime: datetime,
    status: JobStatusType,  # (1)
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIdMappingJobsInputRequestTypeDef

```python
# ListIdMappingJobsInputRequestTypeDef definition

class ListIdMappingJobsInputRequestTypeDef(TypedDict):
    workflowName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdMappingWorkflowsInputRequestTypeDef

```python
# ListIdMappingWorkflowsInputRequestTypeDef definition

class ListIdMappingWorkflowsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMatchingJobsInputRequestTypeDef

```python
# ListMatchingJobsInputRequestTypeDef definition

class ListMatchingJobsInputRequestTypeDef(TypedDict):
    workflowName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMatchingWorkflowsInputRequestTypeDef

```python
# ListMatchingWorkflowsInputRequestTypeDef definition

class ListMatchingWorkflowsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MatchingWorkflowSummaryTypeDef

```python
# MatchingWorkflowSummaryTypeDef definition

class MatchingWorkflowSummaryTypeDef(TypedDict):
    createdAt: datetime,
    resolutionType: ResolutionTypeType,  # (1)
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

1. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
## ListProviderServicesInputRequestTypeDef

```python
# ListProviderServicesInputRequestTypeDef definition

class ListProviderServicesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    providerName: NotRequired[str],
```

## ProviderServiceSummaryTypeDef

```python
# ProviderServiceSummaryTypeDef definition

class ProviderServiceSummaryTypeDef(TypedDict):
    providerName: str,
    providerServiceArn: str,
    providerServiceDisplayName: str,
    providerServiceName: str,
    providerServiceType: ServiceTypeType,  # (1)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ListSchemaMappingsInputRequestTypeDef

```python
# ListSchemaMappingsInputRequestTypeDef definition

class ListSchemaMappingsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SchemaMappingSummaryTypeDef

```python
# SchemaMappingSummaryTypeDef definition

class SchemaMappingSummaryTypeDef(TypedDict):
    createdAt: datetime,
    hasWorkflows: bool,
    schemaArn: str,
    schemaName: str,
    updatedAt: datetime,
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## OutputAttributeTypeDef

```python
# OutputAttributeTypeDef definition

class OutputAttributeTypeDef(TypedDict):
    name: str,
    hashed: NotRequired[bool],
```

## ProviderMarketplaceConfigurationTypeDef

```python
# ProviderMarketplaceConfigurationTypeDef definition

class ProviderMarketplaceConfigurationTypeDef(TypedDict):
    assetId: str,
    dataSetId: str,
    listingId: str,
    revisionId: str,
```

## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    matchingKeys: Sequence[str],
    ruleName: str,
```

## StartIdMappingJobInputRequestTypeDef

```python
# StartIdMappingJobInputRequestTypeDef definition

class StartIdMappingJobInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## StartMatchingJobInputRequestTypeDef

```python
# StartMatchingJobInputRequestTypeDef definition

class StartMatchingJobInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## DeleteIdMappingWorkflowOutputTypeDef

```python
# DeleteIdMappingWorkflowOutputTypeDef definition

class DeleteIdMappingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMatchingWorkflowOutputTypeDef

```python
# DeleteMatchingWorkflowOutputTypeDef definition

class DeleteMatchingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSchemaMappingOutputTypeDef

```python
# DeleteSchemaMappingOutputTypeDef definition

class DeleteSchemaMappingOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchIdOutputTypeDef

```python
# GetMatchIdOutputTypeDef definition

class GetMatchIdOutputTypeDef(TypedDict):
    matchId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartIdMappingJobOutputTypeDef

```python
# StartIdMappingJobOutputTypeDef definition

class StartIdMappingJobOutputTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMatchingJobOutputTypeDef

```python
# StartMatchingJobOutputTypeDef definition

class StartMatchingJobOutputTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchemaMappingInputRequestTypeDef

```python
# CreateSchemaMappingInputRequestTypeDef definition

class CreateSchemaMappingInputRequestTypeDef(TypedDict):
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
## CreateSchemaMappingOutputTypeDef

```python
# CreateSchemaMappingOutputTypeDef definition

class CreateSchemaMappingOutputTypeDef(TypedDict):
    description: str,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaMappingOutputTypeDef

```python
# GetSchemaMappingOutputTypeDef definition

class GetSchemaMappingOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    hasWorkflows: bool,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSchemaMappingInputRequestTypeDef

```python
# UpdateSchemaMappingInputRequestTypeDef definition

class UpdateSchemaMappingInputRequestTypeDef(TypedDict):
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
## UpdateSchemaMappingOutputTypeDef

```python
# UpdateSchemaMappingOutputTypeDef definition

class UpdateSchemaMappingOutputTypeDef(TypedDict):
    description: str,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdMappingJobOutputTypeDef

```python
# GetIdMappingJobOutputTypeDef definition

class GetIdMappingJobOutputTypeDef(TypedDict):
    endTime: datetime,
    errorDetails: ErrorDetailsTypeDef,  # (1)
    jobId: str,
    metrics: IdMappingJobMetricsTypeDef,  # (2)
    startTime: datetime,
    status: JobStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
2. See [:material-code-braces: IdMappingJobMetricsTypeDef](./type_defs.md#idmappingjobmetricstypedef) 
3. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchingJobOutputTypeDef

```python
# GetMatchingJobOutputTypeDef definition

class GetMatchingJobOutputTypeDef(TypedDict):
    endTime: datetime,
    errorDetails: ErrorDetailsTypeDef,  # (1)
    jobId: str,
    metrics: JobMetricsTypeDef,  # (2)
    startTime: datetime,
    status: JobStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
2. See [:material-code-braces: JobMetricsTypeDef](./type_defs.md#jobmetricstypedef) 
3. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdMappingWorkflowsOutputTypeDef

```python
# ListIdMappingWorkflowsOutputTypeDef definition

class ListIdMappingWorkflowsOutputTypeDef(TypedDict):
    nextToken: str,
    workflowSummaries: List[IdMappingWorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdMappingWorkflowSummaryTypeDef](./type_defs.md#idmappingworkflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProviderPropertiesTypeDef

```python
# ProviderPropertiesTypeDef definition

class ProviderPropertiesTypeDef(TypedDict):
    providerServiceArn: str,
    intermediateSourceConfiguration: NotRequired[IntermediateSourceConfigurationTypeDef],  # (1)
    providerConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef) 
## ListIdMappingJobsOutputTypeDef

```python
# ListIdMappingJobsOutputTypeDef definition

class ListIdMappingJobsOutputTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMatchingJobsOutputTypeDef

```python
# ListMatchingJobsOutputTypeDef definition

class ListMatchingJobsOutputTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef

```python
# ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef definition

class ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef(TypedDict):
    workflowName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef

```python
# ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef definition

class ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingJobsInputListMatchingJobsPaginateTypeDef

```python
# ListMatchingJobsInputListMatchingJobsPaginateTypeDef definition

class ListMatchingJobsInputListMatchingJobsPaginateTypeDef(TypedDict):
    workflowName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef

```python
# ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef definition

class ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProviderServicesInputListProviderServicesPaginateTypeDef

```python
# ListProviderServicesInputListProviderServicesPaginateTypeDef definition

class ListProviderServicesInputListProviderServicesPaginateTypeDef(TypedDict):
    providerName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef

```python
# ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef definition

class ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingWorkflowsOutputTypeDef

```python
# ListMatchingWorkflowsOutputTypeDef definition

class ListMatchingWorkflowsOutputTypeDef(TypedDict):
    nextToken: str,
    workflowSummaries: List[MatchingWorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchingWorkflowSummaryTypeDef](./type_defs.md#matchingworkflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProviderServicesOutputTypeDef

```python
# ListProviderServicesOutputTypeDef definition

class ListProviderServicesOutputTypeDef(TypedDict):
    nextToken: str,
    providerServiceSummaries: List[ProviderServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProviderServiceSummaryTypeDef](./type_defs.md#providerservicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemaMappingsOutputTypeDef

```python
# ListSchemaMappingsOutputTypeDef definition

class ListSchemaMappingsOutputTypeDef(TypedDict):
    nextToken: str,
    schemaList: List[SchemaMappingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaMappingSummaryTypeDef](./type_defs.md#schemamappingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutputSourceTypeDef

```python
# OutputSourceTypeDef definition

class OutputSourceTypeDef(TypedDict):
    output: Sequence[OutputAttributeTypeDef],  # (1)
    outputS3Path: str,
    KMSArn: NotRequired[str],
    applyNormalization: NotRequired[bool],
```

1. See [:material-code-braces: OutputAttributeTypeDef](./type_defs.md#outputattributetypedef) 
## ProviderEndpointConfigurationTypeDef

```python
# ProviderEndpointConfigurationTypeDef definition

class ProviderEndpointConfigurationTypeDef(TypedDict):
    marketplaceConfiguration: NotRequired[ProviderMarketplaceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderMarketplaceConfigurationTypeDef](./type_defs.md#providermarketplaceconfigurationtypedef) 
## RuleBasedPropertiesTypeDef

```python
# RuleBasedPropertiesTypeDef definition

class RuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    rules: Sequence[RuleTypeDef],  # (2)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## IdMappingTechniquesTypeDef

```python
# IdMappingTechniquesTypeDef definition

class IdMappingTechniquesTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: ProviderPropertiesTypeDef,  # (2)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) 
## GetProviderServiceOutputTypeDef

```python
# GetProviderServiceOutputTypeDef definition

class GetProviderServiceOutputTypeDef(TypedDict):
    anonymizedOutput: bool,
    providerConfigurationDefinition: Dict[str, Any],
    providerEndpointConfiguration: ProviderEndpointConfigurationTypeDef,  # (1)
    providerEntityOutputDefinition: Dict[str, Any],
    providerIntermediateDataAccessConfiguration: ProviderIntermediateDataAccessConfigurationTypeDef,  # (2)
    providerName: str,
    providerServiceArn: str,
    providerServiceDisplayName: str,
    providerServiceName: str,
    providerServiceType: ServiceTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ProviderEndpointConfigurationTypeDef](./type_defs.md#providerendpointconfigurationtypedef) 
2. See [:material-code-braces: ProviderIntermediateDataAccessConfigurationTypeDef](./type_defs.md#providerintermediatedataaccessconfigurationtypedef) 
3. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResolutionTechniquesTypeDef

```python
# ResolutionTechniquesTypeDef definition

class ResolutionTechniquesTypeDef(TypedDict):
    resolutionType: ResolutionTypeType,  # (2)
    providerProperties: NotRequired[ProviderPropertiesTypeDef],  # (1)
    ruleBasedProperties: NotRequired[RuleBasedPropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) 
2. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
3. See [:material-code-braces: RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef) 
## CreateIdMappingWorkflowInputRequestTypeDef

```python
# CreateIdMappingWorkflowInputRequestTypeDef definition

class CreateIdMappingWorkflowInputRequestTypeDef(TypedDict):
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
## CreateIdMappingWorkflowOutputTypeDef

```python
# CreateIdMappingWorkflowOutputTypeDef definition

class CreateIdMappingWorkflowOutputTypeDef(TypedDict):
    description: str,
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: List[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: List[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdMappingWorkflowOutputTypeDef

```python
# GetIdMappingWorkflowOutputTypeDef definition

class GetIdMappingWorkflowOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: List[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: List[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdMappingWorkflowInputRequestTypeDef

```python
# UpdateIdMappingWorkflowInputRequestTypeDef definition

class UpdateIdMappingWorkflowInputRequestTypeDef(TypedDict):
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
## UpdateIdMappingWorkflowOutputTypeDef

```python
# UpdateIdMappingWorkflowOutputTypeDef definition

class UpdateIdMappingWorkflowOutputTypeDef(TypedDict):
    description: str,
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: List[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: List[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMatchingWorkflowInputRequestTypeDef

```python
# CreateMatchingWorkflowInputRequestTypeDef definition

class CreateMatchingWorkflowInputRequestTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
## CreateMatchingWorkflowOutputTypeDef

```python
# CreateMatchingWorkflowOutputTypeDef definition

class CreateMatchingWorkflowOutputTypeDef(TypedDict):
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (4)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
4. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchingWorkflowOutputTypeDef

```python
# GetMatchingWorkflowOutputTypeDef definition

class GetMatchingWorkflowOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (4)
    roleArn: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
4. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMatchingWorkflowInputRequestTypeDef

```python
# UpdateMatchingWorkflowInputRequestTypeDef definition

class UpdateMatchingWorkflowInputRequestTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
## UpdateMatchingWorkflowOutputTypeDef

```python
# UpdateMatchingWorkflowOutputTypeDef definition

class UpdateMatchingWorkflowOutputTypeDef(TypedDict):
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (4)
    roleArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
4. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
