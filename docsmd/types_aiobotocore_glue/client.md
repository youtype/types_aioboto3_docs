# GlueClient

> [Index](../README.md) > [Glue](./README.md) > GlueClient

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## GlueClient

Type annotations and code completion for `#!python session.client("glue")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# GlueClient usage example

from aioboto3.session import Session
from types_aiobotocore_glue.client import GlueClient

session = Session()
async with session.client("glue") as client:
    client: GlueClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("glue").exceptions` structure.

```python
# GlueClient.exceptions usage example

async with session.client("glue") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.AlreadyExistsException,
        client.exceptions.ClientError,
        client.exceptions.ColumnStatisticsTaskNotRunningException,
        client.exceptions.ColumnStatisticsTaskRunningException,
        client.exceptions.ColumnStatisticsTaskStoppingException,
        client.exceptions.ConcurrentModificationException,
        client.exceptions.ConcurrentRunsExceededException,
        client.exceptions.ConditionCheckFailureException,
        client.exceptions.ConflictException,
        client.exceptions.CrawlerNotRunningException,
        client.exceptions.CrawlerRunningException,
        client.exceptions.CrawlerStoppingException,
        client.exceptions.EntityNotFoundException,
        client.exceptions.FederatedResourceAlreadyExistsException,
        client.exceptions.FederationSourceException,
        client.exceptions.FederationSourceRetryableException,
        client.exceptions.GlueEncryptionException,
        client.exceptions.IdempotentParameterMismatchException,
        client.exceptions.IllegalBlueprintStateException,
        client.exceptions.IllegalSessionStateException,
        client.exceptions.IllegalWorkflowStateException,
        client.exceptions.IntegrationConflictOperationFault,
        client.exceptions.IntegrationNotFoundFault,
        client.exceptions.IntegrationQuotaExceededFault,
        client.exceptions.InternalServerException,
        client.exceptions.InternalServiceException,
        client.exceptions.InvalidInputException,
        client.exceptions.InvalidIntegrationStateFault,
        client.exceptions.InvalidStateException,
        client.exceptions.KMSKeyNotAccessibleFault,
        client.exceptions.MLTransformNotReadyException,
        client.exceptions.NoScheduleException,
        client.exceptions.OperationNotSupportedException,
        client.exceptions.OperationTimeoutException,
        client.exceptions.PermissionTypeMismatchException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ResourceNotReadyException,
        client.exceptions.ResourceNumberLimitExceededException,
        client.exceptions.SchedulerNotRunningException,
        client.exceptions.SchedulerRunningException,
        client.exceptions.SchedulerTransitioningException,
        client.exceptions.TargetResourceNotFound,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
        client.exceptions.VersionMismatchException,
    ) as e:
        print(e)
```

```python
# GlueClient.exceptions type checking example

from types_aiobotocore_glue.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("glue").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("glue").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### batch\_create\_partition

Creates one or more partitions in a batch operation.

Type annotations and code completion for `#!python session.client("glue").batch_create_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_create_partition method definition

await def batch_create_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionInputList: Sequence[PartitionInputTypeDef],  # (1)
    CatalogId: str = ...,
) -> BatchCreatePartitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
2. See [:material-code-braces: BatchCreatePartitionResponseTypeDef](./type_defs.md#batchcreatepartitionresponsetypedef) 


```python
# batch_create_partition method usage example with argument unpacking

kwargs: BatchCreatePartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionInputList": ...,
}

parent.batch_create_partition(**kwargs)
```

1. See [:material-code-braces: BatchCreatePartitionRequestRequestTypeDef](./type_defs.md#batchcreatepartitionrequestrequesttypedef) 

### batch\_delete\_connection

Deletes a list of connection definitions from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").batch_delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_delete_connection method definition

await def batch_delete_connection(
    self,
    *,
    ConnectionNameList: Sequence[str],
    CatalogId: str = ...,
) -> BatchDeleteConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteConnectionResponseTypeDef](./type_defs.md#batchdeleteconnectionresponsetypedef) 


```python
# batch_delete_connection method usage example with argument unpacking

kwargs: BatchDeleteConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionNameList": ...,
}

parent.batch_delete_connection(**kwargs)
```

1. See [:material-code-braces: BatchDeleteConnectionRequestRequestTypeDef](./type_defs.md#batchdeleteconnectionrequestrequesttypedef) 

### batch\_delete\_partition

Deletes one or more partitions in a batch operation.

Type annotations and code completion for `#!python session.client("glue").batch_delete_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_delete_partition method definition

await def batch_delete_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionsToDelete: Sequence[PartitionValueListUnionTypeDef],  # (1)
    CatalogId: str = ...,
) -> BatchDeletePartitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) [:material-code-braces: PartitionValueListOutputTypeDef](./type_defs.md#partitionvaluelistoutputtypedef) 
2. See [:material-code-braces: BatchDeletePartitionResponseTypeDef](./type_defs.md#batchdeletepartitionresponsetypedef) 


```python
# batch_delete_partition method usage example with argument unpacking

kwargs: BatchDeletePartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionsToDelete": ...,
}

parent.batch_delete_partition(**kwargs)
```

1. See [:material-code-braces: BatchDeletePartitionRequestRequestTypeDef](./type_defs.md#batchdeletepartitionrequestrequesttypedef) 

### batch\_delete\_table

Deletes multiple tables at once.

Type annotations and code completion for `#!python session.client("glue").batch_delete_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_delete_table method definition

await def batch_delete_table(
    self,
    *,
    DatabaseName: str,
    TablesToDelete: Sequence[str],
    CatalogId: str = ...,
    TransactionId: str = ...,
) -> BatchDeleteTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteTableResponseTypeDef](./type_defs.md#batchdeletetableresponsetypedef) 


```python
# batch_delete_table method usage example with argument unpacking

kwargs: BatchDeleteTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TablesToDelete": ...,
}

parent.batch_delete_table(**kwargs)
```

1. See [:material-code-braces: BatchDeleteTableRequestRequestTypeDef](./type_defs.md#batchdeletetablerequestrequesttypedef) 

### batch\_delete\_table\_version

Deletes a specified batch of versions of a table.

Type annotations and code completion for `#!python session.client("glue").batch_delete_table_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_delete_table_version method definition

await def batch_delete_table_version(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    VersionIds: Sequence[str],
    CatalogId: str = ...,
) -> BatchDeleteTableVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteTableVersionResponseTypeDef](./type_defs.md#batchdeletetableversionresponsetypedef) 


```python
# batch_delete_table_version method usage example with argument unpacking

kwargs: BatchDeleteTableVersionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "VersionIds": ...,
}

parent.batch_delete_table_version(**kwargs)
```

1. See [:material-code-braces: BatchDeleteTableVersionRequestRequestTypeDef](./type_defs.md#batchdeletetableversionrequestrequesttypedef) 

### batch\_get\_blueprints

Retrieves information about a list of blueprints.

Type annotations and code completion for `#!python session.client("glue").batch_get_blueprints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_blueprints method definition

await def batch_get_blueprints(
    self,
    *,
    Names: Sequence[str],
    IncludeBlueprint: bool = ...,
    IncludeParameterSpec: bool = ...,
) -> BatchGetBlueprintsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetBlueprintsResponseTypeDef](./type_defs.md#batchgetblueprintsresponsetypedef) 


```python
# batch_get_blueprints method usage example with argument unpacking

kwargs: BatchGetBlueprintsRequestRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.batch_get_blueprints(**kwargs)
```

1. See [:material-code-braces: BatchGetBlueprintsRequestRequestTypeDef](./type_defs.md#batchgetblueprintsrequestrequesttypedef) 

### batch\_get\_crawlers

Returns a list of resource metadata for a given list of crawler names.

Type annotations and code completion for `#!python session.client("glue").batch_get_crawlers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_crawlers method definition

await def batch_get_crawlers(
    self,
    *,
    CrawlerNames: Sequence[str],
) -> BatchGetCrawlersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetCrawlersResponseTypeDef](./type_defs.md#batchgetcrawlersresponsetypedef) 


```python
# batch_get_crawlers method usage example with argument unpacking

kwargs: BatchGetCrawlersRequestRequestTypeDef = {  # (1)
    "CrawlerNames": ...,
}

parent.batch_get_crawlers(**kwargs)
```

1. See [:material-code-braces: BatchGetCrawlersRequestRequestTypeDef](./type_defs.md#batchgetcrawlersrequestrequesttypedef) 

### batch\_get\_custom\_entity\_types

Retrieves the details for the custom patterns specified by a list of names.

Type annotations and code completion for `#!python session.client("glue").batch_get_custom_entity_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_custom_entity_types method definition

await def batch_get_custom_entity_types(
    self,
    *,
    Names: Sequence[str],
) -> BatchGetCustomEntityTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetCustomEntityTypesResponseTypeDef](./type_defs.md#batchgetcustomentitytypesresponsetypedef) 


```python
# batch_get_custom_entity_types method usage example with argument unpacking

kwargs: BatchGetCustomEntityTypesRequestRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.batch_get_custom_entity_types(**kwargs)
```

1. See [:material-code-braces: BatchGetCustomEntityTypesRequestRequestTypeDef](./type_defs.md#batchgetcustomentitytypesrequestrequesttypedef) 

### batch\_get\_data\_quality\_result

Retrieves a list of data quality results for the specified result IDs.

Type annotations and code completion for `#!python session.client("glue").batch_get_data_quality_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_data_quality_result method definition

await def batch_get_data_quality_result(
    self,
    *,
    ResultIds: Sequence[str],
) -> BatchGetDataQualityResultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetDataQualityResultResponseTypeDef](./type_defs.md#batchgetdataqualityresultresponsetypedef) 


```python
# batch_get_data_quality_result method usage example with argument unpacking

kwargs: BatchGetDataQualityResultRequestRequestTypeDef = {  # (1)
    "ResultIds": ...,
}

parent.batch_get_data_quality_result(**kwargs)
```

1. See [:material-code-braces: BatchGetDataQualityResultRequestRequestTypeDef](./type_defs.md#batchgetdataqualityresultrequestrequesttypedef) 

### batch\_get\_dev\_endpoints

Returns a list of resource metadata for a given list of development endpoint
names.

Type annotations and code completion for `#!python session.client("glue").batch_get_dev_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_dev_endpoints method definition

await def batch_get_dev_endpoints(
    self,
    *,
    DevEndpointNames: Sequence[str],
) -> BatchGetDevEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetDevEndpointsResponseTypeDef](./type_defs.md#batchgetdevendpointsresponsetypedef) 


```python
# batch_get_dev_endpoints method usage example with argument unpacking

kwargs: BatchGetDevEndpointsRequestRequestTypeDef = {  # (1)
    "DevEndpointNames": ...,
}

parent.batch_get_dev_endpoints(**kwargs)
```

1. See [:material-code-braces: BatchGetDevEndpointsRequestRequestTypeDef](./type_defs.md#batchgetdevendpointsrequestrequesttypedef) 

### batch\_get\_jobs

Returns a list of resource metadata for a given list of job names.

Type annotations and code completion for `#!python session.client("glue").batch_get_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_jobs method definition

await def batch_get_jobs(
    self,
    *,
    JobNames: Sequence[str],
) -> BatchGetJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetJobsResponseTypeDef](./type_defs.md#batchgetjobsresponsetypedef) 


```python
# batch_get_jobs method usage example with argument unpacking

kwargs: BatchGetJobsRequestRequestTypeDef = {  # (1)
    "JobNames": ...,
}

parent.batch_get_jobs(**kwargs)
```

1. See [:material-code-braces: BatchGetJobsRequestRequestTypeDef](./type_defs.md#batchgetjobsrequestrequesttypedef) 

### batch\_get\_partition

Retrieves partitions in a batch request.

Type annotations and code completion for `#!python session.client("glue").batch_get_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_partition method definition

await def batch_get_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionsToGet: Sequence[PartitionValueListTypeDef],  # (1)
    CatalogId: str = ...,
) -> BatchGetPartitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
2. See [:material-code-braces: BatchGetPartitionResponseTypeDef](./type_defs.md#batchgetpartitionresponsetypedef) 


```python
# batch_get_partition method usage example with argument unpacking

kwargs: BatchGetPartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionsToGet": ...,
}

parent.batch_get_partition(**kwargs)
```

1. See [:material-code-braces: BatchGetPartitionRequestRequestTypeDef](./type_defs.md#batchgetpartitionrequestrequesttypedef) 

### batch\_get\_table\_optimizer

Returns the configuration for the specified table optimizers.

Type annotations and code completion for `#!python session.client("glue").batch_get_table_optimizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_table_optimizer method definition

await def batch_get_table_optimizer(
    self,
    *,
    Entries: Sequence[BatchGetTableOptimizerEntryTypeDef],  # (1)
) -> BatchGetTableOptimizerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetTableOptimizerEntryTypeDef](./type_defs.md#batchgettableoptimizerentrytypedef) 
2. See [:material-code-braces: BatchGetTableOptimizerResponseTypeDef](./type_defs.md#batchgettableoptimizerresponsetypedef) 


```python
# batch_get_table_optimizer method usage example with argument unpacking

kwargs: BatchGetTableOptimizerRequestRequestTypeDef = {  # (1)
    "Entries": ...,
}

parent.batch_get_table_optimizer(**kwargs)
```

1. See [:material-code-braces: BatchGetTableOptimizerRequestRequestTypeDef](./type_defs.md#batchgettableoptimizerrequestrequesttypedef) 

### batch\_get\_triggers

Returns a list of resource metadata for a given list of trigger names.

Type annotations and code completion for `#!python session.client("glue").batch_get_triggers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_triggers method definition

await def batch_get_triggers(
    self,
    *,
    TriggerNames: Sequence[str],
) -> BatchGetTriggersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetTriggersResponseTypeDef](./type_defs.md#batchgettriggersresponsetypedef) 


```python
# batch_get_triggers method usage example with argument unpacking

kwargs: BatchGetTriggersRequestRequestTypeDef = {  # (1)
    "TriggerNames": ...,
}

parent.batch_get_triggers(**kwargs)
```

1. See [:material-code-braces: BatchGetTriggersRequestRequestTypeDef](./type_defs.md#batchgettriggersrequestrequesttypedef) 

### batch\_get\_workflows

Returns a list of resource metadata for a given list of workflow names.

Type annotations and code completion for `#!python session.client("glue").batch_get_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_get_workflows method definition

await def batch_get_workflows(
    self,
    *,
    Names: Sequence[str],
    IncludeGraph: bool = ...,
) -> BatchGetWorkflowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetWorkflowsResponseTypeDef](./type_defs.md#batchgetworkflowsresponsetypedef) 


```python
# batch_get_workflows method usage example with argument unpacking

kwargs: BatchGetWorkflowsRequestRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.batch_get_workflows(**kwargs)
```

1. See [:material-code-braces: BatchGetWorkflowsRequestRequestTypeDef](./type_defs.md#batchgetworkflowsrequestrequesttypedef) 

### batch\_put\_data\_quality\_statistic\_annotation

Annotate datapoints over time for a specific data quality statistic.

Type annotations and code completion for `#!python session.client("glue").batch_put_data_quality_statistic_annotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_put_data_quality_statistic_annotation method definition

await def batch_put_data_quality_statistic_annotation(
    self,
    *,
    InclusionAnnotations: Sequence[DatapointInclusionAnnotationTypeDef],  # (1)
    ClientToken: str = ...,
) -> BatchPutDataQualityStatisticAnnotationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DatapointInclusionAnnotationTypeDef](./type_defs.md#datapointinclusionannotationtypedef) 
2. See [:material-code-braces: BatchPutDataQualityStatisticAnnotationResponseTypeDef](./type_defs.md#batchputdataqualitystatisticannotationresponsetypedef) 


```python
# batch_put_data_quality_statistic_annotation method usage example with argument unpacking

kwargs: BatchPutDataQualityStatisticAnnotationRequestRequestTypeDef = {  # (1)
    "InclusionAnnotations": ...,
}

parent.batch_put_data_quality_statistic_annotation(**kwargs)
```

1. See [:material-code-braces: BatchPutDataQualityStatisticAnnotationRequestRequestTypeDef](./type_defs.md#batchputdataqualitystatisticannotationrequestrequesttypedef) 

### batch\_stop\_job\_run

Stops one or more job runs for a specified job definition.

Type annotations and code completion for `#!python session.client("glue").batch_stop_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_stop_job_run method definition

await def batch_stop_job_run(
    self,
    *,
    JobName: str,
    JobRunIds: Sequence[str],
) -> BatchStopJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchStopJobRunResponseTypeDef](./type_defs.md#batchstopjobrunresponsetypedef) 


```python
# batch_stop_job_run method usage example with argument unpacking

kwargs: BatchStopJobRunRequestRequestTypeDef = {  # (1)
    "JobName": ...,
    "JobRunIds": ...,
}

parent.batch_stop_job_run(**kwargs)
```

1. See [:material-code-braces: BatchStopJobRunRequestRequestTypeDef](./type_defs.md#batchstopjobrunrequestrequesttypedef) 

### batch\_update\_partition

Updates one or more partitions in a batch operation.

Type annotations and code completion for `#!python session.client("glue").batch_update_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# batch_update_partition method definition

await def batch_update_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    Entries: Sequence[BatchUpdatePartitionRequestEntryTypeDef],  # (1)
    CatalogId: str = ...,
) -> BatchUpdatePartitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchUpdatePartitionRequestEntryTypeDef](./type_defs.md#batchupdatepartitionrequestentrytypedef) 
2. See [:material-code-braces: BatchUpdatePartitionResponseTypeDef](./type_defs.md#batchupdatepartitionresponsetypedef) 


```python
# batch_update_partition method usage example with argument unpacking

kwargs: BatchUpdatePartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "Entries": ...,
}

parent.batch_update_partition(**kwargs)
```

1. See [:material-code-braces: BatchUpdatePartitionRequestRequestTypeDef](./type_defs.md#batchupdatepartitionrequestrequesttypedef) 

### cancel\_data\_quality\_rule\_recommendation\_run

Cancels the specified recommendation run that was being used to generate rules.

Type annotations and code completion for `#!python session.client("glue").cancel_data_quality_rule_recommendation_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# cancel_data_quality_rule_recommendation_run method definition

await def cancel_data_quality_rule_recommendation_run(
    self,
    *,
    RunId: str,
) -> dict[str, Any]:
    ...
```



```python
# cancel_data_quality_rule_recommendation_run method usage example with argument unpacking

kwargs: CancelDataQualityRuleRecommendationRunRequestRequestTypeDef = {  # (1)
    "RunId": ...,
}

parent.cancel_data_quality_rule_recommendation_run(**kwargs)
```

1. See [:material-code-braces: CancelDataQualityRuleRecommendationRunRequestRequestTypeDef](./type_defs.md#canceldataqualityrulerecommendationrunrequestrequesttypedef) 

### cancel\_data\_quality\_ruleset\_evaluation\_run

Cancels a run where a ruleset is being evaluated against a data source.

Type annotations and code completion for `#!python session.client("glue").cancel_data_quality_ruleset_evaluation_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# cancel_data_quality_ruleset_evaluation_run method definition

await def cancel_data_quality_ruleset_evaluation_run(
    self,
    *,
    RunId: str,
) -> dict[str, Any]:
    ...
```



```python
# cancel_data_quality_ruleset_evaluation_run method usage example with argument unpacking

kwargs: CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef = {  # (1)
    "RunId": ...,
}

parent.cancel_data_quality_ruleset_evaluation_run(**kwargs)
```

1. See [:material-code-braces: CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef](./type_defs.md#canceldataqualityrulesetevaluationrunrequestrequesttypedef) 

### cancel\_ml\_task\_run

Cancels (stops) a task run.

Type annotations and code completion for `#!python session.client("glue").cancel_ml_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# cancel_ml_task_run method definition

await def cancel_ml_task_run(
    self,
    *,
    TransformId: str,
    TaskRunId: str,
) -> CancelMLTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelMLTaskRunResponseTypeDef](./type_defs.md#cancelmltaskrunresponsetypedef) 


```python
# cancel_ml_task_run method usage example with argument unpacking

kwargs: CancelMLTaskRunRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
    "TaskRunId": ...,
}

parent.cancel_ml_task_run(**kwargs)
```

1. See [:material-code-braces: CancelMLTaskRunRequestRequestTypeDef](./type_defs.md#cancelmltaskrunrequestrequesttypedef) 

### cancel\_statement

Cancels the statement.

Type annotations and code completion for `#!python session.client("glue").cancel_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# cancel_statement method definition

await def cancel_statement(
    self,
    *,
    SessionId: str,
    Id: int,
    RequestOrigin: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# cancel_statement method usage example with argument unpacking

kwargs: CancelStatementRequestRequestTypeDef = {  # (1)
    "SessionId": ...,
    "Id": ...,
}

parent.cancel_statement(**kwargs)
```

1. See [:material-code-braces: CancelStatementRequestRequestTypeDef](./type_defs.md#cancelstatementrequestrequesttypedef) 

### check\_schema\_version\_validity

Validates the supplied schema.

Type annotations and code completion for `#!python session.client("glue").check_schema_version_validity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# check_schema_version_validity method definition

await def check_schema_version_validity(
    self,
    *,
    DataFormat: DataFormatType,  # (1)
    SchemaDefinition: str,
) -> CheckSchemaVersionValidityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-braces: CheckSchemaVersionValidityResponseTypeDef](./type_defs.md#checkschemaversionvalidityresponsetypedef) 


```python
# check_schema_version_validity method usage example with argument unpacking

kwargs: CheckSchemaVersionValidityInputRequestTypeDef = {  # (1)
    "DataFormat": ...,
    "SchemaDefinition": ...,
}

parent.check_schema_version_validity(**kwargs)
```

1. See [:material-code-braces: CheckSchemaVersionValidityInputRequestTypeDef](./type_defs.md#checkschemaversionvalidityinputrequesttypedef) 

### create\_blueprint

Registers a blueprint with Glue.

Type annotations and code completion for `#!python session.client("glue").create_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_blueprint method definition

await def create_blueprint(
    self,
    *,
    Name: str,
    BlueprintLocation: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateBlueprintResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateBlueprintResponseTypeDef](./type_defs.md#createblueprintresponsetypedef) 


```python
# create_blueprint method usage example with argument unpacking

kwargs: CreateBlueprintRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "BlueprintLocation": ...,
}

parent.create_blueprint(**kwargs)
```

1. See [:material-code-braces: CreateBlueprintRequestRequestTypeDef](./type_defs.md#createblueprintrequestrequesttypedef) 

### create\_catalog

Creates a new catalog in the Glue Data Catalog.

Type annotations and code completion for `#!python session.client("glue").create_catalog` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_catalog method definition

await def create_catalog(
    self,
    *,
    Name: str,
    CatalogInput: CatalogInputTypeDef,  # (1)
    Tags: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: CatalogInputTypeDef](./type_defs.md#cataloginputtypedef) 


```python
# create_catalog method usage example with argument unpacking

kwargs: CreateCatalogRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "CatalogInput": ...,
}

parent.create_catalog(**kwargs)
```

1. See [:material-code-braces: CreateCatalogRequestRequestTypeDef](./type_defs.md#createcatalogrequestrequesttypedef) 

### create\_classifier

Creates a classifier in the user's account.

Type annotations and code completion for `#!python session.client("glue").create_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_classifier method definition

await def create_classifier(
    self,
    *,
    GrokClassifier: CreateGrokClassifierRequestTypeDef = ...,  # (1)
    XMLClassifier: CreateXMLClassifierRequestTypeDef = ...,  # (2)
    JsonClassifier: CreateJsonClassifierRequestTypeDef = ...,  # (3)
    CsvClassifier: CreateCsvClassifierRequestTypeDef = ...,  # (4)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: CreateGrokClassifierRequestTypeDef](./type_defs.md#creategrokclassifierrequesttypedef) 
2. See [:material-code-braces: CreateXMLClassifierRequestTypeDef](./type_defs.md#createxmlclassifierrequesttypedef) 
3. See [:material-code-braces: CreateJsonClassifierRequestTypeDef](./type_defs.md#createjsonclassifierrequesttypedef) 
4. See [:material-code-braces: CreateCsvClassifierRequestTypeDef](./type_defs.md#createcsvclassifierrequesttypedef) 


```python
# create_classifier method usage example with argument unpacking

kwargs: CreateClassifierRequestRequestTypeDef = {  # (1)
    "GrokClassifier": ...,
}

parent.create_classifier(**kwargs)
```

1. See [:material-code-braces: CreateClassifierRequestRequestTypeDef](./type_defs.md#createclassifierrequestrequesttypedef) 

### create\_column\_statistics\_task\_settings

Creates settings for a column statistics task.

Type annotations and code completion for `#!python session.client("glue").create_column_statistics_task_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_column_statistics_task_settings method definition

await def create_column_statistics_task_settings(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    Role: str,
    Schedule: str = ...,
    ColumnNameList: Sequence[str] = ...,
    SampleSize: float = ...,
    CatalogID: str = ...,
    SecurityConfiguration: str = ...,
    Tags: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```



```python
# create_column_statistics_task_settings method usage example with argument unpacking

kwargs: CreateColumnStatisticsTaskSettingsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "Role": ...,
}

parent.create_column_statistics_task_settings(**kwargs)
```

1. See [:material-code-braces: CreateColumnStatisticsTaskSettingsRequestRequestTypeDef](./type_defs.md#createcolumnstatisticstasksettingsrequestrequesttypedef) 

### create\_connection

Creates a connection definition in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").create_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_connection method definition

await def create_connection(
    self,
    *,
    ConnectionInput: ConnectionInputTypeDef,  # (1)
    CatalogId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateConnectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConnectionInputTypeDef](./type_defs.md#connectioninputtypedef) 
2. See [:material-code-braces: CreateConnectionResponseTypeDef](./type_defs.md#createconnectionresponsetypedef) 


```python
# create_connection method usage example with argument unpacking

kwargs: CreateConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionInput": ...,
}

parent.create_connection(**kwargs)
```

1. See [:material-code-braces: CreateConnectionRequestRequestTypeDef](./type_defs.md#createconnectionrequestrequesttypedef) 

### create\_crawler

Creates a new crawler with specified targets, role, configuration, and optional
schedule.

Type annotations and code completion for `#!python session.client("glue").create_crawler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_crawler method definition

await def create_crawler(
    self,
    *,
    Name: str,
    Role: str,
    Targets: CrawlerTargetsTypeDef,  # (1)
    DatabaseName: str = ...,
    Description: str = ...,
    Schedule: str = ...,
    Classifiers: Sequence[str] = ...,
    TablePrefix: str = ...,
    SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,  # (2)
    RecrawlPolicy: RecrawlPolicyTypeDef = ...,  # (3)
    LineageConfiguration: LineageConfigurationTypeDef = ...,  # (4)
    LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,  # (5)
    Configuration: str = ...,
    CrawlerSecurityConfiguration: str = ...,
    Tags: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
3. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 


```python
# create_crawler method usage example with argument unpacking

kwargs: CreateCrawlerRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Role": ...,
    "Targets": ...,
}

parent.create_crawler(**kwargs)
```

1. See [:material-code-braces: CreateCrawlerRequestRequestTypeDef](./type_defs.md#createcrawlerrequestrequesttypedef) 

### create\_custom\_entity\_type

Creates a custom pattern that is used to detect sensitive data across the
columns and rows of your structured data.

Type annotations and code completion for `#!python session.client("glue").create_custom_entity_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_custom_entity_type method definition

await def create_custom_entity_type(
    self,
    *,
    Name: str,
    RegexString: str,
    ContextWords: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateCustomEntityTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateCustomEntityTypeResponseTypeDef](./type_defs.md#createcustomentitytyperesponsetypedef) 


```python
# create_custom_entity_type method usage example with argument unpacking

kwargs: CreateCustomEntityTypeRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RegexString": ...,
}

parent.create_custom_entity_type(**kwargs)
```

1. See [:material-code-braces: CreateCustomEntityTypeRequestRequestTypeDef](./type_defs.md#createcustomentitytyperequestrequesttypedef) 

### create\_data\_quality\_ruleset

Creates a data quality ruleset with DQDL rules applied to a specified Glue
table.

Type annotations and code completion for `#!python session.client("glue").create_data_quality_ruleset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_data_quality_ruleset method definition

await def create_data_quality_ruleset(
    self,
    *,
    Name: str,
    Ruleset: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
    TargetTable: DataQualityTargetTableTypeDef = ...,  # (1)
    DataQualitySecurityConfiguration: str = ...,
    ClientToken: str = ...,
) -> CreateDataQualityRulesetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
2. See [:material-code-braces: CreateDataQualityRulesetResponseTypeDef](./type_defs.md#createdataqualityrulesetresponsetypedef) 


```python
# create_data_quality_ruleset method usage example with argument unpacking

kwargs: CreateDataQualityRulesetRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Ruleset": ...,
}

parent.create_data_quality_ruleset(**kwargs)
```

1. See [:material-code-braces: CreateDataQualityRulesetRequestRequestTypeDef](./type_defs.md#createdataqualityrulesetrequestrequesttypedef) 

### create\_database

Creates a new database in a Data Catalog.

Type annotations and code completion for `#!python session.client("glue").create_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_database method definition

await def create_database(
    self,
    *,
    DatabaseInput: DatabaseInputTypeDef,  # (1)
    CatalogId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DatabaseInputTypeDef](./type_defs.md#databaseinputtypedef) 


```python
# create_database method usage example with argument unpacking

kwargs: CreateDatabaseRequestRequestTypeDef = {  # (1)
    "DatabaseInput": ...,
}

parent.create_database(**kwargs)
```

1. See [:material-code-braces: CreateDatabaseRequestRequestTypeDef](./type_defs.md#createdatabaserequestrequesttypedef) 

### create\_dev\_endpoint

Creates a new development endpoint.

Type annotations and code completion for `#!python session.client("glue").create_dev_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_dev_endpoint method definition

await def create_dev_endpoint(
    self,
    *,
    EndpointName: str,
    RoleArn: str,
    SecurityGroupIds: Sequence[str] = ...,
    SubnetId: str = ...,
    PublicKey: str = ...,
    PublicKeys: Sequence[str] = ...,
    NumberOfNodes: int = ...,
    WorkerType: WorkerTypeType = ...,  # (1)
    GlueVersion: str = ...,
    NumberOfWorkers: int = ...,
    ExtraPythonLibsS3Path: str = ...,
    ExtraJarsS3Path: str = ...,
    SecurityConfiguration: str = ...,
    Tags: Mapping[str, str] = ...,
    Arguments: Mapping[str, str] = ...,
) -> CreateDevEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
2. See [:material-code-braces: CreateDevEndpointResponseTypeDef](./type_defs.md#createdevendpointresponsetypedef) 


```python
# create_dev_endpoint method usage example with argument unpacking

kwargs: CreateDevEndpointRequestRequestTypeDef = {  # (1)
    "EndpointName": ...,
    "RoleArn": ...,
}

parent.create_dev_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateDevEndpointRequestRequestTypeDef](./type_defs.md#createdevendpointrequestrequesttypedef) 

### create\_integration

Creates a Zero-ETL integration in the caller's account between two resources
with Amazon Resource Names (ARNs): the <code>SourceArn</code> and
<code>TargetArn</code>.

Type annotations and code completion for `#!python session.client("glue").create_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_integration method definition

await def create_integration(
    self,
    *,
    IntegrationName: str,
    SourceArn: str,
    TargetArn: str,
    Description: str = ...,
    DataFilter: str = ...,
    KmsKeyId: str = ...,
    AdditionalEncryptionContext: Mapping[str, str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateIntegrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateIntegrationResponseTypeDef](./type_defs.md#createintegrationresponsetypedef) 


```python
# create_integration method usage example with argument unpacking

kwargs: CreateIntegrationRequestRequestTypeDef = {  # (1)
    "IntegrationName": ...,
    "SourceArn": ...,
    "TargetArn": ...,
}

parent.create_integration(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationRequestRequestTypeDef](./type_defs.md#createintegrationrequestrequesttypedef) 

### create\_integration\_resource\_property

This API can be used for setting up the <code>ResourceProperty</code> of the
Glue connection (for the source) or Glue database ARN (for the target).

Type annotations and code completion for `#!python session.client("glue").create_integration_resource_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_integration_resource_property method definition

await def create_integration_resource_property(
    self,
    *,
    ResourceArn: str,
    SourceProcessingProperties: SourceProcessingPropertiesTypeDef = ...,  # (1)
    TargetProcessingProperties: TargetProcessingPropertiesTypeDef = ...,  # (2)
) -> CreateIntegrationResourcePropertyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
3. See [:material-code-braces: CreateIntegrationResourcePropertyResponseTypeDef](./type_defs.md#createintegrationresourcepropertyresponsetypedef) 


```python
# create_integration_resource_property method usage example with argument unpacking

kwargs: CreateIntegrationResourcePropertyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.create_integration_resource_property(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationResourcePropertyRequestRequestTypeDef](./type_defs.md#createintegrationresourcepropertyrequestrequesttypedef) 

### create\_integration\_table\_properties

This API is used to provide optional override properties for the the tables
that need to be replicated.

Type annotations and code completion for `#!python session.client("glue").create_integration_table_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_integration_table_properties method definition

await def create_integration_table_properties(
    self,
    *,
    ResourceArn: str,
    TableName: str,
    SourceTableConfig: SourceTableConfigTypeDef = ...,  # (1)
    TargetTableConfig: TargetTableConfigTypeDef = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: SourceTableConfigTypeDef](./type_defs.md#sourcetableconfigtypedef) 
2. See [:material-code-braces: TargetTableConfigTypeDef](./type_defs.md#targettableconfigtypedef) 


```python
# create_integration_table_properties method usage example with argument unpacking

kwargs: CreateIntegrationTablePropertiesRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TableName": ...,
}

parent.create_integration_table_properties(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationTablePropertiesRequestRequestTypeDef](./type_defs.md#createintegrationtablepropertiesrequestrequesttypedef) 

### create\_job

Creates a new job definition.

Type annotations and code completion for `#!python session.client("glue").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_job method definition

await def create_job(
    self,
    *,
    Name: str,
    Role: str,
    Command: JobCommandTypeDef,  # (1)
    JobMode: JobModeType = ...,  # (2)
    JobRunQueuingEnabled: bool = ...,
    Description: str = ...,
    LogUri: str = ...,
    ExecutionProperty: ExecutionPropertyTypeDef = ...,  # (3)
    DefaultArguments: Mapping[str, str] = ...,
    NonOverridableArguments: Mapping[str, str] = ...,
    Connections: ConnectionsListTypeDef = ...,  # (4)
    MaxRetries: int = ...,
    AllocatedCapacity: int = ...,
    Timeout: int = ...,
    MaxCapacity: float = ...,
    SecurityConfiguration: str = ...,
    Tags: Mapping[str, str] = ...,
    NotificationProperty: NotificationPropertyTypeDef = ...,  # (5)
    GlueVersion: str = ...,
    NumberOfWorkers: int = ...,
    WorkerType: WorkerTypeType = ...,  # (6)
    CodeGenConfigurationNodes: Mapping[str, CodeGenConfigurationNodeUnionTypeDef] = ...,  # (7)
    ExecutionClass: ExecutionClassType = ...,  # (8)
    SourceControlDetails: SourceControlDetailsTypeDef = ...,  # (9)
    MaintenanceWindow: str = ...,
) -> CreateJobResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
2. See [:material-code-brackets: JobModeType](./literals.md#jobmodetype) 
3. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
4. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
5. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
6. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
7. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) [:material-code-braces: CodeGenConfigurationNodeOutputTypeDef](./type_defs.md#codegenconfigurationnodeoutputtypedef) 
8. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
9. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
10. See [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Role": ...,
    "Command": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 

### create\_ml\_transform

Creates an Glue machine learning transform.

Type annotations and code completion for `#!python session.client("glue").create_ml_transform` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_ml_transform method definition

await def create_ml_transform(
    self,
    *,
    Name: str,
    InputRecordTables: Sequence[GlueTableUnionTypeDef],  # (1)
    Parameters: TransformParametersTypeDef,  # (2)
    Role: str,
    Description: str = ...,
    GlueVersion: str = ...,
    MaxCapacity: float = ...,
    WorkerType: WorkerTypeType = ...,  # (3)
    NumberOfWorkers: int = ...,
    Timeout: int = ...,
    MaxRetries: int = ...,
    Tags: Mapping[str, str] = ...,
    TransformEncryption: TransformEncryptionTypeDef = ...,  # (4)
) -> CreateMLTransformResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 
2. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
4. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
5. See [:material-code-braces: CreateMLTransformResponseTypeDef](./type_defs.md#createmltransformresponsetypedef) 


```python
# create_ml_transform method usage example with argument unpacking

kwargs: CreateMLTransformRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "InputRecordTables": ...,
    "Parameters": ...,
    "Role": ...,
}

parent.create_ml_transform(**kwargs)
```

1. See [:material-code-braces: CreateMLTransformRequestRequestTypeDef](./type_defs.md#createmltransformrequestrequesttypedef) 

### create\_partition

Creates a new partition.

Type annotations and code completion for `#!python session.client("glue").create_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_partition method definition

await def create_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionInput: PartitionInputTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 


```python
# create_partition method usage example with argument unpacking

kwargs: CreatePartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionInput": ...,
}

parent.create_partition(**kwargs)
```

1. See [:material-code-braces: CreatePartitionRequestRequestTypeDef](./type_defs.md#createpartitionrequestrequesttypedef) 

### create\_partition\_index

Creates a specified partition index in an existing table.

Type annotations and code completion for `#!python session.client("glue").create_partition_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_partition_index method definition

await def create_partition_index(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionIndex: PartitionIndexTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: PartitionIndexTypeDef](./type_defs.md#partitionindextypedef) 


```python
# create_partition_index method usage example with argument unpacking

kwargs: CreatePartitionIndexRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionIndex": ...,
}

parent.create_partition_index(**kwargs)
```

1. See [:material-code-braces: CreatePartitionIndexRequestRequestTypeDef](./type_defs.md#createpartitionindexrequestrequesttypedef) 

### create\_registry

Creates a new registry which may be used to hold a collection of schemas.

Type annotations and code completion for `#!python session.client("glue").create_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_registry method definition

await def create_registry(
    self,
    *,
    RegistryName: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateRegistryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRegistryResponseTypeDef](./type_defs.md#createregistryresponsetypedef) 


```python
# create_registry method usage example with argument unpacking

kwargs: CreateRegistryInputRequestTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.create_registry(**kwargs)
```

1. See [:material-code-braces: CreateRegistryInputRequestTypeDef](./type_defs.md#createregistryinputrequesttypedef) 

### create\_schema

Creates a new schema set and registers the schema definition.

Type annotations and code completion for `#!python session.client("glue").create_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_schema method definition

await def create_schema(
    self,
    *,
    SchemaName: str,
    DataFormat: DataFormatType,  # (1)
    RegistryId: RegistryIdTypeDef = ...,  # (2)
    Compatibility: CompatibilityType = ...,  # (3)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
    SchemaDefinition: str = ...,
) -> CreateSchemaResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
3. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
4. See [:material-code-braces: CreateSchemaResponseTypeDef](./type_defs.md#createschemaresponsetypedef) 


```python
# create_schema method usage example with argument unpacking

kwargs: CreateSchemaInputRequestTypeDef = {  # (1)
    "SchemaName": ...,
    "DataFormat": ...,
}

parent.create_schema(**kwargs)
```

1. See [:material-code-braces: CreateSchemaInputRequestTypeDef](./type_defs.md#createschemainputrequesttypedef) 

### create\_script

Transforms a directed acyclic graph (DAG) into code.

Type annotations and code completion for `#!python session.client("glue").create_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_script method definition

await def create_script(
    self,
    *,
    DagNodes: Sequence[CodeGenNodeUnionTypeDef] = ...,  # (1)
    DagEdges: Sequence[CodeGenEdgeTypeDef] = ...,  # (2)
    Language: LanguageType = ...,  # (3)
) -> CreateScriptResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: CodeGenNodeTypeDef](./type_defs.md#codegennodetypedef) [:material-code-braces: CodeGenNodeOutputTypeDef](./type_defs.md#codegennodeoutputtypedef) 
2. See [:material-code-braces: CodeGenEdgeTypeDef](./type_defs.md#codegenedgetypedef) 
3. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
4. See [:material-code-braces: CreateScriptResponseTypeDef](./type_defs.md#createscriptresponsetypedef) 


```python
# create_script method usage example with argument unpacking

kwargs: CreateScriptRequestRequestTypeDef = {  # (1)
    "DagNodes": ...,
}

parent.create_script(**kwargs)
```

1. See [:material-code-braces: CreateScriptRequestRequestTypeDef](./type_defs.md#createscriptrequestrequesttypedef) 

### create\_security\_configuration

Creates a new security configuration.

Type annotations and code completion for `#!python session.client("glue").create_security_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_security_configuration method definition

await def create_security_configuration(
    self,
    *,
    Name: str,
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (1)
) -> CreateSecurityConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: CreateSecurityConfigurationResponseTypeDef](./type_defs.md#createsecurityconfigurationresponsetypedef) 


```python
# create_security_configuration method usage example with argument unpacking

kwargs: CreateSecurityConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "EncryptionConfiguration": ...,
}

parent.create_security_configuration(**kwargs)
```

1. See [:material-code-braces: CreateSecurityConfigurationRequestRequestTypeDef](./type_defs.md#createsecurityconfigurationrequestrequesttypedef) 

### create\_session

Creates a new session.

Type annotations and code completion for `#!python session.client("glue").create_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_session method definition

await def create_session(
    self,
    *,
    Id: str,
    Role: str,
    Command: SessionCommandTypeDef,  # (1)
    Description: str = ...,
    Timeout: int = ...,
    IdleTimeout: int = ...,
    DefaultArguments: Mapping[str, str] = ...,
    Connections: ConnectionsListTypeDef = ...,  # (2)
    MaxCapacity: float = ...,
    NumberOfWorkers: int = ...,
    WorkerType: WorkerTypeType = ...,  # (3)
    SecurityConfiguration: str = ...,
    GlueVersion: str = ...,
    Tags: Mapping[str, str] = ...,
    RequestOrigin: str = ...,
) -> CreateSessionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SessionCommandTypeDef](./type_defs.md#sessioncommandtypedef) 
2. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
4. See [:material-code-braces: CreateSessionResponseTypeDef](./type_defs.md#createsessionresponsetypedef) 


```python
# create_session method usage example with argument unpacking

kwargs: CreateSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "Role": ...,
    "Command": ...,
}

parent.create_session(**kwargs)
```

1. See [:material-code-braces: CreateSessionRequestRequestTypeDef](./type_defs.md#createsessionrequestrequesttypedef) 

### create\_table

Creates a new table definition in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").create_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_table method definition

await def create_table(
    self,
    *,
    DatabaseName: str,
    TableInput: TableInputTypeDef,  # (1)
    CatalogId: str = ...,
    PartitionIndexes: Sequence[PartitionIndexTypeDef] = ...,  # (2)
    TransactionId: str = ...,
    OpenTableFormatInput: OpenTableFormatInputTypeDef = ...,  # (3)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TableInputTypeDef](./type_defs.md#tableinputtypedef) 
2. See [:material-code-braces: PartitionIndexTypeDef](./type_defs.md#partitionindextypedef) 
3. See [:material-code-braces: OpenTableFormatInputTypeDef](./type_defs.md#opentableformatinputtypedef) 


```python
# create_table method usage example with argument unpacking

kwargs: CreateTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableInput": ...,
}

parent.create_table(**kwargs)
```

1. See [:material-code-braces: CreateTableRequestRequestTypeDef](./type_defs.md#createtablerequestrequesttypedef) 

### create\_table\_optimizer

Creates a new table optimizer for a specific function.

Type annotations and code completion for `#!python session.client("glue").create_table_optimizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_table_optimizer method definition

await def create_table_optimizer(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: TableOptimizerConfigurationTypeDef](./type_defs.md#tableoptimizerconfigurationtypedef) 


```python
# create_table_optimizer method usage example with argument unpacking

kwargs: CreateTableOptimizerRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Type": ...,
    "TableOptimizerConfiguration": ...,
}

parent.create_table_optimizer(**kwargs)
```

1. See [:material-code-braces: CreateTableOptimizerRequestRequestTypeDef](./type_defs.md#createtableoptimizerrequestrequesttypedef) 

### create\_trigger

Creates a new trigger.

Type annotations and code completion for `#!python session.client("glue").create_trigger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_trigger method definition

await def create_trigger(
    self,
    *,
    Name: str,
    Type: TriggerTypeType,  # (1)
    Actions: Sequence[ActionUnionTypeDef],  # (2)
    WorkflowName: str = ...,
    Schedule: str = ...,
    Predicate: PredicateTypeDef = ...,  # (3)
    Description: str = ...,
    StartOnCreation: bool = ...,
    Tags: Mapping[str, str] = ...,
    EventBatchingCondition: EventBatchingConditionTypeDef = ...,  # (4)
) -> CreateTriggerResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
3. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
4. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
5. See [:material-code-braces: CreateTriggerResponseTypeDef](./type_defs.md#createtriggerresponsetypedef) 


```python
# create_trigger method usage example with argument unpacking

kwargs: CreateTriggerRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Type": ...,
    "Actions": ...,
}

parent.create_trigger(**kwargs)
```

1. See [:material-code-braces: CreateTriggerRequestRequestTypeDef](./type_defs.md#createtriggerrequestrequesttypedef) 

### create\_usage\_profile

Creates an Glue usage profile.

Type annotations and code completion for `#!python session.client("glue").create_usage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_usage_profile method definition

await def create_usage_profile(
    self,
    *,
    Name: str,
    Configuration: ProfileConfigurationTypeDef,  # (1)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateUsageProfileResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ProfileConfigurationTypeDef](./type_defs.md#profileconfigurationtypedef) 
2. See [:material-code-braces: CreateUsageProfileResponseTypeDef](./type_defs.md#createusageprofileresponsetypedef) 


```python
# create_usage_profile method usage example with argument unpacking

kwargs: CreateUsageProfileRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Configuration": ...,
}

parent.create_usage_profile(**kwargs)
```

1. See [:material-code-braces: CreateUsageProfileRequestRequestTypeDef](./type_defs.md#createusageprofilerequestrequesttypedef) 

### create\_user\_defined\_function

Creates a new function definition in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").create_user_defined_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_user_defined_function method definition

await def create_user_defined_function(
    self,
    *,
    DatabaseName: str,
    FunctionInput: UserDefinedFunctionInputTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: UserDefinedFunctionInputTypeDef](./type_defs.md#userdefinedfunctioninputtypedef) 


```python
# create_user_defined_function method usage example with argument unpacking

kwargs: CreateUserDefinedFunctionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "FunctionInput": ...,
}

parent.create_user_defined_function(**kwargs)
```

1. See [:material-code-braces: CreateUserDefinedFunctionRequestRequestTypeDef](./type_defs.md#createuserdefinedfunctionrequestrequesttypedef) 

### create\_workflow

Creates a new workflow.

Type annotations and code completion for `#!python session.client("glue").create_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# create_workflow method definition

await def create_workflow(
    self,
    *,
    Name: str,
    Description: str = ...,
    DefaultRunProperties: Mapping[str, str] = ...,
    Tags: Mapping[str, str] = ...,
    MaxConcurrentRuns: int = ...,
) -> CreateWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef) 


```python
# create_workflow method usage example with argument unpacking

kwargs: CreateWorkflowRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_workflow(**kwargs)
```

1. See [:material-code-braces: CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef) 

### delete\_blueprint

Deletes an existing blueprint.

Type annotations and code completion for `#!python session.client("glue").delete_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_blueprint method definition

await def delete_blueprint(
    self,
    *,
    Name: str,
) -> DeleteBlueprintResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBlueprintResponseTypeDef](./type_defs.md#deleteblueprintresponsetypedef) 


```python
# delete_blueprint method usage example with argument unpacking

kwargs: DeleteBlueprintRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_blueprint(**kwargs)
```

1. See [:material-code-braces: DeleteBlueprintRequestRequestTypeDef](./type_defs.md#deleteblueprintrequestrequesttypedef) 

### delete\_catalog

Removes the specified catalog from the Glue Data Catalog.

Type annotations and code completion for `#!python session.client("glue").delete_catalog` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_catalog method definition

await def delete_catalog(
    self,
    *,
    CatalogId: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_catalog method usage example with argument unpacking

kwargs: DeleteCatalogRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.delete_catalog(**kwargs)
```

1. See [:material-code-braces: DeleteCatalogRequestRequestTypeDef](./type_defs.md#deletecatalogrequestrequesttypedef) 

### delete\_classifier

Removes a classifier from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").delete_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_classifier method definition

await def delete_classifier(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_classifier method usage example with argument unpacking

kwargs: DeleteClassifierRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_classifier(**kwargs)
```

1. See [:material-code-braces: DeleteClassifierRequestRequestTypeDef](./type_defs.md#deleteclassifierrequestrequesttypedef) 

### delete\_column\_statistics\_for\_partition

Delete the partition column statistics of a column.

Type annotations and code completion for `#!python session.client("glue").delete_column_statistics_for_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_column_statistics_for_partition method definition

await def delete_column_statistics_for_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnName: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_column_statistics_for_partition method usage example with argument unpacking

kwargs: DeleteColumnStatisticsForPartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValues": ...,
    "ColumnName": ...,
}

parent.delete_column_statistics_for_partition(**kwargs)
```

1. See [:material-code-braces: DeleteColumnStatisticsForPartitionRequestRequestTypeDef](./type_defs.md#deletecolumnstatisticsforpartitionrequestrequesttypedef) 

### delete\_column\_statistics\_for\_table

Retrieves table statistics of columns.

Type annotations and code completion for `#!python session.client("glue").delete_column_statistics_for_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_column_statistics_for_table method definition

await def delete_column_statistics_for_table(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    ColumnName: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_column_statistics_for_table method usage example with argument unpacking

kwargs: DeleteColumnStatisticsForTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "ColumnName": ...,
}

parent.delete_column_statistics_for_table(**kwargs)
```

1. See [:material-code-braces: DeleteColumnStatisticsForTableRequestRequestTypeDef](./type_defs.md#deletecolumnstatisticsfortablerequestrequesttypedef) 

### delete\_column\_statistics\_task\_settings

Deletes settings for a column statistics task.

Type annotations and code completion for `#!python session.client("glue").delete_column_statistics_task_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_column_statistics_task_settings method definition

await def delete_column_statistics_task_settings(
    self,
    *,
    DatabaseName: str,
    TableName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_column_statistics_task_settings method usage example with argument unpacking

kwargs: DeleteColumnStatisticsTaskSettingsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.delete_column_statistics_task_settings(**kwargs)
```

1. See [:material-code-braces: DeleteColumnStatisticsTaskSettingsRequestRequestTypeDef](./type_defs.md#deletecolumnstatisticstasksettingsrequestrequesttypedef) 

### delete\_connection

Deletes a connection from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_connection method definition

await def delete_connection(
    self,
    *,
    ConnectionName: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_connection method usage example with argument unpacking

kwargs: DeleteConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionName": ...,
}

parent.delete_connection(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef) 

### delete\_crawler

Removes a specified crawler from the Glue Data Catalog, unless the crawler
state is <code>RUNNING</code>.

Type annotations and code completion for `#!python session.client("glue").delete_crawler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_crawler method definition

await def delete_crawler(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_crawler method usage example with argument unpacking

kwargs: DeleteCrawlerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_crawler(**kwargs)
```

1. See [:material-code-braces: DeleteCrawlerRequestRequestTypeDef](./type_defs.md#deletecrawlerrequestrequesttypedef) 

### delete\_custom\_entity\_type

Deletes a custom pattern by specifying its name.

Type annotations and code completion for `#!python session.client("glue").delete_custom_entity_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_custom_entity_type method definition

await def delete_custom_entity_type(
    self,
    *,
    Name: str,
) -> DeleteCustomEntityTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCustomEntityTypeResponseTypeDef](./type_defs.md#deletecustomentitytyperesponsetypedef) 


```python
# delete_custom_entity_type method usage example with argument unpacking

kwargs: DeleteCustomEntityTypeRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_custom_entity_type(**kwargs)
```

1. See [:material-code-braces: DeleteCustomEntityTypeRequestRequestTypeDef](./type_defs.md#deletecustomentitytyperequestrequesttypedef) 

### delete\_data\_quality\_ruleset

Deletes a data quality ruleset.

Type annotations and code completion for `#!python session.client("glue").delete_data_quality_ruleset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_data_quality_ruleset method definition

await def delete_data_quality_ruleset(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_data_quality_ruleset method usage example with argument unpacking

kwargs: DeleteDataQualityRulesetRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_data_quality_ruleset(**kwargs)
```

1. See [:material-code-braces: DeleteDataQualityRulesetRequestRequestTypeDef](./type_defs.md#deletedataqualityrulesetrequestrequesttypedef) 

### delete\_database

Removes a specified database from a Data Catalog.

Type annotations and code completion for `#!python session.client("glue").delete_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_database method definition

await def delete_database(
    self,
    *,
    Name: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_database method usage example with argument unpacking

kwargs: DeleteDatabaseRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_database(**kwargs)
```

1. See [:material-code-braces: DeleteDatabaseRequestRequestTypeDef](./type_defs.md#deletedatabaserequestrequesttypedef) 

### delete\_dev\_endpoint

Deletes a specified development endpoint.

Type annotations and code completion for `#!python session.client("glue").delete_dev_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_dev_endpoint method definition

await def delete_dev_endpoint(
    self,
    *,
    EndpointName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_dev_endpoint method usage example with argument unpacking

kwargs: DeleteDevEndpointRequestRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.delete_dev_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteDevEndpointRequestRequestTypeDef](./type_defs.md#deletedevendpointrequestrequesttypedef) 

### delete\_integration

Deletes the specified Zero-ETL integration.

Type annotations and code completion for `#!python session.client("glue").delete_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_integration method definition

await def delete_integration(
    self,
    *,
    IntegrationIdentifier: str,
) -> DeleteIntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIntegrationResponseTypeDef](./type_defs.md#deleteintegrationresponsetypedef) 


```python
# delete_integration method usage example with argument unpacking

kwargs: DeleteIntegrationRequestRequestTypeDef = {  # (1)
    "IntegrationIdentifier": ...,
}

parent.delete_integration(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationRequestRequestTypeDef](./type_defs.md#deleteintegrationrequestrequesttypedef) 

### delete\_integration\_table\_properties

Deletes the table properties that have been created for the tables that need to
be replicated.

Type annotations and code completion for `#!python session.client("glue").delete_integration_table_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_integration_table_properties method definition

await def delete_integration_table_properties(
    self,
    *,
    ResourceArn: str,
    TableName: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_integration_table_properties method usage example with argument unpacking

kwargs: DeleteIntegrationTablePropertiesRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TableName": ...,
}

parent.delete_integration_table_properties(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationTablePropertiesRequestRequestTypeDef](./type_defs.md#deleteintegrationtablepropertiesrequestrequesttypedef) 

### delete\_job

Deletes a specified job definition.

Type annotations and code completion for `#!python session.client("glue").delete_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_job method definition

await def delete_job(
    self,
    *,
    JobName: str,
) -> DeleteJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteJobResponseTypeDef](./type_defs.md#deletejobresponsetypedef) 


```python
# delete_job method usage example with argument unpacking

kwargs: DeleteJobRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.delete_job(**kwargs)
```

1. See [:material-code-braces: DeleteJobRequestRequestTypeDef](./type_defs.md#deletejobrequestrequesttypedef) 

### delete\_ml\_transform

Deletes an Glue machine learning transform.

Type annotations and code completion for `#!python session.client("glue").delete_ml_transform` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_ml_transform method definition

await def delete_ml_transform(
    self,
    *,
    TransformId: str,
) -> DeleteMLTransformResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMLTransformResponseTypeDef](./type_defs.md#deletemltransformresponsetypedef) 


```python
# delete_ml_transform method usage example with argument unpacking

kwargs: DeleteMLTransformRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
}

parent.delete_ml_transform(**kwargs)
```

1. See [:material-code-braces: DeleteMLTransformRequestRequestTypeDef](./type_defs.md#deletemltransformrequestrequesttypedef) 

### delete\_partition

Deletes a specified partition.

Type annotations and code completion for `#!python session.client("glue").delete_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_partition method definition

await def delete_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_partition method usage example with argument unpacking

kwargs: DeletePartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValues": ...,
}

parent.delete_partition(**kwargs)
```

1. See [:material-code-braces: DeletePartitionRequestRequestTypeDef](./type_defs.md#deletepartitionrequestrequesttypedef) 

### delete\_partition\_index

Deletes a specified partition index from an existing table.

Type annotations and code completion for `#!python session.client("glue").delete_partition_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_partition_index method definition

await def delete_partition_index(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    IndexName: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_partition_index method usage example with argument unpacking

kwargs: DeletePartitionIndexRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "IndexName": ...,
}

parent.delete_partition_index(**kwargs)
```

1. See [:material-code-braces: DeletePartitionIndexRequestRequestTypeDef](./type_defs.md#deletepartitionindexrequestrequesttypedef) 

### delete\_registry

Delete the entire registry including schema and all of its versions.

Type annotations and code completion for `#!python session.client("glue").delete_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_registry method definition

await def delete_registry(
    self,
    *,
    RegistryId: RegistryIdTypeDef,  # (1)
) -> DeleteRegistryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: DeleteRegistryResponseTypeDef](./type_defs.md#deleteregistryresponsetypedef) 


```python
# delete_registry method usage example with argument unpacking

kwargs: DeleteRegistryInputRequestTypeDef = {  # (1)
    "RegistryId": ...,
}

parent.delete_registry(**kwargs)
```

1. See [:material-code-braces: DeleteRegistryInputRequestTypeDef](./type_defs.md#deleteregistryinputrequesttypedef) 

### delete\_resource\_policy

Deletes a specified policy.

Type annotations and code completion for `#!python session.client("glue").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    PolicyHashCondition: str = ...,
    ResourceArn: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "PolicyHashCondition": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_schema

Deletes the entire schema set, including the schema set and all of its versions.

Type annotations and code completion for `#!python session.client("glue").delete_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_schema method definition

await def delete_schema(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
) -> DeleteSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: DeleteSchemaResponseTypeDef](./type_defs.md#deleteschemaresponsetypedef) 


```python
# delete_schema method usage example with argument unpacking

kwargs: DeleteSchemaInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.delete_schema(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaInputRequestTypeDef](./type_defs.md#deleteschemainputrequesttypedef) 

### delete\_schema\_versions

Remove versions from the specified schema.

Type annotations and code completion for `#!python session.client("glue").delete_schema_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_schema_versions method definition

await def delete_schema_versions(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    Versions: str,
) -> DeleteSchemaVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: DeleteSchemaVersionsResponseTypeDef](./type_defs.md#deleteschemaversionsresponsetypedef) 


```python
# delete_schema_versions method usage example with argument unpacking

kwargs: DeleteSchemaVersionsInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
    "Versions": ...,
}

parent.delete_schema_versions(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaVersionsInputRequestTypeDef](./type_defs.md#deleteschemaversionsinputrequesttypedef) 

### delete\_security\_configuration

Deletes a specified security configuration.

Type annotations and code completion for `#!python session.client("glue").delete_security_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_security_configuration method definition

await def delete_security_configuration(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_security_configuration method usage example with argument unpacking

kwargs: DeleteSecurityConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_security_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteSecurityConfigurationRequestRequestTypeDef](./type_defs.md#deletesecurityconfigurationrequestrequesttypedef) 

### delete\_session

Deletes the session.

Type annotations and code completion for `#!python session.client("glue").delete_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_session method definition

await def delete_session(
    self,
    *,
    Id: str,
    RequestOrigin: str = ...,
) -> DeleteSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef) 


```python
# delete_session method usage example with argument unpacking

kwargs: DeleteSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_session(**kwargs)
```

1. See [:material-code-braces: DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef) 

### delete\_table

Removes a table definition from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").delete_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_table method definition

await def delete_table(
    self,
    *,
    DatabaseName: str,
    Name: str,
    CatalogId: str = ...,
    TransactionId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_table method usage example with argument unpacking

kwargs: DeleteTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "Name": ...,
}

parent.delete_table(**kwargs)
```

1. See [:material-code-braces: DeleteTableRequestRequestTypeDef](./type_defs.md#deletetablerequestrequesttypedef) 

### delete\_table\_optimizer

Deletes an optimizer and all associated metadata for a table.

Type annotations and code completion for `#!python session.client("glue").delete_table_optimizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_table_optimizer method definition

await def delete_table_optimizer(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 


```python
# delete_table_optimizer method usage example with argument unpacking

kwargs: DeleteTableOptimizerRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Type": ...,
}

parent.delete_table_optimizer(**kwargs)
```

1. See [:material-code-braces: DeleteTableOptimizerRequestRequestTypeDef](./type_defs.md#deletetableoptimizerrequestrequesttypedef) 

### delete\_table\_version

Deletes a specified version of a table.

Type annotations and code completion for `#!python session.client("glue").delete_table_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_table_version method definition

await def delete_table_version(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    VersionId: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_table_version method usage example with argument unpacking

kwargs: DeleteTableVersionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "VersionId": ...,
}

parent.delete_table_version(**kwargs)
```

1. See [:material-code-braces: DeleteTableVersionRequestRequestTypeDef](./type_defs.md#deletetableversionrequestrequesttypedef) 

### delete\_trigger

Deletes a specified trigger.

Type annotations and code completion for `#!python session.client("glue").delete_trigger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_trigger method definition

await def delete_trigger(
    self,
    *,
    Name: str,
) -> DeleteTriggerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTriggerResponseTypeDef](./type_defs.md#deletetriggerresponsetypedef) 


```python
# delete_trigger method usage example with argument unpacking

kwargs: DeleteTriggerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_trigger(**kwargs)
```

1. See [:material-code-braces: DeleteTriggerRequestRequestTypeDef](./type_defs.md#deletetriggerrequestrequesttypedef) 

### delete\_usage\_profile

Deletes the Glue specified usage profile.

Type annotations and code completion for `#!python session.client("glue").delete_usage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_usage_profile method definition

await def delete_usage_profile(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# delete_usage_profile method usage example with argument unpacking

kwargs: DeleteUsageProfileRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_usage_profile(**kwargs)
```

1. See [:material-code-braces: DeleteUsageProfileRequestRequestTypeDef](./type_defs.md#deleteusageprofilerequestrequesttypedef) 

### delete\_user\_defined\_function

Deletes an existing function definition from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").delete_user_defined_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_user_defined_function method definition

await def delete_user_defined_function(
    self,
    *,
    DatabaseName: str,
    FunctionName: str,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# delete_user_defined_function method usage example with argument unpacking

kwargs: DeleteUserDefinedFunctionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "FunctionName": ...,
}

parent.delete_user_defined_function(**kwargs)
```

1. See [:material-code-braces: DeleteUserDefinedFunctionRequestRequestTypeDef](./type_defs.md#deleteuserdefinedfunctionrequestrequesttypedef) 

### delete\_workflow

Deletes a workflow.

Type annotations and code completion for `#!python session.client("glue").delete_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# delete_workflow method definition

await def delete_workflow(
    self,
    *,
    Name: str,
) -> DeleteWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkflowResponseTypeDef](./type_defs.md#deleteworkflowresponsetypedef) 


```python
# delete_workflow method usage example with argument unpacking

kwargs: DeleteWorkflowRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef) 

### describe\_connection\_type

The <code>DescribeConnectionType</code> API provides full details of the
supported options for a given connection type in Glue.

Type annotations and code completion for `#!python session.client("glue").describe_connection_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# describe_connection_type method definition

await def describe_connection_type(
    self,
    *,
    ConnectionType: str,
) -> DescribeConnectionTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectionTypeResponseTypeDef](./type_defs.md#describeconnectiontyperesponsetypedef) 


```python
# describe_connection_type method usage example with argument unpacking

kwargs: DescribeConnectionTypeRequestRequestTypeDef = {  # (1)
    "ConnectionType": ...,
}

parent.describe_connection_type(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionTypeRequestRequestTypeDef](./type_defs.md#describeconnectiontyperequestrequesttypedef) 

### describe\_entity

Provides details regarding the entity used with the connection type, with a
description of the data model for each field in the selected entity.

Type annotations and code completion for `#!python session.client("glue").describe_entity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# describe_entity method definition

await def describe_entity(
    self,
    *,
    ConnectionName: str,
    EntityName: str,
    CatalogId: str = ...,
    NextToken: str = ...,
    DataStoreApiVersion: str = ...,
) -> DescribeEntityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef) 


```python
# describe_entity method usage example with argument unpacking

kwargs: DescribeEntityRequestRequestTypeDef = {  # (1)
    "ConnectionName": ...,
    "EntityName": ...,
}

parent.describe_entity(**kwargs)
```

1. See [:material-code-braces: DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef) 

### describe\_inbound\_integrations

Returns a list of inbound integrations for the specified integration.

Type annotations and code completion for `#!python session.client("glue").describe_inbound_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# describe_inbound_integrations method definition

await def describe_inbound_integrations(
    self,
    *,
    IntegrationArn: str = ...,
    Marker: str = ...,
    MaxRecords: int = ...,
    TargetArn: str = ...,
) -> DescribeInboundIntegrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInboundIntegrationsResponseTypeDef](./type_defs.md#describeinboundintegrationsresponsetypedef) 


```python
# describe_inbound_integrations method usage example with argument unpacking

kwargs: DescribeInboundIntegrationsRequestRequestTypeDef = {  # (1)
    "IntegrationArn": ...,
}

parent.describe_inbound_integrations(**kwargs)
```

1. See [:material-code-braces: DescribeInboundIntegrationsRequestRequestTypeDef](./type_defs.md#describeinboundintegrationsrequestrequesttypedef) 

### describe\_integrations

The API is used to retrieve a list of integrations.

Type annotations and code completion for `#!python session.client("glue").describe_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# describe_integrations method definition

await def describe_integrations(
    self,
    *,
    IntegrationIdentifier: str = ...,
    Marker: str = ...,
    MaxRecords: int = ...,
    Filters: Sequence[IntegrationFilterTypeDef] = ...,  # (1)
) -> DescribeIntegrationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: IntegrationFilterTypeDef](./type_defs.md#integrationfiltertypedef) 
2. See [:material-code-braces: DescribeIntegrationsResponseTypeDef](./type_defs.md#describeintegrationsresponsetypedef) 


```python
# describe_integrations method usage example with argument unpacking

kwargs: DescribeIntegrationsRequestRequestTypeDef = {  # (1)
    "IntegrationIdentifier": ...,
}

parent.describe_integrations(**kwargs)
```

1. See [:material-code-braces: DescribeIntegrationsRequestRequestTypeDef](./type_defs.md#describeintegrationsrequestrequesttypedef) 

### get\_blueprint

Retrieves the details of a blueprint.

Type annotations and code completion for `#!python session.client("glue").get_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_blueprint method definition

await def get_blueprint(
    self,
    *,
    Name: str,
    IncludeBlueprint: bool = ...,
    IncludeParameterSpec: bool = ...,
) -> GetBlueprintResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBlueprintResponseTypeDef](./type_defs.md#getblueprintresponsetypedef) 


```python
# get_blueprint method usage example with argument unpacking

kwargs: GetBlueprintRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_blueprint(**kwargs)
```

1. See [:material-code-braces: GetBlueprintRequestRequestTypeDef](./type_defs.md#getblueprintrequestrequesttypedef) 

### get\_blueprint\_run

Retrieves the details of a blueprint run.

Type annotations and code completion for `#!python session.client("glue").get_blueprint_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_blueprint_run method definition

await def get_blueprint_run(
    self,
    *,
    BlueprintName: str,
    RunId: str,
) -> GetBlueprintRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBlueprintRunResponseTypeDef](./type_defs.md#getblueprintrunresponsetypedef) 


```python
# get_blueprint_run method usage example with argument unpacking

kwargs: GetBlueprintRunRequestRequestTypeDef = {  # (1)
    "BlueprintName": ...,
    "RunId": ...,
}

parent.get_blueprint_run(**kwargs)
```

1. See [:material-code-braces: GetBlueprintRunRequestRequestTypeDef](./type_defs.md#getblueprintrunrequestrequesttypedef) 

### get\_blueprint\_runs

Retrieves the details of blueprint runs for a specified blueprint.

Type annotations and code completion for `#!python session.client("glue").get_blueprint_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_blueprint_runs method definition

await def get_blueprint_runs(
    self,
    *,
    BlueprintName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetBlueprintRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBlueprintRunsResponseTypeDef](./type_defs.md#getblueprintrunsresponsetypedef) 


```python
# get_blueprint_runs method usage example with argument unpacking

kwargs: GetBlueprintRunsRequestRequestTypeDef = {  # (1)
    "BlueprintName": ...,
}

parent.get_blueprint_runs(**kwargs)
```

1. See [:material-code-braces: GetBlueprintRunsRequestRequestTypeDef](./type_defs.md#getblueprintrunsrequestrequesttypedef) 

### get\_catalog

The name of the Catalog to retrieve.

Type annotations and code completion for `#!python session.client("glue").get_catalog` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_catalog method definition

await def get_catalog(
    self,
    *,
    CatalogId: str,
) -> GetCatalogResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCatalogResponseTypeDef](./type_defs.md#getcatalogresponsetypedef) 


```python
# get_catalog method usage example with argument unpacking

kwargs: GetCatalogRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.get_catalog(**kwargs)
```

1. See [:material-code-braces: GetCatalogRequestRequestTypeDef](./type_defs.md#getcatalogrequestrequesttypedef) 

### get\_catalog\_import\_status

Retrieves the status of a migration operation.

Type annotations and code completion for `#!python session.client("glue").get_catalog_import_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_catalog_import_status method definition

await def get_catalog_import_status(
    self,
    *,
    CatalogId: str = ...,
) -> GetCatalogImportStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCatalogImportStatusResponseTypeDef](./type_defs.md#getcatalogimportstatusresponsetypedef) 


```python
# get_catalog_import_status method usage example with argument unpacking

kwargs: GetCatalogImportStatusRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.get_catalog_import_status(**kwargs)
```

1. See [:material-code-braces: GetCatalogImportStatusRequestRequestTypeDef](./type_defs.md#getcatalogimportstatusrequestrequesttypedef) 

### get\_catalogs

Retrieves all catalogs defined in a catalog in the Glue Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_catalogs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_catalogs method definition

await def get_catalogs(
    self,
    *,
    ParentCatalogId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    Recursive: bool = ...,
) -> GetCatalogsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCatalogsResponseTypeDef](./type_defs.md#getcatalogsresponsetypedef) 


```python
# get_catalogs method usage example with argument unpacking

kwargs: GetCatalogsRequestRequestTypeDef = {  # (1)
    "ParentCatalogId": ...,
}

parent.get_catalogs(**kwargs)
```

1. See [:material-code-braces: GetCatalogsRequestRequestTypeDef](./type_defs.md#getcatalogsrequestrequesttypedef) 

### get\_classifier

Retrieve a classifier by name.

Type annotations and code completion for `#!python session.client("glue").get_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_classifier method definition

await def get_classifier(
    self,
    *,
    Name: str,
) -> GetClassifierResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClassifierResponseTypeDef](./type_defs.md#getclassifierresponsetypedef) 


```python
# get_classifier method usage example with argument unpacking

kwargs: GetClassifierRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_classifier(**kwargs)
```

1. See [:material-code-braces: GetClassifierRequestRequestTypeDef](./type_defs.md#getclassifierrequestrequesttypedef) 

### get\_classifiers

Lists all classifier objects in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_classifiers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_classifiers method definition

await def get_classifiers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetClassifiersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetClassifiersResponseTypeDef](./type_defs.md#getclassifiersresponsetypedef) 


```python
# get_classifiers method usage example with argument unpacking

kwargs: GetClassifiersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_classifiers(**kwargs)
```

1. See [:material-code-braces: GetClassifiersRequestRequestTypeDef](./type_defs.md#getclassifiersrequestrequesttypedef) 

### get\_column\_statistics\_for\_partition

Retrieves partition statistics of columns.

Type annotations and code completion for `#!python session.client("glue").get_column_statistics_for_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_column_statistics_for_partition method definition

await def get_column_statistics_for_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnNames: Sequence[str],
    CatalogId: str = ...,
) -> GetColumnStatisticsForPartitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetColumnStatisticsForPartitionResponseTypeDef](./type_defs.md#getcolumnstatisticsforpartitionresponsetypedef) 


```python
# get_column_statistics_for_partition method usage example with argument unpacking

kwargs: GetColumnStatisticsForPartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValues": ...,
    "ColumnNames": ...,
}

parent.get_column_statistics_for_partition(**kwargs)
```

1. See [:material-code-braces: GetColumnStatisticsForPartitionRequestRequestTypeDef](./type_defs.md#getcolumnstatisticsforpartitionrequestrequesttypedef) 

### get\_column\_statistics\_for\_table

Retrieves table statistics of columns.

Type annotations and code completion for `#!python session.client("glue").get_column_statistics_for_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_column_statistics_for_table method definition

await def get_column_statistics_for_table(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    ColumnNames: Sequence[str],
    CatalogId: str = ...,
) -> GetColumnStatisticsForTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetColumnStatisticsForTableResponseTypeDef](./type_defs.md#getcolumnstatisticsfortableresponsetypedef) 


```python
# get_column_statistics_for_table method usage example with argument unpacking

kwargs: GetColumnStatisticsForTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "ColumnNames": ...,
}

parent.get_column_statistics_for_table(**kwargs)
```

1. See [:material-code-braces: GetColumnStatisticsForTableRequestRequestTypeDef](./type_defs.md#getcolumnstatisticsfortablerequestrequesttypedef) 

### get\_column\_statistics\_task\_run

Get the associated metadata/information for a task run, given a task run ID.

Type annotations and code completion for `#!python session.client("glue").get_column_statistics_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_column_statistics_task_run method definition

await def get_column_statistics_task_run(
    self,
    *,
    ColumnStatisticsTaskRunId: str,
) -> GetColumnStatisticsTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetColumnStatisticsTaskRunResponseTypeDef](./type_defs.md#getcolumnstatisticstaskrunresponsetypedef) 


```python
# get_column_statistics_task_run method usage example with argument unpacking

kwargs: GetColumnStatisticsTaskRunRequestRequestTypeDef = {  # (1)
    "ColumnStatisticsTaskRunId": ...,
}

parent.get_column_statistics_task_run(**kwargs)
```

1. See [:material-code-braces: GetColumnStatisticsTaskRunRequestRequestTypeDef](./type_defs.md#getcolumnstatisticstaskrunrequestrequesttypedef) 

### get\_column\_statistics\_task\_runs

Retrieves information about all runs associated with the specified table.

Type annotations and code completion for `#!python session.client("glue").get_column_statistics_task_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_column_statistics_task_runs method definition

await def get_column_statistics_task_runs(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetColumnStatisticsTaskRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetColumnStatisticsTaskRunsResponseTypeDef](./type_defs.md#getcolumnstatisticstaskrunsresponsetypedef) 


```python
# get_column_statistics_task_runs method usage example with argument unpacking

kwargs: GetColumnStatisticsTaskRunsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_column_statistics_task_runs(**kwargs)
```

1. See [:material-code-braces: GetColumnStatisticsTaskRunsRequestRequestTypeDef](./type_defs.md#getcolumnstatisticstaskrunsrequestrequesttypedef) 

### get\_column\_statistics\_task\_settings

Gets settings for a column statistics task.

Type annotations and code completion for `#!python session.client("glue").get_column_statistics_task_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_column_statistics_task_settings method definition

await def get_column_statistics_task_settings(
    self,
    *,
    DatabaseName: str,
    TableName: str,
) -> GetColumnStatisticsTaskSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetColumnStatisticsTaskSettingsResponseTypeDef](./type_defs.md#getcolumnstatisticstasksettingsresponsetypedef) 


```python
# get_column_statistics_task_settings method usage example with argument unpacking

kwargs: GetColumnStatisticsTaskSettingsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_column_statistics_task_settings(**kwargs)
```

1. See [:material-code-braces: GetColumnStatisticsTaskSettingsRequestRequestTypeDef](./type_defs.md#getcolumnstatisticstasksettingsrequestrequesttypedef) 

### get\_connection

Retrieves a connection definition from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_connection method definition

await def get_connection(
    self,
    *,
    Name: str,
    CatalogId: str = ...,
    HidePassword: bool = ...,
    ApplyOverrideForComputeEnvironment: ComputeEnvironmentType = ...,  # (1)
) -> GetConnectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ComputeEnvironmentType](./literals.md#computeenvironmenttype) 
2. See [:material-code-braces: GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef) 


```python
# get_connection method usage example with argument unpacking

kwargs: GetConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_connection(**kwargs)
```

1. See [:material-code-braces: GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef) 

### get\_connections

Retrieves a list of connection definitions from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_connections method definition

await def get_connections(
    self,
    *,
    CatalogId: str = ...,
    Filter: GetConnectionsFilterTypeDef = ...,  # (1)
    HidePassword: bool = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetConnectionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
2. See [:material-code-braces: GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef) 


```python
# get_connections method usage example with argument unpacking

kwargs: GetConnectionsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.get_connections(**kwargs)
```

1. See [:material-code-braces: GetConnectionsRequestRequestTypeDef](./type_defs.md#getconnectionsrequestrequesttypedef) 

### get\_crawler

Retrieves metadata for a specified crawler.

Type annotations and code completion for `#!python session.client("glue").get_crawler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_crawler method definition

await def get_crawler(
    self,
    *,
    Name: str,
) -> GetCrawlerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCrawlerResponseTypeDef](./type_defs.md#getcrawlerresponsetypedef) 


```python
# get_crawler method usage example with argument unpacking

kwargs: GetCrawlerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_crawler(**kwargs)
```

1. See [:material-code-braces: GetCrawlerRequestRequestTypeDef](./type_defs.md#getcrawlerrequestrequesttypedef) 

### get\_crawler\_metrics

Retrieves metrics about specified crawlers.

Type annotations and code completion for `#!python session.client("glue").get_crawler_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_crawler_metrics method definition

await def get_crawler_metrics(
    self,
    *,
    CrawlerNameList: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetCrawlerMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCrawlerMetricsResponseTypeDef](./type_defs.md#getcrawlermetricsresponsetypedef) 


```python
# get_crawler_metrics method usage example with argument unpacking

kwargs: GetCrawlerMetricsRequestRequestTypeDef = {  # (1)
    "CrawlerNameList": ...,
}

parent.get_crawler_metrics(**kwargs)
```

1. See [:material-code-braces: GetCrawlerMetricsRequestRequestTypeDef](./type_defs.md#getcrawlermetricsrequestrequesttypedef) 

### get\_crawlers

Retrieves metadata for all crawlers defined in the customer account.

Type annotations and code completion for `#!python session.client("glue").get_crawlers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_crawlers method definition

await def get_crawlers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetCrawlersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCrawlersResponseTypeDef](./type_defs.md#getcrawlersresponsetypedef) 


```python
# get_crawlers method usage example with argument unpacking

kwargs: GetCrawlersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_crawlers(**kwargs)
```

1. See [:material-code-braces: GetCrawlersRequestRequestTypeDef](./type_defs.md#getcrawlersrequestrequesttypedef) 

### get\_custom\_entity\_type

Retrieves the details of a custom pattern by specifying its name.

Type annotations and code completion for `#!python session.client("glue").get_custom_entity_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_custom_entity_type method definition

await def get_custom_entity_type(
    self,
    *,
    Name: str,
) -> GetCustomEntityTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCustomEntityTypeResponseTypeDef](./type_defs.md#getcustomentitytyperesponsetypedef) 


```python
# get_custom_entity_type method usage example with argument unpacking

kwargs: GetCustomEntityTypeRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_custom_entity_type(**kwargs)
```

1. See [:material-code-braces: GetCustomEntityTypeRequestRequestTypeDef](./type_defs.md#getcustomentitytyperequestrequesttypedef) 

### get\_data\_catalog\_encryption\_settings

Retrieves the security configuration for a specified catalog.

Type annotations and code completion for `#!python session.client("glue").get_data_catalog_encryption_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_catalog_encryption_settings method definition

await def get_data_catalog_encryption_settings(
    self,
    *,
    CatalogId: str = ...,
) -> GetDataCatalogEncryptionSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataCatalogEncryptionSettingsResponseTypeDef](./type_defs.md#getdatacatalogencryptionsettingsresponsetypedef) 


```python
# get_data_catalog_encryption_settings method usage example with argument unpacking

kwargs: GetDataCatalogEncryptionSettingsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.get_data_catalog_encryption_settings(**kwargs)
```

1. See [:material-code-braces: GetDataCatalogEncryptionSettingsRequestRequestTypeDef](./type_defs.md#getdatacatalogencryptionsettingsrequestrequesttypedef) 

### get\_data\_quality\_model

Retrieve the training status of the model along with more information
(CompletedOn, StartedOn, FailureReason).

Type annotations and code completion for `#!python session.client("glue").get_data_quality_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_quality_model method definition

await def get_data_quality_model(
    self,
    *,
    ProfileId: str,
    StatisticId: str = ...,
) -> GetDataQualityModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityModelResponseTypeDef](./type_defs.md#getdataqualitymodelresponsetypedef) 


```python
# get_data_quality_model method usage example with argument unpacking

kwargs: GetDataQualityModelRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
}

parent.get_data_quality_model(**kwargs)
```

1. See [:material-code-braces: GetDataQualityModelRequestRequestTypeDef](./type_defs.md#getdataqualitymodelrequestrequesttypedef) 

### get\_data\_quality\_model\_result

Retrieve a statistic's predictions for a given Profile ID.

Type annotations and code completion for `#!python session.client("glue").get_data_quality_model_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_quality_model_result method definition

await def get_data_quality_model_result(
    self,
    *,
    StatisticId: str,
    ProfileId: str,
) -> GetDataQualityModelResultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityModelResultResponseTypeDef](./type_defs.md#getdataqualitymodelresultresponsetypedef) 


```python
# get_data_quality_model_result method usage example with argument unpacking

kwargs: GetDataQualityModelResultRequestRequestTypeDef = {  # (1)
    "StatisticId": ...,
    "ProfileId": ...,
}

parent.get_data_quality_model_result(**kwargs)
```

1. See [:material-code-braces: GetDataQualityModelResultRequestRequestTypeDef](./type_defs.md#getdataqualitymodelresultrequestrequesttypedef) 

### get\_data\_quality\_result

Retrieves the result of a data quality rule evaluation.

Type annotations and code completion for `#!python session.client("glue").get_data_quality_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_quality_result method definition

await def get_data_quality_result(
    self,
    *,
    ResultId: str,
) -> GetDataQualityResultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityResultResponseTypeDef](./type_defs.md#getdataqualityresultresponsetypedef) 


```python
# get_data_quality_result method usage example with argument unpacking

kwargs: GetDataQualityResultRequestRequestTypeDef = {  # (1)
    "ResultId": ...,
}

parent.get_data_quality_result(**kwargs)
```

1. See [:material-code-braces: GetDataQualityResultRequestRequestTypeDef](./type_defs.md#getdataqualityresultrequestrequesttypedef) 

### get\_data\_quality\_rule\_recommendation\_run

Gets the specified recommendation run that was used to generate rules.

Type annotations and code completion for `#!python session.client("glue").get_data_quality_rule_recommendation_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_quality_rule_recommendation_run method definition

await def get_data_quality_rule_recommendation_run(
    self,
    *,
    RunId: str,
) -> GetDataQualityRuleRecommendationRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityRuleRecommendationRunResponseTypeDef](./type_defs.md#getdataqualityrulerecommendationrunresponsetypedef) 


```python
# get_data_quality_rule_recommendation_run method usage example with argument unpacking

kwargs: GetDataQualityRuleRecommendationRunRequestRequestTypeDef = {  # (1)
    "RunId": ...,
}

parent.get_data_quality_rule_recommendation_run(**kwargs)
```

1. See [:material-code-braces: GetDataQualityRuleRecommendationRunRequestRequestTypeDef](./type_defs.md#getdataqualityrulerecommendationrunrequestrequesttypedef) 

### get\_data\_quality\_ruleset

Returns an existing ruleset by identifier or name.

Type annotations and code completion for `#!python session.client("glue").get_data_quality_ruleset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_quality_ruleset method definition

await def get_data_quality_ruleset(
    self,
    *,
    Name: str,
) -> GetDataQualityRulesetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityRulesetResponseTypeDef](./type_defs.md#getdataqualityrulesetresponsetypedef) 


```python
# get_data_quality_ruleset method usage example with argument unpacking

kwargs: GetDataQualityRulesetRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_data_quality_ruleset(**kwargs)
```

1. See [:material-code-braces: GetDataQualityRulesetRequestRequestTypeDef](./type_defs.md#getdataqualityrulesetrequestrequesttypedef) 

### get\_data\_quality\_ruleset\_evaluation\_run

Retrieves a specific run where a ruleset is evaluated against a data source.

Type annotations and code completion for `#!python session.client("glue").get_data_quality_ruleset_evaluation_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_data_quality_ruleset_evaluation_run method definition

await def get_data_quality_ruleset_evaluation_run(
    self,
    *,
    RunId: str,
) -> GetDataQualityRulesetEvaluationRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataQualityRulesetEvaluationRunResponseTypeDef](./type_defs.md#getdataqualityrulesetevaluationrunresponsetypedef) 


```python
# get_data_quality_ruleset_evaluation_run method usage example with argument unpacking

kwargs: GetDataQualityRulesetEvaluationRunRequestRequestTypeDef = {  # (1)
    "RunId": ...,
}

parent.get_data_quality_ruleset_evaluation_run(**kwargs)
```

1. See [:material-code-braces: GetDataQualityRulesetEvaluationRunRequestRequestTypeDef](./type_defs.md#getdataqualityrulesetevaluationrunrequestrequesttypedef) 

### get\_database

Retrieves the definition of a specified database.

Type annotations and code completion for `#!python session.client("glue").get_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_database method definition

await def get_database(
    self,
    *,
    Name: str,
    CatalogId: str = ...,
) -> GetDatabaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDatabaseResponseTypeDef](./type_defs.md#getdatabaseresponsetypedef) 


```python
# get_database method usage example with argument unpacking

kwargs: GetDatabaseRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_database(**kwargs)
```

1. See [:material-code-braces: GetDatabaseRequestRequestTypeDef](./type_defs.md#getdatabaserequestrequesttypedef) 

### get\_databases

Retrieves all databases defined in a given Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_databases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_databases method definition

await def get_databases(
    self,
    *,
    CatalogId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (1)
    AttributesToGet: Sequence[DatabaseAttributesType] = ...,  # (2)
) -> GetDatabasesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-brackets: DatabaseAttributesType](./literals.md#databaseattributestype) 
3. See [:material-code-braces: GetDatabasesResponseTypeDef](./type_defs.md#getdatabasesresponsetypedef) 


```python
# get_databases method usage example with argument unpacking

kwargs: GetDatabasesRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.get_databases(**kwargs)
```

1. See [:material-code-braces: GetDatabasesRequestRequestTypeDef](./type_defs.md#getdatabasesrequestrequesttypedef) 

### get\_dataflow\_graph

Transforms a Python script into a directed acyclic graph (DAG).

Type annotations and code completion for `#!python session.client("glue").get_dataflow_graph` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_dataflow_graph method definition

await def get_dataflow_graph(
    self,
    *,
    PythonScript: str = ...,
) -> GetDataflowGraphResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataflowGraphResponseTypeDef](./type_defs.md#getdataflowgraphresponsetypedef) 


```python
# get_dataflow_graph method usage example with argument unpacking

kwargs: GetDataflowGraphRequestRequestTypeDef = {  # (1)
    "PythonScript": ...,
}

parent.get_dataflow_graph(**kwargs)
```

1. See [:material-code-braces: GetDataflowGraphRequestRequestTypeDef](./type_defs.md#getdataflowgraphrequestrequesttypedef) 

### get\_dev\_endpoint

Retrieves information about a specified development endpoint.

Type annotations and code completion for `#!python session.client("glue").get_dev_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_dev_endpoint method definition

await def get_dev_endpoint(
    self,
    *,
    EndpointName: str,
) -> GetDevEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDevEndpointResponseTypeDef](./type_defs.md#getdevendpointresponsetypedef) 


```python
# get_dev_endpoint method usage example with argument unpacking

kwargs: GetDevEndpointRequestRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.get_dev_endpoint(**kwargs)
```

1. See [:material-code-braces: GetDevEndpointRequestRequestTypeDef](./type_defs.md#getdevendpointrequestrequesttypedef) 

### get\_dev\_endpoints

Retrieves all the development endpoints in this Amazon Web Services account.

Type annotations and code completion for `#!python session.client("glue").get_dev_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_dev_endpoints method definition

await def get_dev_endpoints(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetDevEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDevEndpointsResponseTypeDef](./type_defs.md#getdevendpointsresponsetypedef) 


```python
# get_dev_endpoints method usage example with argument unpacking

kwargs: GetDevEndpointsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_dev_endpoints(**kwargs)
```

1. See [:material-code-braces: GetDevEndpointsRequestRequestTypeDef](./type_defs.md#getdevendpointsrequestrequesttypedef) 

### get\_entity\_records

This API is used to query preview data from a given connection type or from a
native Amazon S3 based Glue Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_entity_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_entity_records method definition

await def get_entity_records(
    self,
    *,
    EntityName: str,
    Limit: int,
    ConnectionName: str = ...,
    CatalogId: str = ...,
    NextToken: str = ...,
    DataStoreApiVersion: str = ...,
    ConnectionOptions: Mapping[str, str] = ...,
    FilterPredicate: str = ...,
    OrderBy: str = ...,
    SelectedFields: Sequence[str] = ...,
) -> GetEntityRecordsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEntityRecordsResponseTypeDef](./type_defs.md#getentityrecordsresponsetypedef) 


```python
# get_entity_records method usage example with argument unpacking

kwargs: GetEntityRecordsRequestRequestTypeDef = {  # (1)
    "EntityName": ...,
    "Limit": ...,
}

parent.get_entity_records(**kwargs)
```

1. See [:material-code-braces: GetEntityRecordsRequestRequestTypeDef](./type_defs.md#getentityrecordsrequestrequesttypedef) 

### get\_integration\_resource\_property

This API is used for fetching the <code>ResourceProperty</code> of the Glue
connection (for the source) or Glue database ARN (for the target).

Type annotations and code completion for `#!python session.client("glue").get_integration_resource_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_integration_resource_property method definition

await def get_integration_resource_property(
    self,
    *,
    ResourceArn: str,
) -> GetIntegrationResourcePropertyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationResourcePropertyResponseTypeDef](./type_defs.md#getintegrationresourcepropertyresponsetypedef) 


```python
# get_integration_resource_property method usage example with argument unpacking

kwargs: GetIntegrationResourcePropertyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_integration_resource_property(**kwargs)
```

1. See [:material-code-braces: GetIntegrationResourcePropertyRequestRequestTypeDef](./type_defs.md#getintegrationresourcepropertyrequestrequesttypedef) 

### get\_integration\_table\_properties

This API is used to retrieve optional override properties for the tables that
need to be replicated.

Type annotations and code completion for `#!python session.client("glue").get_integration_table_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_integration_table_properties method definition

await def get_integration_table_properties(
    self,
    *,
    ResourceArn: str,
    TableName: str,
) -> GetIntegrationTablePropertiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationTablePropertiesResponseTypeDef](./type_defs.md#getintegrationtablepropertiesresponsetypedef) 


```python
# get_integration_table_properties method usage example with argument unpacking

kwargs: GetIntegrationTablePropertiesRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TableName": ...,
}

parent.get_integration_table_properties(**kwargs)
```

1. See [:material-code-braces: GetIntegrationTablePropertiesRequestRequestTypeDef](./type_defs.md#getintegrationtablepropertiesrequestrequesttypedef) 

### get\_job

Retrieves an existing job definition.

Type annotations and code completion for `#!python session.client("glue").get_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_job method definition

await def get_job(
    self,
    *,
    JobName: str,
) -> GetJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef) 


```python
# get_job method usage example with argument unpacking

kwargs: GetJobRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.get_job(**kwargs)
```

1. See [:material-code-braces: GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef) 

### get\_job\_bookmark

Returns information on a job bookmark entry.

Type annotations and code completion for `#!python session.client("glue").get_job_bookmark` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_job_bookmark method definition

await def get_job_bookmark(
    self,
    *,
    JobName: str,
    RunId: str = ...,
) -> GetJobBookmarkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobBookmarkResponseTypeDef](./type_defs.md#getjobbookmarkresponsetypedef) 


```python
# get_job_bookmark method usage example with argument unpacking

kwargs: GetJobBookmarkRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.get_job_bookmark(**kwargs)
```

1. See [:material-code-braces: GetJobBookmarkRequestRequestTypeDef](./type_defs.md#getjobbookmarkrequestrequesttypedef) 

### get\_job\_run

Retrieves the metadata for a given job run.

Type annotations and code completion for `#!python session.client("glue").get_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_job_run method definition

await def get_job_run(
    self,
    *,
    JobName: str,
    RunId: str,
    PredecessorsIncluded: bool = ...,
) -> GetJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobRunResponseTypeDef](./type_defs.md#getjobrunresponsetypedef) 


```python
# get_job_run method usage example with argument unpacking

kwargs: GetJobRunRequestRequestTypeDef = {  # (1)
    "JobName": ...,
    "RunId": ...,
}

parent.get_job_run(**kwargs)
```

1. See [:material-code-braces: GetJobRunRequestRequestTypeDef](./type_defs.md#getjobrunrequestrequesttypedef) 

### get\_job\_runs

Retrieves metadata for all runs of a given job definition.

Type annotations and code completion for `#!python session.client("glue").get_job_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_job_runs method definition

await def get_job_runs(
    self,
    *,
    JobName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetJobRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobRunsResponseTypeDef](./type_defs.md#getjobrunsresponsetypedef) 


```python
# get_job_runs method usage example with argument unpacking

kwargs: GetJobRunsRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.get_job_runs(**kwargs)
```

1. See [:material-code-braces: GetJobRunsRequestRequestTypeDef](./type_defs.md#getjobrunsrequestrequesttypedef) 

### get\_jobs

Retrieves all current job definitions.

Type annotations and code completion for `#!python session.client("glue").get_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_jobs method definition

await def get_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobsResponseTypeDef](./type_defs.md#getjobsresponsetypedef) 


```python
# get_jobs method usage example with argument unpacking

kwargs: GetJobsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_jobs(**kwargs)
```

1. See [:material-code-braces: GetJobsRequestRequestTypeDef](./type_defs.md#getjobsrequestrequesttypedef) 

### get\_ml\_task\_run

Gets details for a specific task run on a machine learning transform.

Type annotations and code completion for `#!python session.client("glue").get_ml_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_ml_task_run method definition

await def get_ml_task_run(
    self,
    *,
    TransformId: str,
    TaskRunId: str,
) -> GetMLTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMLTaskRunResponseTypeDef](./type_defs.md#getmltaskrunresponsetypedef) 


```python
# get_ml_task_run method usage example with argument unpacking

kwargs: GetMLTaskRunRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
    "TaskRunId": ...,
}

parent.get_ml_task_run(**kwargs)
```

1. See [:material-code-braces: GetMLTaskRunRequestRequestTypeDef](./type_defs.md#getmltaskrunrequestrequesttypedef) 

### get\_ml\_task\_runs

Gets a list of runs for a machine learning transform.

Type annotations and code completion for `#!python session.client("glue").get_ml_task_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_ml_task_runs method definition

await def get_ml_task_runs(
    self,
    *,
    TransformId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filter: TaskRunFilterCriteriaTypeDef = ...,  # (1)
    Sort: TaskRunSortCriteriaTypeDef = ...,  # (2)
) -> GetMLTaskRunsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TaskRunFilterCriteriaTypeDef](./type_defs.md#taskrunfiltercriteriatypedef) 
2. See [:material-code-braces: TaskRunSortCriteriaTypeDef](./type_defs.md#taskrunsortcriteriatypedef) 
3. See [:material-code-braces: GetMLTaskRunsResponseTypeDef](./type_defs.md#getmltaskrunsresponsetypedef) 


```python
# get_ml_task_runs method usage example with argument unpacking

kwargs: GetMLTaskRunsRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
}

parent.get_ml_task_runs(**kwargs)
```

1. See [:material-code-braces: GetMLTaskRunsRequestRequestTypeDef](./type_defs.md#getmltaskrunsrequestrequesttypedef) 

### get\_ml\_transform

Gets an Glue machine learning transform artifact and all its corresponding
metadata.

Type annotations and code completion for `#!python session.client("glue").get_ml_transform` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_ml_transform method definition

await def get_ml_transform(
    self,
    *,
    TransformId: str,
) -> GetMLTransformResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMLTransformResponseTypeDef](./type_defs.md#getmltransformresponsetypedef) 


```python
# get_ml_transform method usage example with argument unpacking

kwargs: GetMLTransformRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
}

parent.get_ml_transform(**kwargs)
```

1. See [:material-code-braces: GetMLTransformRequestRequestTypeDef](./type_defs.md#getmltransformrequestrequesttypedef) 

### get\_ml\_transforms

Gets a sortable, filterable list of existing Glue machine learning transforms.

Type annotations and code completion for `#!python session.client("glue").get_ml_transforms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_ml_transforms method definition

await def get_ml_transforms(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filter: TransformFilterCriteriaTypeDef = ...,  # (1)
    Sort: TransformSortCriteriaTypeDef = ...,  # (2)
) -> GetMLTransformsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TransformFilterCriteriaTypeDef](./type_defs.md#transformfiltercriteriatypedef) 
2. See [:material-code-braces: TransformSortCriteriaTypeDef](./type_defs.md#transformsortcriteriatypedef) 
3. See [:material-code-braces: GetMLTransformsResponseTypeDef](./type_defs.md#getmltransformsresponsetypedef) 


```python
# get_ml_transforms method usage example with argument unpacking

kwargs: GetMLTransformsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_ml_transforms(**kwargs)
```

1. See [:material-code-braces: GetMLTransformsRequestRequestTypeDef](./type_defs.md#getmltransformsrequestrequesttypedef) 

### get\_mapping

Creates mappings.

Type annotations and code completion for `#!python session.client("glue").get_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_mapping method definition

await def get_mapping(
    self,
    *,
    Source: CatalogEntryTypeDef,  # (1)
    Sinks: Sequence[CatalogEntryTypeDef] = ...,  # (2)
    Location: LocationTypeDef = ...,  # (3)
) -> GetMappingResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
2. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
3. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
4. See [:material-code-braces: GetMappingResponseTypeDef](./type_defs.md#getmappingresponsetypedef) 


```python
# get_mapping method usage example with argument unpacking

kwargs: GetMappingRequestRequestTypeDef = {  # (1)
    "Source": ...,
}

parent.get_mapping(**kwargs)
```

1. See [:material-code-braces: GetMappingRequestRequestTypeDef](./type_defs.md#getmappingrequestrequesttypedef) 

### get\_partition

Retrieves information about a specified partition.

Type annotations and code completion for `#!python session.client("glue").get_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_partition method definition

await def get_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    CatalogId: str = ...,
) -> GetPartitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPartitionResponseTypeDef](./type_defs.md#getpartitionresponsetypedef) 


```python
# get_partition method usage example with argument unpacking

kwargs: GetPartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValues": ...,
}

parent.get_partition(**kwargs)
```

1. See [:material-code-braces: GetPartitionRequestRequestTypeDef](./type_defs.md#getpartitionrequestrequesttypedef) 

### get\_partition\_indexes

Retrieves the partition indexes associated with a table.

Type annotations and code completion for `#!python session.client("glue").get_partition_indexes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_partition_indexes method definition

await def get_partition_indexes(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    NextToken: str = ...,
) -> GetPartitionIndexesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPartitionIndexesResponseTypeDef](./type_defs.md#getpartitionindexesresponsetypedef) 


```python
# get_partition_indexes method usage example with argument unpacking

kwargs: GetPartitionIndexesRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_partition_indexes(**kwargs)
```

1. See [:material-code-braces: GetPartitionIndexesRequestRequestTypeDef](./type_defs.md#getpartitionindexesrequestrequesttypedef) 

### get\_partitions

Retrieves information about the partitions in a table.

Type annotations and code completion for `#!python session.client("glue").get_partitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_partitions method definition

await def get_partitions(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    Expression: str = ...,
    NextToken: str = ...,
    Segment: SegmentTypeDef = ...,  # (1)
    MaxResults: int = ...,
    ExcludeColumnSchema: bool = ...,
    TransactionId: str = ...,
    QueryAsOfTime: TimestampTypeDef = ...,
) -> GetPartitionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: GetPartitionsResponseTypeDef](./type_defs.md#getpartitionsresponsetypedef) 


```python
# get_partitions method usage example with argument unpacking

kwargs: GetPartitionsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_partitions(**kwargs)
```

1. See [:material-code-braces: GetPartitionsRequestRequestTypeDef](./type_defs.md#getpartitionsrequestrequesttypedef) 

### get\_plan

Gets code to perform a specified mapping.

Type annotations and code completion for `#!python session.client("glue").get_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_plan method definition

await def get_plan(
    self,
    *,
    Mapping: Sequence[MappingEntryTypeDef],  # (1)
    Source: CatalogEntryTypeDef,  # (2)
    Sinks: Sequence[CatalogEntryTypeDef] = ...,  # (3)
    Location: LocationTypeDef = ...,  # (4)
    Language: LanguageType = ...,  # (5)
    AdditionalPlanOptionsMap: Mapping[str, str] = ...,
) -> GetPlanResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: MappingEntryTypeDef](./type_defs.md#mappingentrytypedef) 
2. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
3. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
4. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
5. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
6. See [:material-code-braces: GetPlanResponseTypeDef](./type_defs.md#getplanresponsetypedef) 


```python
# get_plan method usage example with argument unpacking

kwargs: GetPlanRequestRequestTypeDef = {  # (1)
    "Mapping": ...,
    "Source": ...,
}

parent.get_plan(**kwargs)
```

1. See [:material-code-braces: GetPlanRequestRequestTypeDef](./type_defs.md#getplanrequestrequesttypedef) 

### get\_registry

Describes the specified registry in detail.

Type annotations and code completion for `#!python session.client("glue").get_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_registry method definition

await def get_registry(
    self,
    *,
    RegistryId: RegistryIdTypeDef,  # (1)
) -> GetRegistryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: GetRegistryResponseTypeDef](./type_defs.md#getregistryresponsetypedef) 


```python
# get_registry method usage example with argument unpacking

kwargs: GetRegistryInputRequestTypeDef = {  # (1)
    "RegistryId": ...,
}

parent.get_registry(**kwargs)
```

1. See [:material-code-braces: GetRegistryInputRequestTypeDef](./type_defs.md#getregistryinputrequesttypedef) 

### get\_resource\_policies

Retrieves the resource policies set on individual resources by Resource Access
Manager during cross-account permission grants.

Type annotations and code completion for `#!python session.client("glue").get_resource_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_resource_policies method definition

await def get_resource_policies(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetResourcePoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


```python
# get_resource_policies method usage example with argument unpacking

kwargs: GetResourcePoliciesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_resource_policies(**kwargs)
```

1. See [:material-code-braces: GetResourcePoliciesRequestRequestTypeDef](./type_defs.md#getresourcepoliciesrequestrequesttypedef) 

### get\_resource\_policy

Retrieves a specified resource policy.

Type annotations and code completion for `#!python session.client("glue").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    ResourceArn: str = ...,
) -> GetResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef) 

### get\_schema

Describes the specified schema in detail.

Type annotations and code completion for `#!python session.client("glue").get_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_schema method definition

await def get_schema(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
) -> GetSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: GetSchemaResponseTypeDef](./type_defs.md#getschemaresponsetypedef) 


```python
# get_schema method usage example with argument unpacking

kwargs: GetSchemaInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.get_schema(**kwargs)
```

1. See [:material-code-braces: GetSchemaInputRequestTypeDef](./type_defs.md#getschemainputrequesttypedef) 

### get\_schema\_by\_definition

Retrieves a schema by the <code>SchemaDefinition</code>.

Type annotations and code completion for `#!python session.client("glue").get_schema_by_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_schema_by_definition method definition

await def get_schema_by_definition(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaDefinition: str,
) -> GetSchemaByDefinitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: GetSchemaByDefinitionResponseTypeDef](./type_defs.md#getschemabydefinitionresponsetypedef) 


```python
# get_schema_by_definition method usage example with argument unpacking

kwargs: GetSchemaByDefinitionInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
    "SchemaDefinition": ...,
}

parent.get_schema_by_definition(**kwargs)
```

1. See [:material-code-braces: GetSchemaByDefinitionInputRequestTypeDef](./type_defs.md#getschemabydefinitioninputrequesttypedef) 

### get\_schema\_version

Get the specified schema by its unique ID assigned when a version of the schema
is created or registered.

Type annotations and code completion for `#!python session.client("glue").get_schema_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_schema_version method definition

await def get_schema_version(
    self,
    *,
    SchemaId: SchemaIdTypeDef = ...,  # (1)
    SchemaVersionId: str = ...,
    SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,  # (2)
) -> GetSchemaVersionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: GetSchemaVersionResponseTypeDef](./type_defs.md#getschemaversionresponsetypedef) 


```python
# get_schema_version method usage example with argument unpacking

kwargs: GetSchemaVersionInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.get_schema_version(**kwargs)
```

1. See [:material-code-braces: GetSchemaVersionInputRequestTypeDef](./type_defs.md#getschemaversioninputrequesttypedef) 

### get\_schema\_versions\_diff

Fetches the schema version difference in the specified difference type between
two stored schema versions in the Schema Registry.

Type annotations and code completion for `#!python session.client("glue").get_schema_versions_diff` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_schema_versions_diff method definition

await def get_schema_versions_diff(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    FirstSchemaVersionNumber: SchemaVersionNumberTypeDef,  # (2)
    SecondSchemaVersionNumber: SchemaVersionNumberTypeDef,  # (2)
    SchemaDiffType: SchemaDiffTypeType,  # (4)
) -> GetSchemaVersionsDiffResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
4. See [:material-code-brackets: SchemaDiffTypeType](./literals.md#schemadifftypetype) 
5. See [:material-code-braces: GetSchemaVersionsDiffResponseTypeDef](./type_defs.md#getschemaversionsdiffresponsetypedef) 


```python
# get_schema_versions_diff method usage example with argument unpacking

kwargs: GetSchemaVersionsDiffInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
    "FirstSchemaVersionNumber": ...,
    "SecondSchemaVersionNumber": ...,
    "SchemaDiffType": ...,
}

parent.get_schema_versions_diff(**kwargs)
```

1. See [:material-code-braces: GetSchemaVersionsDiffInputRequestTypeDef](./type_defs.md#getschemaversionsdiffinputrequesttypedef) 

### get\_security\_configuration

Retrieves a specified security configuration.

Type annotations and code completion for `#!python session.client("glue").get_security_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_security_configuration method definition

await def get_security_configuration(
    self,
    *,
    Name: str,
) -> GetSecurityConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSecurityConfigurationResponseTypeDef](./type_defs.md#getsecurityconfigurationresponsetypedef) 


```python
# get_security_configuration method usage example with argument unpacking

kwargs: GetSecurityConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_security_configuration(**kwargs)
```

1. See [:material-code-braces: GetSecurityConfigurationRequestRequestTypeDef](./type_defs.md#getsecurityconfigurationrequestrequesttypedef) 

### get\_security\_configurations

Retrieves a list of all security configurations.

Type annotations and code completion for `#!python session.client("glue").get_security_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_security_configurations method definition

await def get_security_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetSecurityConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSecurityConfigurationsResponseTypeDef](./type_defs.md#getsecurityconfigurationsresponsetypedef) 


```python
# get_security_configurations method usage example with argument unpacking

kwargs: GetSecurityConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.get_security_configurations(**kwargs)
```

1. See [:material-code-braces: GetSecurityConfigurationsRequestRequestTypeDef](./type_defs.md#getsecurityconfigurationsrequestrequesttypedef) 

### get\_session

Retrieves the session.

Type annotations and code completion for `#!python session.client("glue").get_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_session method definition

await def get_session(
    self,
    *,
    Id: str,
    RequestOrigin: str = ...,
) -> GetSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef) 


```python
# get_session method usage example with argument unpacking

kwargs: GetSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_session(**kwargs)
```

1. See [:material-code-braces: GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef) 

### get\_statement

Retrieves the statement.

Type annotations and code completion for `#!python session.client("glue").get_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_statement method definition

await def get_statement(
    self,
    *,
    SessionId: str,
    Id: int,
    RequestOrigin: str = ...,
) -> GetStatementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStatementResponseTypeDef](./type_defs.md#getstatementresponsetypedef) 


```python
# get_statement method usage example with argument unpacking

kwargs: GetStatementRequestRequestTypeDef = {  # (1)
    "SessionId": ...,
    "Id": ...,
}

parent.get_statement(**kwargs)
```

1. See [:material-code-braces: GetStatementRequestRequestTypeDef](./type_defs.md#getstatementrequestrequesttypedef) 

### get\_table

Retrieves the <code>Table</code> definition in a Data Catalog for a specified
table.

Type annotations and code completion for `#!python session.client("glue").get_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_table method definition

await def get_table(
    self,
    *,
    DatabaseName: str,
    Name: str,
    CatalogId: str = ...,
    TransactionId: str = ...,
    QueryAsOfTime: TimestampTypeDef = ...,
    IncludeStatusDetails: bool = ...,
) -> GetTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableResponseTypeDef](./type_defs.md#gettableresponsetypedef) 


```python
# get_table method usage example with argument unpacking

kwargs: GetTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "Name": ...,
}

parent.get_table(**kwargs)
```

1. See [:material-code-braces: GetTableRequestRequestTypeDef](./type_defs.md#gettablerequestrequesttypedef) 

### get\_table\_optimizer

Returns the configuration of all optimizers associated with a specified table.

Type annotations and code completion for `#!python session.client("glue").get_table_optimizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_table_optimizer method definition

await def get_table_optimizer(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
) -> GetTableOptimizerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: GetTableOptimizerResponseTypeDef](./type_defs.md#gettableoptimizerresponsetypedef) 


```python
# get_table_optimizer method usage example with argument unpacking

kwargs: GetTableOptimizerRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Type": ...,
}

parent.get_table_optimizer(**kwargs)
```

1. See [:material-code-braces: GetTableOptimizerRequestRequestTypeDef](./type_defs.md#gettableoptimizerrequestrequesttypedef) 

### get\_table\_version

Retrieves a specified version of a table.

Type annotations and code completion for `#!python session.client("glue").get_table_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_table_version method definition

await def get_table_version(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    VersionId: str = ...,
) -> GetTableVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableVersionResponseTypeDef](./type_defs.md#gettableversionresponsetypedef) 


```python
# get_table_version method usage example with argument unpacking

kwargs: GetTableVersionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_table_version(**kwargs)
```

1. See [:material-code-braces: GetTableVersionRequestRequestTypeDef](./type_defs.md#gettableversionrequestrequesttypedef) 

### get\_table\_versions

Retrieves a list of strings that identify available versions of a specified
table.

Type annotations and code completion for `#!python session.client("glue").get_table_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_table_versions method definition

await def get_table_versions(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    CatalogId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetTableVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableVersionsResponseTypeDef](./type_defs.md#gettableversionsresponsetypedef) 


```python
# get_table_versions method usage example with argument unpacking

kwargs: GetTableVersionsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.get_table_versions(**kwargs)
```

1. See [:material-code-braces: GetTableVersionsRequestRequestTypeDef](./type_defs.md#gettableversionsrequestrequesttypedef) 

### get\_tables

Retrieves the definitions of some or all of the tables in a given
<code>Database</code>.

Type annotations and code completion for `#!python session.client("glue").get_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_tables method definition

await def get_tables(
    self,
    *,
    DatabaseName: str,
    CatalogId: str = ...,
    Expression: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    TransactionId: str = ...,
    QueryAsOfTime: TimestampTypeDef = ...,
    IncludeStatusDetails: bool = ...,
    AttributesToGet: Sequence[TableAttributesType] = ...,  # (1)
) -> GetTablesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TableAttributesType](./literals.md#tableattributestype) 
2. See [:material-code-braces: GetTablesResponseTypeDef](./type_defs.md#gettablesresponsetypedef) 


```python
# get_tables method usage example with argument unpacking

kwargs: GetTablesRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
}

parent.get_tables(**kwargs)
```

1. See [:material-code-braces: GetTablesRequestRequestTypeDef](./type_defs.md#gettablesrequestrequesttypedef) 

### get\_tags

Retrieves a list of tags associated with a resource.

Type annotations and code completion for `#!python session.client("glue").get_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_tags method definition

await def get_tags(
    self,
    *,
    ResourceArn: str,
) -> GetTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTagsResponseTypeDef](./type_defs.md#gettagsresponsetypedef) 


```python
# get_tags method usage example with argument unpacking

kwargs: GetTagsRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_tags(**kwargs)
```

1. See [:material-code-braces: GetTagsRequestRequestTypeDef](./type_defs.md#gettagsrequestrequesttypedef) 

### get\_trigger

Retrieves the definition of a trigger.

Type annotations and code completion for `#!python session.client("glue").get_trigger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_trigger method definition

await def get_trigger(
    self,
    *,
    Name: str,
) -> GetTriggerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTriggerResponseTypeDef](./type_defs.md#gettriggerresponsetypedef) 


```python
# get_trigger method usage example with argument unpacking

kwargs: GetTriggerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_trigger(**kwargs)
```

1. See [:material-code-braces: GetTriggerRequestRequestTypeDef](./type_defs.md#gettriggerrequestrequesttypedef) 

### get\_triggers

Gets all the triggers associated with a job.

Type annotations and code completion for `#!python session.client("glue").get_triggers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_triggers method definition

await def get_triggers(
    self,
    *,
    NextToken: str = ...,
    DependentJobName: str = ...,
    MaxResults: int = ...,
) -> GetTriggersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTriggersResponseTypeDef](./type_defs.md#gettriggersresponsetypedef) 


```python
# get_triggers method usage example with argument unpacking

kwargs: GetTriggersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.get_triggers(**kwargs)
```

1. See [:material-code-braces: GetTriggersRequestRequestTypeDef](./type_defs.md#gettriggersrequestrequesttypedef) 

### get\_unfiltered\_partition\_metadata

Retrieves partition metadata from the Data Catalog that contains unfiltered
metadata.

Type annotations and code completion for `#!python session.client("glue").get_unfiltered_partition_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_unfiltered_partition_metadata method definition

await def get_unfiltered_partition_metadata(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Region: str = ...,
    AuditContext: AuditContextTypeDef = ...,  # (2)
    QuerySessionContext: QuerySessionContextTypeDef = ...,  # (3)
) -> GetUnfilteredPartitionMetadataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
4. See [:material-code-braces: GetUnfilteredPartitionMetadataResponseTypeDef](./type_defs.md#getunfilteredpartitionmetadataresponsetypedef) 


```python
# get_unfiltered_partition_metadata method usage example with argument unpacking

kwargs: GetUnfilteredPartitionMetadataRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValues": ...,
    "SupportedPermissionTypes": ...,
}

parent.get_unfiltered_partition_metadata(**kwargs)
```

1. See [:material-code-braces: GetUnfilteredPartitionMetadataRequestRequestTypeDef](./type_defs.md#getunfilteredpartitionmetadatarequestrequesttypedef) 

### get\_unfiltered\_partitions\_metadata

Retrieves partition metadata from the Data Catalog that contains unfiltered
metadata.

Type annotations and code completion for `#!python session.client("glue").get_unfiltered_partitions_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_unfiltered_partitions_metadata method definition

await def get_unfiltered_partitions_metadata(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Region: str = ...,
    Expression: str = ...,
    AuditContext: AuditContextTypeDef = ...,  # (2)
    NextToken: str = ...,
    Segment: SegmentTypeDef = ...,  # (3)
    MaxResults: int = ...,
    QuerySessionContext: QuerySessionContextTypeDef = ...,  # (4)
) -> GetUnfilteredPartitionsMetadataResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
4. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
5. See [:material-code-braces: GetUnfilteredPartitionsMetadataResponseTypeDef](./type_defs.md#getunfilteredpartitionsmetadataresponsetypedef) 


```python
# get_unfiltered_partitions_metadata method usage example with argument unpacking

kwargs: GetUnfilteredPartitionsMetadataRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "SupportedPermissionTypes": ...,
}

parent.get_unfiltered_partitions_metadata(**kwargs)
```

1. See [:material-code-braces: GetUnfilteredPartitionsMetadataRequestRequestTypeDef](./type_defs.md#getunfilteredpartitionsmetadatarequestrequesttypedef) 

### get\_unfiltered\_table\_metadata

Allows a third-party analytical engine to retrieve unfiltered table metadata
from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_unfiltered_table_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_unfiltered_table_metadata method definition

await def get_unfiltered_table_metadata(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    Name: str,
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Region: str = ...,
    AuditContext: AuditContextTypeDef = ...,  # (2)
    ParentResourceArn: str = ...,
    RootResourceArn: str = ...,
    SupportedDialect: SupportedDialectTypeDef = ...,  # (3)
    Permissions: Sequence[PermissionType] = ...,  # (4)
    QuerySessionContext: QuerySessionContextTypeDef = ...,  # (5)
) -> GetUnfilteredTableMetadataResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: SupportedDialectTypeDef](./type_defs.md#supporteddialecttypedef) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
5. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
6. See [:material-code-braces: GetUnfilteredTableMetadataResponseTypeDef](./type_defs.md#getunfilteredtablemetadataresponsetypedef) 


```python
# get_unfiltered_table_metadata method usage example with argument unpacking

kwargs: GetUnfilteredTableMetadataRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "Name": ...,
    "SupportedPermissionTypes": ...,
}

parent.get_unfiltered_table_metadata(**kwargs)
```

1. See [:material-code-braces: GetUnfilteredTableMetadataRequestRequestTypeDef](./type_defs.md#getunfilteredtablemetadatarequestrequesttypedef) 

### get\_usage\_profile

Retrieves information about the specified Glue usage profile.

Type annotations and code completion for `#!python session.client("glue").get_usage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_usage_profile method definition

await def get_usage_profile(
    self,
    *,
    Name: str,
) -> GetUsageProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUsageProfileResponseTypeDef](./type_defs.md#getusageprofileresponsetypedef) 


```python
# get_usage_profile method usage example with argument unpacking

kwargs: GetUsageProfileRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_usage_profile(**kwargs)
```

1. See [:material-code-braces: GetUsageProfileRequestRequestTypeDef](./type_defs.md#getusageprofilerequestrequesttypedef) 

### get\_user\_defined\_function

Retrieves a specified function definition from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_user_defined_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_user_defined_function method definition

await def get_user_defined_function(
    self,
    *,
    DatabaseName: str,
    FunctionName: str,
    CatalogId: str = ...,
) -> GetUserDefinedFunctionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserDefinedFunctionResponseTypeDef](./type_defs.md#getuserdefinedfunctionresponsetypedef) 


```python
# get_user_defined_function method usage example with argument unpacking

kwargs: GetUserDefinedFunctionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "FunctionName": ...,
}

parent.get_user_defined_function(**kwargs)
```

1. See [:material-code-braces: GetUserDefinedFunctionRequestRequestTypeDef](./type_defs.md#getuserdefinedfunctionrequestrequesttypedef) 

### get\_user\_defined\_functions

Retrieves multiple function definitions from the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").get_user_defined_functions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_user_defined_functions method definition

await def get_user_defined_functions(
    self,
    *,
    Pattern: str,
    CatalogId: str = ...,
    DatabaseName: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetUserDefinedFunctionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserDefinedFunctionsResponseTypeDef](./type_defs.md#getuserdefinedfunctionsresponsetypedef) 


```python
# get_user_defined_functions method usage example with argument unpacking

kwargs: GetUserDefinedFunctionsRequestRequestTypeDef = {  # (1)
    "Pattern": ...,
}

parent.get_user_defined_functions(**kwargs)
```

1. See [:material-code-braces: GetUserDefinedFunctionsRequestRequestTypeDef](./type_defs.md#getuserdefinedfunctionsrequestrequesttypedef) 

### get\_workflow

Retrieves resource metadata for a workflow.

Type annotations and code completion for `#!python session.client("glue").get_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_workflow method definition

await def get_workflow(
    self,
    *,
    Name: str,
    IncludeGraph: bool = ...,
) -> GetWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef) 


```python
# get_workflow method usage example with argument unpacking

kwargs: GetWorkflowRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_workflow(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef) 

### get\_workflow\_run

Retrieves the metadata for a given workflow run.

Type annotations and code completion for `#!python session.client("glue").get_workflow_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_workflow_run method definition

await def get_workflow_run(
    self,
    *,
    Name: str,
    RunId: str,
    IncludeGraph: bool = ...,
) -> GetWorkflowRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowRunResponseTypeDef](./type_defs.md#getworkflowrunresponsetypedef) 


```python
# get_workflow_run method usage example with argument unpacking

kwargs: GetWorkflowRunRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RunId": ...,
}

parent.get_workflow_run(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRunRequestRequestTypeDef](./type_defs.md#getworkflowrunrequestrequesttypedef) 

### get\_workflow\_run\_properties

Retrieves the workflow run properties which were set during the run.

Type annotations and code completion for `#!python session.client("glue").get_workflow_run_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_workflow_run_properties method definition

await def get_workflow_run_properties(
    self,
    *,
    Name: str,
    RunId: str,
) -> GetWorkflowRunPropertiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowRunPropertiesResponseTypeDef](./type_defs.md#getworkflowrunpropertiesresponsetypedef) 


```python
# get_workflow_run_properties method usage example with argument unpacking

kwargs: GetWorkflowRunPropertiesRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RunId": ...,
}

parent.get_workflow_run_properties(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRunPropertiesRequestRequestTypeDef](./type_defs.md#getworkflowrunpropertiesrequestrequesttypedef) 

### get\_workflow\_runs

Retrieves metadata for all runs of a given workflow.

Type annotations and code completion for `#!python session.client("glue").get_workflow_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# get_workflow_runs method definition

await def get_workflow_runs(
    self,
    *,
    Name: str,
    IncludeGraph: bool = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetWorkflowRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowRunsResponseTypeDef](./type_defs.md#getworkflowrunsresponsetypedef) 


```python
# get_workflow_runs method usage example with argument unpacking

kwargs: GetWorkflowRunsRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_workflow_runs(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRunsRequestRequestTypeDef](./type_defs.md#getworkflowrunsrequestrequesttypedef) 

### import\_catalog\_to\_glue

Imports an existing Amazon Athena Data Catalog to Glue.

Type annotations and code completion for `#!python session.client("glue").import_catalog_to_glue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# import_catalog_to_glue method definition

await def import_catalog_to_glue(
    self,
    *,
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# import_catalog_to_glue method usage example with argument unpacking

kwargs: ImportCatalogToGlueRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.import_catalog_to_glue(**kwargs)
```

1. See [:material-code-braces: ImportCatalogToGlueRequestRequestTypeDef](./type_defs.md#importcatalogtogluerequestrequesttypedef) 

### list\_blueprints

Lists all the blueprint names in an account.

Type annotations and code completion for `#!python session.client("glue").list_blueprints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_blueprints method definition

await def list_blueprints(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Tags: Mapping[str, str] = ...,
) -> ListBlueprintsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBlueprintsResponseTypeDef](./type_defs.md#listblueprintsresponsetypedef) 


```python
# list_blueprints method usage example with argument unpacking

kwargs: ListBlueprintsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_blueprints(**kwargs)
```

1. See [:material-code-braces: ListBlueprintsRequestRequestTypeDef](./type_defs.md#listblueprintsrequestrequesttypedef) 

### list\_column\_statistics\_task\_runs

List all task runs for a particular account.

Type annotations and code completion for `#!python session.client("glue").list_column_statistics_task_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_column_statistics_task_runs method definition

await def list_column_statistics_task_runs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListColumnStatisticsTaskRunsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListColumnStatisticsTaskRunsResponseTypeDef](./type_defs.md#listcolumnstatisticstaskrunsresponsetypedef) 


```python
# list_column_statistics_task_runs method usage example with argument unpacking

kwargs: ListColumnStatisticsTaskRunsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_column_statistics_task_runs(**kwargs)
```

1. See [:material-code-braces: ListColumnStatisticsTaskRunsRequestRequestTypeDef](./type_defs.md#listcolumnstatisticstaskrunsrequestrequesttypedef) 

### list\_connection\_types

The <code>ListConnectionTypes</code> API provides a discovery mechanism to
learn available connection types in Glue.

Type annotations and code completion for `#!python session.client("glue").list_connection_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_connection_types method definition

await def list_connection_types(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListConnectionTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConnectionTypesResponseTypeDef](./type_defs.md#listconnectiontypesresponsetypedef) 


```python
# list_connection_types method usage example with argument unpacking

kwargs: ListConnectionTypesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_connection_types(**kwargs)
```

1. See [:material-code-braces: ListConnectionTypesRequestRequestTypeDef](./type_defs.md#listconnectiontypesrequestrequesttypedef) 

### list\_crawlers

Retrieves the names of all crawler resources in this Amazon Web Services
account, or the resources with the specified tag.

Type annotations and code completion for `#!python session.client("glue").list_crawlers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_crawlers method definition

await def list_crawlers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> ListCrawlersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCrawlersResponseTypeDef](./type_defs.md#listcrawlersresponsetypedef) 


```python
# list_crawlers method usage example with argument unpacking

kwargs: ListCrawlersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_crawlers(**kwargs)
```

1. See [:material-code-braces: ListCrawlersRequestRequestTypeDef](./type_defs.md#listcrawlersrequestrequesttypedef) 

### list\_crawls

Returns all the crawls of a specified crawler.

Type annotations and code completion for `#!python session.client("glue").list_crawls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_crawls method definition

await def list_crawls(
    self,
    *,
    CrawlerName: str,
    MaxResults: int = ...,
    Filters: Sequence[CrawlsFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
) -> ListCrawlsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CrawlsFilterTypeDef](./type_defs.md#crawlsfiltertypedef) 
2. See [:material-code-braces: ListCrawlsResponseTypeDef](./type_defs.md#listcrawlsresponsetypedef) 


```python
# list_crawls method usage example with argument unpacking

kwargs: ListCrawlsRequestRequestTypeDef = {  # (1)
    "CrawlerName": ...,
}

parent.list_crawls(**kwargs)
```

1. See [:material-code-braces: ListCrawlsRequestRequestTypeDef](./type_defs.md#listcrawlsrequestrequesttypedef) 

### list\_custom\_entity\_types

Lists all the custom patterns that have been created.

Type annotations and code completion for `#!python session.client("glue").list_custom_entity_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_custom_entity_types method definition

await def list_custom_entity_types(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Tags: Mapping[str, str] = ...,
) -> ListCustomEntityTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomEntityTypesResponseTypeDef](./type_defs.md#listcustomentitytypesresponsetypedef) 


```python
# list_custom_entity_types method usage example with argument unpacking

kwargs: ListCustomEntityTypesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_custom_entity_types(**kwargs)
```

1. See [:material-code-braces: ListCustomEntityTypesRequestRequestTypeDef](./type_defs.md#listcustomentitytypesrequestrequesttypedef) 

### list\_data\_quality\_results

Returns all data quality execution results for your account.

Type annotations and code completion for `#!python session.client("glue").list_data_quality_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_data_quality_results method definition

await def list_data_quality_results(
    self,
    *,
    Filter: DataQualityResultFilterCriteriaTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataQualityResultsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataQualityResultFilterCriteriaTypeDef](./type_defs.md#dataqualityresultfiltercriteriatypedef) 
2. See [:material-code-braces: ListDataQualityResultsResponseTypeDef](./type_defs.md#listdataqualityresultsresponsetypedef) 


```python
# list_data_quality_results method usage example with argument unpacking

kwargs: ListDataQualityResultsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_data_quality_results(**kwargs)
```

1. See [:material-code-braces: ListDataQualityResultsRequestRequestTypeDef](./type_defs.md#listdataqualityresultsrequestrequesttypedef) 

### list\_data\_quality\_rule\_recommendation\_runs

Lists the recommendation runs meeting the filter criteria.

Type annotations and code completion for `#!python session.client("glue").list_data_quality_rule_recommendation_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_data_quality_rule_recommendation_runs method definition

await def list_data_quality_rule_recommendation_runs(
    self,
    *,
    Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataQualityRuleRecommendationRunFilterTypeDef](./type_defs.md#dataqualityrulerecommendationrunfiltertypedef) 
2. See [:material-code-braces: ListDataQualityRuleRecommendationRunsResponseTypeDef](./type_defs.md#listdataqualityrulerecommendationrunsresponsetypedef) 


```python
# list_data_quality_rule_recommendation_runs method usage example with argument unpacking

kwargs: ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_data_quality_rule_recommendation_runs(**kwargs)
```

1. See [:material-code-braces: ListDataQualityRuleRecommendationRunsRequestRequestTypeDef](./type_defs.md#listdataqualityrulerecommendationrunsrequestrequesttypedef) 

### list\_data\_quality\_ruleset\_evaluation\_runs

Lists all the runs meeting the filter criteria, where a ruleset is evaluated
against a data source.

Type annotations and code completion for `#!python session.client("glue").list_data_quality_ruleset_evaluation_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_data_quality_ruleset_evaluation_runs method definition

await def list_data_quality_ruleset_evaluation_runs(
    self,
    *,
    Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataQualityRulesetEvaluationRunFilterTypeDef](./type_defs.md#dataqualityrulesetevaluationrunfiltertypedef) 
2. See [:material-code-braces: ListDataQualityRulesetEvaluationRunsResponseTypeDef](./type_defs.md#listdataqualityrulesetevaluationrunsresponsetypedef) 


```python
# list_data_quality_ruleset_evaluation_runs method usage example with argument unpacking

kwargs: ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_data_quality_ruleset_evaluation_runs(**kwargs)
```

1. See [:material-code-braces: ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef](./type_defs.md#listdataqualityrulesetevaluationrunsrequestrequesttypedef) 

### list\_data\_quality\_rulesets

Returns a paginated list of rulesets for the specified list of Glue tables.

Type annotations and code completion for `#!python session.client("glue").list_data_quality_rulesets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_data_quality_rulesets method definition

await def list_data_quality_rulesets(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,  # (1)
    Tags: Mapping[str, str] = ...,
) -> ListDataQualityRulesetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataQualityRulesetFilterCriteriaTypeDef](./type_defs.md#dataqualityrulesetfiltercriteriatypedef) 
2. See [:material-code-braces: ListDataQualityRulesetsResponseTypeDef](./type_defs.md#listdataqualityrulesetsresponsetypedef) 


```python
# list_data_quality_rulesets method usage example with argument unpacking

kwargs: ListDataQualityRulesetsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_data_quality_rulesets(**kwargs)
```

1. See [:material-code-braces: ListDataQualityRulesetsRequestRequestTypeDef](./type_defs.md#listdataqualityrulesetsrequestrequesttypedef) 

### list\_data\_quality\_statistic\_annotations

Retrieve annotations for a data quality statistic.

Type annotations and code completion for `#!python session.client("glue").list_data_quality_statistic_annotations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_data_quality_statistic_annotations method definition

await def list_data_quality_statistic_annotations(
    self,
    *,
    StatisticId: str = ...,
    ProfileId: str = ...,
    TimestampFilter: TimestampFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDataQualityStatisticAnnotationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TimestampFilterTypeDef](./type_defs.md#timestampfiltertypedef) 
2. See [:material-code-braces: ListDataQualityStatisticAnnotationsResponseTypeDef](./type_defs.md#listdataqualitystatisticannotationsresponsetypedef) 


```python
# list_data_quality_statistic_annotations method usage example with argument unpacking

kwargs: ListDataQualityStatisticAnnotationsRequestRequestTypeDef = {  # (1)
    "StatisticId": ...,
}

parent.list_data_quality_statistic_annotations(**kwargs)
```

1. See [:material-code-braces: ListDataQualityStatisticAnnotationsRequestRequestTypeDef](./type_defs.md#listdataqualitystatisticannotationsrequestrequesttypedef) 

### list\_data\_quality\_statistics

Retrieves a list of data quality statistics.

Type annotations and code completion for `#!python session.client("glue").list_data_quality_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_data_quality_statistics method definition

await def list_data_quality_statistics(
    self,
    *,
    StatisticId: str = ...,
    ProfileId: str = ...,
    TimestampFilter: TimestampFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDataQualityStatisticsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TimestampFilterTypeDef](./type_defs.md#timestampfiltertypedef) 
2. See [:material-code-braces: ListDataQualityStatisticsResponseTypeDef](./type_defs.md#listdataqualitystatisticsresponsetypedef) 


```python
# list_data_quality_statistics method usage example with argument unpacking

kwargs: ListDataQualityStatisticsRequestRequestTypeDef = {  # (1)
    "StatisticId": ...,
}

parent.list_data_quality_statistics(**kwargs)
```

1. See [:material-code-braces: ListDataQualityStatisticsRequestRequestTypeDef](./type_defs.md#listdataqualitystatisticsrequestrequesttypedef) 

### list\_dev\_endpoints

Retrieves the names of all <code>DevEndpoint</code> resources in this Amazon
Web Services account, or the resources with the specified tag.

Type annotations and code completion for `#!python session.client("glue").list_dev_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_dev_endpoints method definition

await def list_dev_endpoints(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Tags: Mapping[str, str] = ...,
) -> ListDevEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDevEndpointsResponseTypeDef](./type_defs.md#listdevendpointsresponsetypedef) 


```python
# list_dev_endpoints method usage example with argument unpacking

kwargs: ListDevEndpointsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_dev_endpoints(**kwargs)
```

1. See [:material-code-braces: ListDevEndpointsRequestRequestTypeDef](./type_defs.md#listdevendpointsrequestrequesttypedef) 

### list\_entities

Returns the available entities supported by the connection type.

Type annotations and code completion for `#!python session.client("glue").list_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_entities method definition

await def list_entities(
    self,
    *,
    ConnectionName: str = ...,
    CatalogId: str = ...,
    ParentEntityName: str = ...,
    NextToken: str = ...,
    DataStoreApiVersion: str = ...,
) -> ListEntitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


```python
# list_entities method usage example with argument unpacking

kwargs: ListEntitiesRequestRequestTypeDef = {  # (1)
    "ConnectionName": ...,
}

parent.list_entities(**kwargs)
```

1. See [:material-code-braces: ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef) 

### list\_jobs

Retrieves the names of all job resources in this Amazon Web Services account,
or the resources with the specified tag.

Type annotations and code completion for `#!python session.client("glue").list_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_jobs method definition

await def list_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Tags: Mapping[str, str] = ...,
) -> ListJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# list_jobs method usage example with argument unpacking

kwargs: ListJobsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_jobs(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef) 

### list\_ml\_transforms

Retrieves a sortable, filterable list of existing Glue machine learning
transforms in this Amazon Web Services account, or the resources with the
specified tag.

Type annotations and code completion for `#!python session.client("glue").list_ml_transforms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_ml_transforms method definition

await def list_ml_transforms(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filter: TransformFilterCriteriaTypeDef = ...,  # (1)
    Sort: TransformSortCriteriaTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> ListMLTransformsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TransformFilterCriteriaTypeDef](./type_defs.md#transformfiltercriteriatypedef) 
2. See [:material-code-braces: TransformSortCriteriaTypeDef](./type_defs.md#transformsortcriteriatypedef) 
3. See [:material-code-braces: ListMLTransformsResponseTypeDef](./type_defs.md#listmltransformsresponsetypedef) 


```python
# list_ml_transforms method usage example with argument unpacking

kwargs: ListMLTransformsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_ml_transforms(**kwargs)
```

1. See [:material-code-braces: ListMLTransformsRequestRequestTypeDef](./type_defs.md#listmltransformsrequestrequesttypedef) 

### list\_registries

Returns a list of registries that you have created, with minimal registry
information.

Type annotations and code completion for `#!python session.client("glue").list_registries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_registries method definition

await def list_registries(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRegistriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


```python
# list_registries method usage example with argument unpacking

kwargs: ListRegistriesInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_registries(**kwargs)
```

1. See [:material-code-braces: ListRegistriesInputRequestTypeDef](./type_defs.md#listregistriesinputrequesttypedef) 

### list\_schema\_versions

Returns a list of schema versions that you have created, with minimal
information.

Type annotations and code completion for `#!python session.client("glue").list_schema_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_schema_versions method definition

await def list_schema_versions(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSchemaVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


```python
# list_schema_versions method usage example with argument unpacking

kwargs: ListSchemaVersionsInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.list_schema_versions(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsInputRequestTypeDef](./type_defs.md#listschemaversionsinputrequesttypedef) 

### list\_schemas

Returns a list of schemas with minimal details.

Type annotations and code completion for `#!python session.client("glue").list_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_schemas method definition

await def list_schemas(
    self,
    *,
    RegistryId: RegistryIdTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSchemasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# list_schemas method usage example with argument unpacking

kwargs: ListSchemasInputRequestTypeDef = {  # (1)
    "RegistryId": ...,
}

parent.list_schemas(**kwargs)
```

1. See [:material-code-braces: ListSchemasInputRequestTypeDef](./type_defs.md#listschemasinputrequesttypedef) 

### list\_sessions

Retrieve a list of sessions.

Type annotations and code completion for `#!python session.client("glue").list_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_sessions method definition

await def list_sessions(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Tags: Mapping[str, str] = ...,
    RequestOrigin: str = ...,
) -> ListSessionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 


```python
# list_sessions method usage example with argument unpacking

kwargs: ListSessionsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_sessions(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestRequestTypeDef](./type_defs.md#listsessionsrequestrequesttypedef) 

### list\_statements

Lists statements for the session.

Type annotations and code completion for `#!python session.client("glue").list_statements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_statements method definition

await def list_statements(
    self,
    *,
    SessionId: str,
    RequestOrigin: str = ...,
    NextToken: str = ...,
) -> ListStatementsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStatementsResponseTypeDef](./type_defs.md#liststatementsresponsetypedef) 


```python
# list_statements method usage example with argument unpacking

kwargs: ListStatementsRequestRequestTypeDef = {  # (1)
    "SessionId": ...,
}

parent.list_statements(**kwargs)
```

1. See [:material-code-braces: ListStatementsRequestRequestTypeDef](./type_defs.md#liststatementsrequestrequesttypedef) 

### list\_table\_optimizer\_runs

Lists the history of previous optimizer runs for a specific table.

Type annotations and code completion for `#!python session.client("glue").list_table_optimizer_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_table_optimizer_runs method definition

await def list_table_optimizer_runs(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTableOptimizerRunsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: ListTableOptimizerRunsResponseTypeDef](./type_defs.md#listtableoptimizerrunsresponsetypedef) 


```python
# list_table_optimizer_runs method usage example with argument unpacking

kwargs: ListTableOptimizerRunsRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Type": ...,
}

parent.list_table_optimizer_runs(**kwargs)
```

1. See [:material-code-braces: ListTableOptimizerRunsRequestRequestTypeDef](./type_defs.md#listtableoptimizerrunsrequestrequesttypedef) 

### list\_triggers

Retrieves the names of all trigger resources in this Amazon Web Services
account, or the resources with the specified tag.

Type annotations and code completion for `#!python session.client("glue").list_triggers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_triggers method definition

await def list_triggers(
    self,
    *,
    NextToken: str = ...,
    DependentJobName: str = ...,
    MaxResults: int = ...,
    Tags: Mapping[str, str] = ...,
) -> ListTriggersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTriggersResponseTypeDef](./type_defs.md#listtriggersresponsetypedef) 


```python
# list_triggers method usage example with argument unpacking

kwargs: ListTriggersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_triggers(**kwargs)
```

1. See [:material-code-braces: ListTriggersRequestRequestTypeDef](./type_defs.md#listtriggersrequestrequesttypedef) 

### list\_usage\_profiles

List all the Glue usage profiles.

Type annotations and code completion for `#!python session.client("glue").list_usage_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_usage_profiles method definition

await def list_usage_profiles(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUsageProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsageProfilesResponseTypeDef](./type_defs.md#listusageprofilesresponsetypedef) 


```python
# list_usage_profiles method usage example with argument unpacking

kwargs: ListUsageProfilesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_usage_profiles(**kwargs)
```

1. See [:material-code-braces: ListUsageProfilesRequestRequestTypeDef](./type_defs.md#listusageprofilesrequestrequesttypedef) 

### list\_workflows

Lists names of workflows created in the account.

Type annotations and code completion for `#!python session.client("glue").list_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# list_workflows method definition

await def list_workflows(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListWorkflowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# list_workflows method usage example with argument unpacking

kwargs: ListWorkflowsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_workflows(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef) 

### modify\_integration

Modifies a Zero-ETL integration in the caller's account.

Type annotations and code completion for `#!python session.client("glue").modify_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# modify_integration method definition

await def modify_integration(
    self,
    *,
    IntegrationIdentifier: str,
    Description: str = ...,
    DataFilter: str = ...,
    IntegrationName: str = ...,
) -> ModifyIntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyIntegrationResponseTypeDef](./type_defs.md#modifyintegrationresponsetypedef) 


```python
# modify_integration method usage example with argument unpacking

kwargs: ModifyIntegrationRequestRequestTypeDef = {  # (1)
    "IntegrationIdentifier": ...,
}

parent.modify_integration(**kwargs)
```

1. See [:material-code-braces: ModifyIntegrationRequestRequestTypeDef](./type_defs.md#modifyintegrationrequestrequesttypedef) 

### put\_data\_catalog\_encryption\_settings

Sets the security configuration for a specified catalog.

Type annotations and code completion for `#!python session.client("glue").put_data_catalog_encryption_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# put_data_catalog_encryption_settings method definition

await def put_data_catalog_encryption_settings(
    self,
    *,
    DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataCatalogEncryptionSettingsTypeDef](./type_defs.md#datacatalogencryptionsettingstypedef) 


```python
# put_data_catalog_encryption_settings method usage example with argument unpacking

kwargs: PutDataCatalogEncryptionSettingsRequestRequestTypeDef = {  # (1)
    "DataCatalogEncryptionSettings": ...,
}

parent.put_data_catalog_encryption_settings(**kwargs)
```

1. See [:material-code-braces: PutDataCatalogEncryptionSettingsRequestRequestTypeDef](./type_defs.md#putdatacatalogencryptionsettingsrequestrequesttypedef) 

### put\_data\_quality\_profile\_annotation

Annotate all datapoints for a Profile.

Type annotations and code completion for `#!python session.client("glue").put_data_quality_profile_annotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# put_data_quality_profile_annotation method definition

await def put_data_quality_profile_annotation(
    self,
    *,
    ProfileId: str,
    InclusionAnnotation: InclusionAnnotationValueType,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: InclusionAnnotationValueType](./literals.md#inclusionannotationvaluetype) 


```python
# put_data_quality_profile_annotation method usage example with argument unpacking

kwargs: PutDataQualityProfileAnnotationRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
    "InclusionAnnotation": ...,
}

parent.put_data_quality_profile_annotation(**kwargs)
```

1. See [:material-code-braces: PutDataQualityProfileAnnotationRequestRequestTypeDef](./type_defs.md#putdataqualityprofileannotationrequestrequesttypedef) 

### put\_resource\_policy

Sets the Data Catalog resource policy for access control.

Type annotations and code completion for `#!python session.client("glue").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    PolicyInJson: str,
    ResourceArn: str = ...,
    PolicyHashCondition: str = ...,
    PolicyExistsCondition: ExistConditionType = ...,  # (1)
    EnableHybrid: EnableHybridValuesType = ...,  # (2)
) -> PutResourcePolicyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ExistConditionType](./literals.md#existconditiontype) 
2. See [:material-code-brackets: EnableHybridValuesType](./literals.md#enablehybridvaluestype) 
3. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "PolicyInJson": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### put\_schema\_version\_metadata

Puts the metadata key value pair for a specified schema version ID.

Type annotations and code completion for `#!python session.client("glue").put_schema_version_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# put_schema_version_metadata method definition

await def put_schema_version_metadata(
    self,
    *,
    MetadataKeyValue: MetadataKeyValuePairTypeDef,  # (1)
    SchemaId: SchemaIdTypeDef = ...,  # (2)
    SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,  # (3)
    SchemaVersionId: str = ...,
) -> PutSchemaVersionMetadataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
2. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
4. See [:material-code-braces: PutSchemaVersionMetadataResponseTypeDef](./type_defs.md#putschemaversionmetadataresponsetypedef) 


```python
# put_schema_version_metadata method usage example with argument unpacking

kwargs: PutSchemaVersionMetadataInputRequestTypeDef = {  # (1)
    "MetadataKeyValue": ...,
}

parent.put_schema_version_metadata(**kwargs)
```

1. See [:material-code-braces: PutSchemaVersionMetadataInputRequestTypeDef](./type_defs.md#putschemaversionmetadatainputrequesttypedef) 

### put\_workflow\_run\_properties

Puts the specified workflow run properties for the given workflow run.

Type annotations and code completion for `#!python session.client("glue").put_workflow_run_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# put_workflow_run_properties method definition

await def put_workflow_run_properties(
    self,
    *,
    Name: str,
    RunId: str,
    RunProperties: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# put_workflow_run_properties method usage example with argument unpacking

kwargs: PutWorkflowRunPropertiesRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RunId": ...,
    "RunProperties": ...,
}

parent.put_workflow_run_properties(**kwargs)
```

1. See [:material-code-braces: PutWorkflowRunPropertiesRequestRequestTypeDef](./type_defs.md#putworkflowrunpropertiesrequestrequesttypedef) 

### query\_schema\_version\_metadata

Queries for the schema version metadata information.

Type annotations and code completion for `#!python session.client("glue").query_schema_version_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# query_schema_version_metadata method definition

await def query_schema_version_metadata(
    self,
    *,
    SchemaId: SchemaIdTypeDef = ...,  # (1)
    SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,  # (2)
    SchemaVersionId: str = ...,
    MetadataList: Sequence[MetadataKeyValuePairTypeDef] = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> QuerySchemaVersionMetadataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
4. See [:material-code-braces: QuerySchemaVersionMetadataResponseTypeDef](./type_defs.md#queryschemaversionmetadataresponsetypedef) 


```python
# query_schema_version_metadata method usage example with argument unpacking

kwargs: QuerySchemaVersionMetadataInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.query_schema_version_metadata(**kwargs)
```

1. See [:material-code-braces: QuerySchemaVersionMetadataInputRequestTypeDef](./type_defs.md#queryschemaversionmetadatainputrequesttypedef) 

### register\_schema\_version

Adds a new version to the existing schema.

Type annotations and code completion for `#!python session.client("glue").register_schema_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# register_schema_version method definition

await def register_schema_version(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaDefinition: str,
) -> RegisterSchemaVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: RegisterSchemaVersionResponseTypeDef](./type_defs.md#registerschemaversionresponsetypedef) 


```python
# register_schema_version method usage example with argument unpacking

kwargs: RegisterSchemaVersionInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
    "SchemaDefinition": ...,
}

parent.register_schema_version(**kwargs)
```

1. See [:material-code-braces: RegisterSchemaVersionInputRequestTypeDef](./type_defs.md#registerschemaversioninputrequesttypedef) 

### remove\_schema\_version\_metadata

Removes a key value pair from the schema version metadata for the specified
schema version ID.

Type annotations and code completion for `#!python session.client("glue").remove_schema_version_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# remove_schema_version_metadata method definition

await def remove_schema_version_metadata(
    self,
    *,
    MetadataKeyValue: MetadataKeyValuePairTypeDef,  # (1)
    SchemaId: SchemaIdTypeDef = ...,  # (2)
    SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,  # (3)
    SchemaVersionId: str = ...,
) -> RemoveSchemaVersionMetadataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
2. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
4. See [:material-code-braces: RemoveSchemaVersionMetadataResponseTypeDef](./type_defs.md#removeschemaversionmetadataresponsetypedef) 


```python
# remove_schema_version_metadata method usage example with argument unpacking

kwargs: RemoveSchemaVersionMetadataInputRequestTypeDef = {  # (1)
    "MetadataKeyValue": ...,
}

parent.remove_schema_version_metadata(**kwargs)
```

1. See [:material-code-braces: RemoveSchemaVersionMetadataInputRequestTypeDef](./type_defs.md#removeschemaversionmetadatainputrequesttypedef) 

### reset\_job\_bookmark

Resets a bookmark entry.

Type annotations and code completion for `#!python session.client("glue").reset_job_bookmark` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# reset_job_bookmark method definition

await def reset_job_bookmark(
    self,
    *,
    JobName: str,
    RunId: str = ...,
) -> ResetJobBookmarkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetJobBookmarkResponseTypeDef](./type_defs.md#resetjobbookmarkresponsetypedef) 


```python
# reset_job_bookmark method usage example with argument unpacking

kwargs: ResetJobBookmarkRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.reset_job_bookmark(**kwargs)
```

1. See [:material-code-braces: ResetJobBookmarkRequestRequestTypeDef](./type_defs.md#resetjobbookmarkrequestrequesttypedef) 

### resume\_workflow\_run

Restarts selected nodes of a previous partially completed workflow run and
resumes the workflow run.

Type annotations and code completion for `#!python session.client("glue").resume_workflow_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# resume_workflow_run method definition

await def resume_workflow_run(
    self,
    *,
    Name: str,
    RunId: str,
    NodeIds: Sequence[str],
) -> ResumeWorkflowRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResumeWorkflowRunResponseTypeDef](./type_defs.md#resumeworkflowrunresponsetypedef) 


```python
# resume_workflow_run method usage example with argument unpacking

kwargs: ResumeWorkflowRunRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RunId": ...,
    "NodeIds": ...,
}

parent.resume_workflow_run(**kwargs)
```

1. See [:material-code-braces: ResumeWorkflowRunRequestRequestTypeDef](./type_defs.md#resumeworkflowrunrequestrequesttypedef) 

### run\_statement

Executes the statement.

Type annotations and code completion for `#!python session.client("glue").run_statement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# run_statement method definition

await def run_statement(
    self,
    *,
    SessionId: str,
    Code: str,
    RequestOrigin: str = ...,
) -> RunStatementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RunStatementResponseTypeDef](./type_defs.md#runstatementresponsetypedef) 


```python
# run_statement method usage example with argument unpacking

kwargs: RunStatementRequestRequestTypeDef = {  # (1)
    "SessionId": ...,
    "Code": ...,
}

parent.run_statement(**kwargs)
```

1. See [:material-code-braces: RunStatementRequestRequestTypeDef](./type_defs.md#runstatementrequestrequesttypedef) 

### search\_tables

Searches a set of tables based on properties in the table metadata as well as
on the parent database.

Type annotations and code completion for `#!python session.client("glue").search_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# search_tables method definition

await def search_tables(
    self,
    *,
    CatalogId: str = ...,
    NextToken: str = ...,
    Filters: Sequence[PropertyPredicateTypeDef] = ...,  # (1)
    SearchText: str = ...,
    SortCriteria: Sequence[SortCriterionTypeDef] = ...,  # (2)
    MaxResults: int = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (3)
    IncludeStatusDetails: bool = ...,
) -> SearchTablesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PropertyPredicateTypeDef](./type_defs.md#propertypredicatetypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
4. See [:material-code-braces: SearchTablesResponseTypeDef](./type_defs.md#searchtablesresponsetypedef) 


```python
# search_tables method usage example with argument unpacking

kwargs: SearchTablesRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.search_tables(**kwargs)
```

1. See [:material-code-braces: SearchTablesRequestRequestTypeDef](./type_defs.md#searchtablesrequestrequesttypedef) 

### start\_blueprint\_run

Starts a new run of the specified blueprint.

Type annotations and code completion for `#!python session.client("glue").start_blueprint_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_blueprint_run method definition

await def start_blueprint_run(
    self,
    *,
    BlueprintName: str,
    RoleArn: str,
    Parameters: str = ...,
) -> StartBlueprintRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartBlueprintRunResponseTypeDef](./type_defs.md#startblueprintrunresponsetypedef) 


```python
# start_blueprint_run method usage example with argument unpacking

kwargs: StartBlueprintRunRequestRequestTypeDef = {  # (1)
    "BlueprintName": ...,
    "RoleArn": ...,
}

parent.start_blueprint_run(**kwargs)
```

1. See [:material-code-braces: StartBlueprintRunRequestRequestTypeDef](./type_defs.md#startblueprintrunrequestrequesttypedef) 

### start\_column\_statistics\_task\_run

Starts a column statistics task run, for a specified table and columns.

Type annotations and code completion for `#!python session.client("glue").start_column_statistics_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_column_statistics_task_run method definition

await def start_column_statistics_task_run(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    Role: str,
    ColumnNameList: Sequence[str] = ...,
    SampleSize: float = ...,
    CatalogID: str = ...,
    SecurityConfiguration: str = ...,
) -> StartColumnStatisticsTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartColumnStatisticsTaskRunResponseTypeDef](./type_defs.md#startcolumnstatisticstaskrunresponsetypedef) 


```python
# start_column_statistics_task_run method usage example with argument unpacking

kwargs: StartColumnStatisticsTaskRunRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "Role": ...,
}

parent.start_column_statistics_task_run(**kwargs)
```

1. See [:material-code-braces: StartColumnStatisticsTaskRunRequestRequestTypeDef](./type_defs.md#startcolumnstatisticstaskrunrequestrequesttypedef) 

### start\_column\_statistics\_task\_run\_schedule

Starts a column statistics task run schedule.

Type annotations and code completion for `#!python session.client("glue").start_column_statistics_task_run_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_column_statistics_task_run_schedule method definition

await def start_column_statistics_task_run_schedule(
    self,
    *,
    DatabaseName: str,
    TableName: str,
) -> dict[str, Any]:
    ...
```



```python
# start_column_statistics_task_run_schedule method usage example with argument unpacking

kwargs: StartColumnStatisticsTaskRunScheduleRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.start_column_statistics_task_run_schedule(**kwargs)
```

1. See [:material-code-braces: StartColumnStatisticsTaskRunScheduleRequestRequestTypeDef](./type_defs.md#startcolumnstatisticstaskrunschedulerequestrequesttypedef) 

### start\_crawler

Starts a crawl using the specified crawler, regardless of what is scheduled.

Type annotations and code completion for `#!python session.client("glue").start_crawler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_crawler method definition

await def start_crawler(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# start_crawler method usage example with argument unpacking

kwargs: StartCrawlerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_crawler(**kwargs)
```

1. See [:material-code-braces: StartCrawlerRequestRequestTypeDef](./type_defs.md#startcrawlerrequestrequesttypedef) 

### start\_crawler\_schedule

Changes the schedule state of the specified crawler to <code>SCHEDULED</code>,
unless the crawler is already running or the schedule state is already
<code>SCHEDULED</code>.

Type annotations and code completion for `#!python session.client("glue").start_crawler_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_crawler_schedule method definition

await def start_crawler_schedule(
    self,
    *,
    CrawlerName: str,
) -> dict[str, Any]:
    ...
```



```python
# start_crawler_schedule method usage example with argument unpacking

kwargs: StartCrawlerScheduleRequestRequestTypeDef = {  # (1)
    "CrawlerName": ...,
}

parent.start_crawler_schedule(**kwargs)
```

1. See [:material-code-braces: StartCrawlerScheduleRequestRequestTypeDef](./type_defs.md#startcrawlerschedulerequestrequesttypedef) 

### start\_data\_quality\_rule\_recommendation\_run

Starts a recommendation run that is used to generate rules when you don't know
what rules to write.

Type annotations and code completion for `#!python session.client("glue").start_data_quality_rule_recommendation_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_data_quality_rule_recommendation_run method definition

await def start_data_quality_rule_recommendation_run(
    self,
    *,
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: int = ...,
    Timeout: int = ...,
    CreatedRulesetName: str = ...,
    DataQualitySecurityConfiguration: str = ...,
    ClientToken: str = ...,
) -> StartDataQualityRuleRecommendationRunResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: StartDataQualityRuleRecommendationRunResponseTypeDef](./type_defs.md#startdataqualityrulerecommendationrunresponsetypedef) 


```python
# start_data_quality_rule_recommendation_run method usage example with argument unpacking

kwargs: StartDataQualityRuleRecommendationRunRequestRequestTypeDef = {  # (1)
    "DataSource": ...,
    "Role": ...,
}

parent.start_data_quality_rule_recommendation_run(**kwargs)
```

1. See [:material-code-braces: StartDataQualityRuleRecommendationRunRequestRequestTypeDef](./type_defs.md#startdataqualityrulerecommendationrunrequestrequesttypedef) 

### start\_data\_quality\_ruleset\_evaluation\_run

Once you have a ruleset definition (either recommended or your own), you call
this operation to evaluate the ruleset against a data source (Glue table).

Type annotations and code completion for `#!python session.client("glue").start_data_quality_ruleset_evaluation_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_data_quality_ruleset_evaluation_run method definition

await def start_data_quality_ruleset_evaluation_run(
    self,
    *,
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    RulesetNames: Sequence[str],
    NumberOfWorkers: int = ...,
    Timeout: int = ...,
    ClientToken: str = ...,
    AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,  # (2)
    AdditionalDataSources: Mapping[str, DataSourceUnionTypeDef] = ...,  # (3)
) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataQualityEvaluationRunAdditionalRunOptionsTypeDef](./type_defs.md#dataqualityevaluationrunadditionalrunoptionstypedef) 
3. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
4. See [:material-code-braces: StartDataQualityRulesetEvaluationRunResponseTypeDef](./type_defs.md#startdataqualityrulesetevaluationrunresponsetypedef) 


```python
# start_data_quality_ruleset_evaluation_run method usage example with argument unpacking

kwargs: StartDataQualityRulesetEvaluationRunRequestRequestTypeDef = {  # (1)
    "DataSource": ...,
    "Role": ...,
    "RulesetNames": ...,
}

parent.start_data_quality_ruleset_evaluation_run(**kwargs)
```

1. See [:material-code-braces: StartDataQualityRulesetEvaluationRunRequestRequestTypeDef](./type_defs.md#startdataqualityrulesetevaluationrunrequestrequesttypedef) 

### start\_export\_labels\_task\_run

Begins an asynchronous task to export all labeled data for a particular
transform.

Type annotations and code completion for `#!python session.client("glue").start_export_labels_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_export_labels_task_run method definition

await def start_export_labels_task_run(
    self,
    *,
    TransformId: str,
    OutputS3Path: str,
) -> StartExportLabelsTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartExportLabelsTaskRunResponseTypeDef](./type_defs.md#startexportlabelstaskrunresponsetypedef) 


```python
# start_export_labels_task_run method usage example with argument unpacking

kwargs: StartExportLabelsTaskRunRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
    "OutputS3Path": ...,
}

parent.start_export_labels_task_run(**kwargs)
```

1. See [:material-code-braces: StartExportLabelsTaskRunRequestRequestTypeDef](./type_defs.md#startexportlabelstaskrunrequestrequesttypedef) 

### start\_import\_labels\_task\_run

Enables you to provide additional labels (examples of truth) to be used to
teach the machine learning transform and improve its quality.

Type annotations and code completion for `#!python session.client("glue").start_import_labels_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_import_labels_task_run method definition

await def start_import_labels_task_run(
    self,
    *,
    TransformId: str,
    InputS3Path: str,
    ReplaceAllLabels: bool = ...,
) -> StartImportLabelsTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartImportLabelsTaskRunResponseTypeDef](./type_defs.md#startimportlabelstaskrunresponsetypedef) 


```python
# start_import_labels_task_run method usage example with argument unpacking

kwargs: StartImportLabelsTaskRunRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
    "InputS3Path": ...,
}

parent.start_import_labels_task_run(**kwargs)
```

1. See [:material-code-braces: StartImportLabelsTaskRunRequestRequestTypeDef](./type_defs.md#startimportlabelstaskrunrequestrequesttypedef) 

### start\_job\_run

Starts a job run using a job definition.

Type annotations and code completion for `#!python session.client("glue").start_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_job_run method definition

await def start_job_run(
    self,
    *,
    JobName: str,
    JobRunQueuingEnabled: bool = ...,
    JobRunId: str = ...,
    Arguments: Mapping[str, str] = ...,
    AllocatedCapacity: int = ...,
    Timeout: int = ...,
    MaxCapacity: float = ...,
    SecurityConfiguration: str = ...,
    NotificationProperty: NotificationPropertyTypeDef = ...,  # (1)
    WorkerType: WorkerTypeType = ...,  # (2)
    NumberOfWorkers: int = ...,
    ExecutionClass: ExecutionClassType = ...,  # (3)
) -> StartJobRunResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
2. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
3. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
4. See [:material-code-braces: StartJobRunResponseTypeDef](./type_defs.md#startjobrunresponsetypedef) 


```python
# start_job_run method usage example with argument unpacking

kwargs: StartJobRunRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.start_job_run(**kwargs)
```

1. See [:material-code-braces: StartJobRunRequestRequestTypeDef](./type_defs.md#startjobrunrequestrequesttypedef) 

### start\_ml\_evaluation\_task\_run

Starts a task to estimate the quality of the transform.

Type annotations and code completion for `#!python session.client("glue").start_ml_evaluation_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_ml_evaluation_task_run method definition

await def start_ml_evaluation_task_run(
    self,
    *,
    TransformId: str,
) -> StartMLEvaluationTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMLEvaluationTaskRunResponseTypeDef](./type_defs.md#startmlevaluationtaskrunresponsetypedef) 


```python
# start_ml_evaluation_task_run method usage example with argument unpacking

kwargs: StartMLEvaluationTaskRunRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
}

parent.start_ml_evaluation_task_run(**kwargs)
```

1. See [:material-code-braces: StartMLEvaluationTaskRunRequestRequestTypeDef](./type_defs.md#startmlevaluationtaskrunrequestrequesttypedef) 

### start\_ml\_labeling\_set\_generation\_task\_run

Starts the active learning workflow for your machine learning transform to
improve the transform's quality by generating label sets and adding labels.

Type annotations and code completion for `#!python session.client("glue").start_ml_labeling_set_generation_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_ml_labeling_set_generation_task_run method definition

await def start_ml_labeling_set_generation_task_run(
    self,
    *,
    TransformId: str,
    OutputS3Path: str,
) -> StartMLLabelingSetGenerationTaskRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMLLabelingSetGenerationTaskRunResponseTypeDef](./type_defs.md#startmllabelingsetgenerationtaskrunresponsetypedef) 


```python
# start_ml_labeling_set_generation_task_run method usage example with argument unpacking

kwargs: StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
    "OutputS3Path": ...,
}

parent.start_ml_labeling_set_generation_task_run(**kwargs)
```

1. See [:material-code-braces: StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef](./type_defs.md#startmllabelingsetgenerationtaskrunrequestrequesttypedef) 

### start\_trigger

Starts an existing trigger.

Type annotations and code completion for `#!python session.client("glue").start_trigger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_trigger method definition

await def start_trigger(
    self,
    *,
    Name: str,
) -> StartTriggerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartTriggerResponseTypeDef](./type_defs.md#starttriggerresponsetypedef) 


```python
# start_trigger method usage example with argument unpacking

kwargs: StartTriggerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_trigger(**kwargs)
```

1. See [:material-code-braces: StartTriggerRequestRequestTypeDef](./type_defs.md#starttriggerrequestrequesttypedef) 

### start\_workflow\_run

Starts a new run of the specified workflow.

Type annotations and code completion for `#!python session.client("glue").start_workflow_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# start_workflow_run method definition

await def start_workflow_run(
    self,
    *,
    Name: str,
    RunProperties: Mapping[str, str] = ...,
) -> StartWorkflowRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartWorkflowRunResponseTypeDef](./type_defs.md#startworkflowrunresponsetypedef) 


```python
# start_workflow_run method usage example with argument unpacking

kwargs: StartWorkflowRunRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_workflow_run(**kwargs)
```

1. See [:material-code-braces: StartWorkflowRunRequestRequestTypeDef](./type_defs.md#startworkflowrunrequestrequesttypedef) 

### stop\_column\_statistics\_task\_run

Stops a task run for the specified table.

Type annotations and code completion for `#!python session.client("glue").stop_column_statistics_task_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_column_statistics_task_run method definition

await def stop_column_statistics_task_run(
    self,
    *,
    DatabaseName: str,
    TableName: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_column_statistics_task_run method usage example with argument unpacking

kwargs: StopColumnStatisticsTaskRunRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.stop_column_statistics_task_run(**kwargs)
```

1. See [:material-code-braces: StopColumnStatisticsTaskRunRequestRequestTypeDef](./type_defs.md#stopcolumnstatisticstaskrunrequestrequesttypedef) 

### stop\_column\_statistics\_task\_run\_schedule

Stops a column statistics task run schedule.

Type annotations and code completion for `#!python session.client("glue").stop_column_statistics_task_run_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_column_statistics_task_run_schedule method definition

await def stop_column_statistics_task_run_schedule(
    self,
    *,
    DatabaseName: str,
    TableName: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_column_statistics_task_run_schedule method usage example with argument unpacking

kwargs: StopColumnStatisticsTaskRunScheduleRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.stop_column_statistics_task_run_schedule(**kwargs)
```

1. See [:material-code-braces: StopColumnStatisticsTaskRunScheduleRequestRequestTypeDef](./type_defs.md#stopcolumnstatisticstaskrunschedulerequestrequesttypedef) 

### stop\_crawler

If the specified crawler is running, stops the crawl.

Type annotations and code completion for `#!python session.client("glue").stop_crawler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_crawler method definition

await def stop_crawler(
    self,
    *,
    Name: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_crawler method usage example with argument unpacking

kwargs: StopCrawlerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.stop_crawler(**kwargs)
```

1. See [:material-code-braces: StopCrawlerRequestRequestTypeDef](./type_defs.md#stopcrawlerrequestrequesttypedef) 

### stop\_crawler\_schedule

Sets the schedule state of the specified crawler to <code>NOT_SCHEDULED</code>,
but does not stop the crawler if it is already running.

Type annotations and code completion for `#!python session.client("glue").stop_crawler_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_crawler_schedule method definition

await def stop_crawler_schedule(
    self,
    *,
    CrawlerName: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_crawler_schedule method usage example with argument unpacking

kwargs: StopCrawlerScheduleRequestRequestTypeDef = {  # (1)
    "CrawlerName": ...,
}

parent.stop_crawler_schedule(**kwargs)
```

1. See [:material-code-braces: StopCrawlerScheduleRequestRequestTypeDef](./type_defs.md#stopcrawlerschedulerequestrequesttypedef) 

### stop\_session

Stops the session.

Type annotations and code completion for `#!python session.client("glue").stop_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_session method definition

await def stop_session(
    self,
    *,
    Id: str,
    RequestOrigin: str = ...,
) -> StopSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopSessionResponseTypeDef](./type_defs.md#stopsessionresponsetypedef) 


```python
# stop_session method usage example with argument unpacking

kwargs: StopSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.stop_session(**kwargs)
```

1. See [:material-code-braces: StopSessionRequestRequestTypeDef](./type_defs.md#stopsessionrequestrequesttypedef) 

### stop\_trigger

Stops a specified trigger.

Type annotations and code completion for `#!python session.client("glue").stop_trigger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_trigger method definition

await def stop_trigger(
    self,
    *,
    Name: str,
) -> StopTriggerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopTriggerResponseTypeDef](./type_defs.md#stoptriggerresponsetypedef) 


```python
# stop_trigger method usage example with argument unpacking

kwargs: StopTriggerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.stop_trigger(**kwargs)
```

1. See [:material-code-braces: StopTriggerRequestRequestTypeDef](./type_defs.md#stoptriggerrequestrequesttypedef) 

### stop\_workflow\_run

Stops the execution of the specified workflow run.

Type annotations and code completion for `#!python session.client("glue").stop_workflow_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# stop_workflow_run method definition

await def stop_workflow_run(
    self,
    *,
    Name: str,
    RunId: str,
) -> dict[str, Any]:
    ...
```



```python
# stop_workflow_run method usage example with argument unpacking

kwargs: StopWorkflowRunRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RunId": ...,
}

parent.stop_workflow_run(**kwargs)
```

1. See [:material-code-braces: StopWorkflowRunRequestRequestTypeDef](./type_defs.md#stopworkflowrunrequestrequesttypedef) 

### tag\_resource

Adds tags to a resource.

Type annotations and code completion for `#!python session.client("glue").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    TagsToAdd: Mapping[str, str],
) -> dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagsToAdd": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_connection

Tests a connection to a service to validate the service credentials that you
provide.

Type annotations and code completion for `#!python session.client("glue").test_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# test_connection method definition

await def test_connection(
    self,
    *,
    ConnectionName: str = ...,
    CatalogId: str = ...,
    TestConnectionInput: TestConnectionInputTypeDef = ...,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TestConnectionInputTypeDef](./type_defs.md#testconnectioninputtypedef) 


```python
# test_connection method usage example with argument unpacking

kwargs: TestConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionName": ...,
}

parent.test_connection(**kwargs)
```

1. See [:material-code-braces: TestConnectionRequestRequestTypeDef](./type_defs.md#testconnectionrequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.client("glue").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagsToRemove: Sequence[str],
) -> dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagsToRemove": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_blueprint

Updates a registered blueprint.

Type annotations and code completion for `#!python session.client("glue").update_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_blueprint method definition

await def update_blueprint(
    self,
    *,
    Name: str,
    BlueprintLocation: str,
    Description: str = ...,
) -> UpdateBlueprintResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBlueprintResponseTypeDef](./type_defs.md#updateblueprintresponsetypedef) 


```python
# update_blueprint method usage example with argument unpacking

kwargs: UpdateBlueprintRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "BlueprintLocation": ...,
}

parent.update_blueprint(**kwargs)
```

1. See [:material-code-braces: UpdateBlueprintRequestRequestTypeDef](./type_defs.md#updateblueprintrequestrequesttypedef) 

### update\_catalog

Updates an existing catalog's properties in the Glue Data Catalog.

Type annotations and code completion for `#!python session.client("glue").update_catalog` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_catalog method definition

await def update_catalog(
    self,
    *,
    CatalogId: str,
    CatalogInput: CatalogInputTypeDef,  # (1)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: CatalogInputTypeDef](./type_defs.md#cataloginputtypedef) 


```python
# update_catalog method usage example with argument unpacking

kwargs: UpdateCatalogRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "CatalogInput": ...,
}

parent.update_catalog(**kwargs)
```

1. See [:material-code-braces: UpdateCatalogRequestRequestTypeDef](./type_defs.md#updatecatalogrequestrequesttypedef) 

### update\_classifier

Modifies an existing classifier (a <code>GrokClassifier</code>, an
<code>XMLClassifier</code>, a <code>JsonClassifier</code>, or a
<code>CsvClassifier</code>, depending on which field is present).

Type annotations and code completion for `#!python session.client("glue").update_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_classifier method definition

await def update_classifier(
    self,
    *,
    GrokClassifier: UpdateGrokClassifierRequestTypeDef = ...,  # (1)
    XMLClassifier: UpdateXMLClassifierRequestTypeDef = ...,  # (2)
    JsonClassifier: UpdateJsonClassifierRequestTypeDef = ...,  # (3)
    CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...,  # (4)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: UpdateGrokClassifierRequestTypeDef](./type_defs.md#updategrokclassifierrequesttypedef) 
2. See [:material-code-braces: UpdateXMLClassifierRequestTypeDef](./type_defs.md#updatexmlclassifierrequesttypedef) 
3. See [:material-code-braces: UpdateJsonClassifierRequestTypeDef](./type_defs.md#updatejsonclassifierrequesttypedef) 
4. See [:material-code-braces: UpdateCsvClassifierRequestTypeDef](./type_defs.md#updatecsvclassifierrequesttypedef) 


```python
# update_classifier method usage example with argument unpacking

kwargs: UpdateClassifierRequestRequestTypeDef = {  # (1)
    "GrokClassifier": ...,
}

parent.update_classifier(**kwargs)
```

1. See [:material-code-braces: UpdateClassifierRequestRequestTypeDef](./type_defs.md#updateclassifierrequestrequesttypedef) 

### update\_column\_statistics\_for\_partition

Creates or updates partition statistics of columns.

Type annotations and code completion for `#!python session.client("glue").update_column_statistics_for_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_column_statistics_for_partition method definition

await def update_column_statistics_for_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnStatisticsList: Sequence[ColumnStatisticsUnionTypeDef],  # (1)
    CatalogId: str = ...,
) -> UpdateColumnStatisticsForPartitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) [:material-code-braces: ColumnStatisticsOutputTypeDef](./type_defs.md#columnstatisticsoutputtypedef) 
2. See [:material-code-braces: UpdateColumnStatisticsForPartitionResponseTypeDef](./type_defs.md#updatecolumnstatisticsforpartitionresponsetypedef) 


```python
# update_column_statistics_for_partition method usage example with argument unpacking

kwargs: UpdateColumnStatisticsForPartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValues": ...,
    "ColumnStatisticsList": ...,
}

parent.update_column_statistics_for_partition(**kwargs)
```

1. See [:material-code-braces: UpdateColumnStatisticsForPartitionRequestRequestTypeDef](./type_defs.md#updatecolumnstatisticsforpartitionrequestrequesttypedef) 

### update\_column\_statistics\_for\_table

Creates or updates table statistics of columns.

Type annotations and code completion for `#!python session.client("glue").update_column_statistics_for_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_column_statistics_for_table method definition

await def update_column_statistics_for_table(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],  # (1)
    CatalogId: str = ...,
) -> UpdateColumnStatisticsForTableResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
2. See [:material-code-braces: UpdateColumnStatisticsForTableResponseTypeDef](./type_defs.md#updatecolumnstatisticsfortableresponsetypedef) 


```python
# update_column_statistics_for_table method usage example with argument unpacking

kwargs: UpdateColumnStatisticsForTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "ColumnStatisticsList": ...,
}

parent.update_column_statistics_for_table(**kwargs)
```

1. See [:material-code-braces: UpdateColumnStatisticsForTableRequestRequestTypeDef](./type_defs.md#updatecolumnstatisticsfortablerequestrequesttypedef) 

### update\_column\_statistics\_task\_settings

Updates settings for a column statistics task.

Type annotations and code completion for `#!python session.client("glue").update_column_statistics_task_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_column_statistics_task_settings method definition

await def update_column_statistics_task_settings(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    Role: str = ...,
    Schedule: str = ...,
    ColumnNameList: Sequence[str] = ...,
    SampleSize: float = ...,
    CatalogID: str = ...,
    SecurityConfiguration: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_column_statistics_task_settings method usage example with argument unpacking

kwargs: UpdateColumnStatisticsTaskSettingsRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
}

parent.update_column_statistics_task_settings(**kwargs)
```

1. See [:material-code-braces: UpdateColumnStatisticsTaskSettingsRequestRequestTypeDef](./type_defs.md#updatecolumnstatisticstasksettingsrequestrequesttypedef) 

### update\_connection

Updates a connection definition in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").update_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_connection method definition

await def update_connection(
    self,
    *,
    Name: str,
    ConnectionInput: ConnectionInputTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: ConnectionInputTypeDef](./type_defs.md#connectioninputtypedef) 


```python
# update_connection method usage example with argument unpacking

kwargs: UpdateConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ConnectionInput": ...,
}

parent.update_connection(**kwargs)
```

1. See [:material-code-braces: UpdateConnectionRequestRequestTypeDef](./type_defs.md#updateconnectionrequestrequesttypedef) 

### update\_crawler

Updates a crawler.

Type annotations and code completion for `#!python session.client("glue").update_crawler` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_crawler method definition

await def update_crawler(
    self,
    *,
    Name: str,
    Role: str = ...,
    DatabaseName: str = ...,
    Description: str = ...,
    Targets: CrawlerTargetsTypeDef = ...,  # (1)
    Schedule: str = ...,
    Classifiers: Sequence[str] = ...,
    TablePrefix: str = ...,
    SchemaChangePolicy: SchemaChangePolicyTypeDef = ...,  # (2)
    RecrawlPolicy: RecrawlPolicyTypeDef = ...,  # (3)
    LineageConfiguration: LineageConfigurationTypeDef = ...,  # (4)
    LakeFormationConfiguration: LakeFormationConfigurationTypeDef = ...,  # (5)
    Configuration: str = ...,
    CrawlerSecurityConfiguration: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
3. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 


```python
# update_crawler method usage example with argument unpacking

kwargs: UpdateCrawlerRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_crawler(**kwargs)
```

1. See [:material-code-braces: UpdateCrawlerRequestRequestTypeDef](./type_defs.md#updatecrawlerrequestrequesttypedef) 

### update\_crawler\_schedule

Updates the schedule of a crawler using a <code>cron</code> expression.

Type annotations and code completion for `#!python session.client("glue").update_crawler_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_crawler_schedule method definition

await def update_crawler_schedule(
    self,
    *,
    CrawlerName: str,
    Schedule: str = ...,
) -> dict[str, Any]:
    ...
```



```python
# update_crawler_schedule method usage example with argument unpacking

kwargs: UpdateCrawlerScheduleRequestRequestTypeDef = {  # (1)
    "CrawlerName": ...,
}

parent.update_crawler_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateCrawlerScheduleRequestRequestTypeDef](./type_defs.md#updatecrawlerschedulerequestrequesttypedef) 

### update\_data\_quality\_ruleset

Updates the specified data quality ruleset.

Type annotations and code completion for `#!python session.client("glue").update_data_quality_ruleset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_data_quality_ruleset method definition

await def update_data_quality_ruleset(
    self,
    *,
    Name: str,
    Description: str = ...,
    Ruleset: str = ...,
) -> UpdateDataQualityRulesetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDataQualityRulesetResponseTypeDef](./type_defs.md#updatedataqualityrulesetresponsetypedef) 


```python
# update_data_quality_ruleset method usage example with argument unpacking

kwargs: UpdateDataQualityRulesetRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_data_quality_ruleset(**kwargs)
```

1. See [:material-code-braces: UpdateDataQualityRulesetRequestRequestTypeDef](./type_defs.md#updatedataqualityrulesetrequestrequesttypedef) 

### update\_database

Updates an existing database definition in a Data Catalog.

Type annotations and code completion for `#!python session.client("glue").update_database` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_database method definition

await def update_database(
    self,
    *,
    Name: str,
    DatabaseInput: DatabaseInputTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DatabaseInputTypeDef](./type_defs.md#databaseinputtypedef) 


```python
# update_database method usage example with argument unpacking

kwargs: UpdateDatabaseRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "DatabaseInput": ...,
}

parent.update_database(**kwargs)
```

1. See [:material-code-braces: UpdateDatabaseRequestRequestTypeDef](./type_defs.md#updatedatabaserequestrequesttypedef) 

### update\_dev\_endpoint

Updates a specified development endpoint.

Type annotations and code completion for `#!python session.client("glue").update_dev_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_dev_endpoint method definition

await def update_dev_endpoint(
    self,
    *,
    EndpointName: str,
    PublicKey: str = ...,
    AddPublicKeys: Sequence[str] = ...,
    DeletePublicKeys: Sequence[str] = ...,
    CustomLibraries: DevEndpointCustomLibrariesTypeDef = ...,  # (1)
    UpdateEtlLibraries: bool = ...,
    DeleteArguments: Sequence[str] = ...,
    AddArguments: Mapping[str, str] = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: DevEndpointCustomLibrariesTypeDef](./type_defs.md#devendpointcustomlibrariestypedef) 


```python
# update_dev_endpoint method usage example with argument unpacking

kwargs: UpdateDevEndpointRequestRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.update_dev_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateDevEndpointRequestRequestTypeDef](./type_defs.md#updatedevendpointrequestrequesttypedef) 

### update\_integration\_resource\_property

This API can be used for updating the <code>ResourceProperty</code> of the Glue
connection (for the source) or Glue database ARN (for the target).

Type annotations and code completion for `#!python session.client("glue").update_integration_resource_property` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_integration_resource_property method definition

await def update_integration_resource_property(
    self,
    *,
    ResourceArn: str,
    SourceProcessingProperties: SourceProcessingPropertiesTypeDef = ...,  # (1)
    TargetProcessingProperties: TargetProcessingPropertiesTypeDef = ...,  # (2)
) -> UpdateIntegrationResourcePropertyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
3. See [:material-code-braces: UpdateIntegrationResourcePropertyResponseTypeDef](./type_defs.md#updateintegrationresourcepropertyresponsetypedef) 


```python
# update_integration_resource_property method usage example with argument unpacking

kwargs: UpdateIntegrationResourcePropertyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.update_integration_resource_property(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationResourcePropertyRequestRequestTypeDef](./type_defs.md#updateintegrationresourcepropertyrequestrequesttypedef) 

### update\_integration\_table\_properties

This API is used to provide optional override properties for the tables that
need to be replicated.

Type annotations and code completion for `#!python session.client("glue").update_integration_table_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_integration_table_properties method definition

await def update_integration_table_properties(
    self,
    *,
    ResourceArn: str,
    TableName: str,
    SourceTableConfig: SourceTableConfigTypeDef = ...,  # (1)
    TargetTableConfig: TargetTableConfigTypeDef = ...,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: SourceTableConfigTypeDef](./type_defs.md#sourcetableconfigtypedef) 
2. See [:material-code-braces: TargetTableConfigTypeDef](./type_defs.md#targettableconfigtypedef) 


```python
# update_integration_table_properties method usage example with argument unpacking

kwargs: UpdateIntegrationTablePropertiesRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TableName": ...,
}

parent.update_integration_table_properties(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationTablePropertiesRequestRequestTypeDef](./type_defs.md#updateintegrationtablepropertiesrequestrequesttypedef) 

### update\_job

Updates an existing job definition.

Type annotations and code completion for `#!python session.client("glue").update_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_job method definition

await def update_job(
    self,
    *,
    JobName: str,
    JobUpdate: JobUpdateTypeDef,  # (1)
) -> UpdateJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: JobUpdateTypeDef](./type_defs.md#jobupdatetypedef) 
2. See [:material-code-braces: UpdateJobResponseTypeDef](./type_defs.md#updatejobresponsetypedef) 


```python
# update_job method usage example with argument unpacking

kwargs: UpdateJobRequestRequestTypeDef = {  # (1)
    "JobName": ...,
    "JobUpdate": ...,
}

parent.update_job(**kwargs)
```

1. See [:material-code-braces: UpdateJobRequestRequestTypeDef](./type_defs.md#updatejobrequestrequesttypedef) 

### update\_job\_from\_source\_control

Synchronizes a job from the source control repository.

Type annotations and code completion for `#!python session.client("glue").update_job_from_source_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_job_from_source_control method definition

await def update_job_from_source_control(
    self,
    *,
    JobName: str = ...,
    Provider: SourceControlProviderType = ...,  # (1)
    RepositoryName: str = ...,
    RepositoryOwner: str = ...,
    BranchName: str = ...,
    Folder: str = ...,
    CommitId: str = ...,
    AuthStrategy: SourceControlAuthStrategyType = ...,  # (2)
    AuthToken: str = ...,
) -> UpdateJobFromSourceControlResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
3. See [:material-code-braces: UpdateJobFromSourceControlResponseTypeDef](./type_defs.md#updatejobfromsourcecontrolresponsetypedef) 


```python
# update_job_from_source_control method usage example with argument unpacking

kwargs: UpdateJobFromSourceControlRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.update_job_from_source_control(**kwargs)
```

1. See [:material-code-braces: UpdateJobFromSourceControlRequestRequestTypeDef](./type_defs.md#updatejobfromsourcecontrolrequestrequesttypedef) 

### update\_ml\_transform

Updates an existing machine learning transform.

Type annotations and code completion for `#!python session.client("glue").update_ml_transform` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_ml_transform method definition

await def update_ml_transform(
    self,
    *,
    TransformId: str,
    Name: str = ...,
    Description: str = ...,
    Parameters: TransformParametersTypeDef = ...,  # (1)
    Role: str = ...,
    GlueVersion: str = ...,
    MaxCapacity: float = ...,
    WorkerType: WorkerTypeType = ...,  # (2)
    NumberOfWorkers: int = ...,
    Timeout: int = ...,
    MaxRetries: int = ...,
) -> UpdateMLTransformResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
2. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
3. See [:material-code-braces: UpdateMLTransformResponseTypeDef](./type_defs.md#updatemltransformresponsetypedef) 


```python
# update_ml_transform method usage example with argument unpacking

kwargs: UpdateMLTransformRequestRequestTypeDef = {  # (1)
    "TransformId": ...,
}

parent.update_ml_transform(**kwargs)
```

1. See [:material-code-braces: UpdateMLTransformRequestRequestTypeDef](./type_defs.md#updatemltransformrequestrequesttypedef) 

### update\_partition

Updates a partition.

Type annotations and code completion for `#!python session.client("glue").update_partition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_partition method definition

await def update_partition(
    self,
    *,
    DatabaseName: str,
    TableName: str,
    PartitionValueList: Sequence[str],
    PartitionInput: PartitionInputTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 


```python
# update_partition method usage example with argument unpacking

kwargs: UpdatePartitionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableName": ...,
    "PartitionValueList": ...,
    "PartitionInput": ...,
}

parent.update_partition(**kwargs)
```

1. See [:material-code-braces: UpdatePartitionRequestRequestTypeDef](./type_defs.md#updatepartitionrequestrequesttypedef) 

### update\_registry

Updates an existing registry which is used to hold a collection of schemas.

Type annotations and code completion for `#!python session.client("glue").update_registry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_registry method definition

await def update_registry(
    self,
    *,
    RegistryId: RegistryIdTypeDef,  # (1)
    Description: str,
) -> UpdateRegistryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: UpdateRegistryResponseTypeDef](./type_defs.md#updateregistryresponsetypedef) 


```python
# update_registry method usage example with argument unpacking

kwargs: UpdateRegistryInputRequestTypeDef = {  # (1)
    "RegistryId": ...,
    "Description": ...,
}

parent.update_registry(**kwargs)
```

1. See [:material-code-braces: UpdateRegistryInputRequestTypeDef](./type_defs.md#updateregistryinputrequesttypedef) 

### update\_schema

Updates the description, compatibility setting, or version checkpoint for a
schema set.

Type annotations and code completion for `#!python session.client("glue").update_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_schema method definition

await def update_schema(
    self,
    *,
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaVersionNumber: SchemaVersionNumberTypeDef = ...,  # (2)
    Compatibility: CompatibilityType = ...,  # (3)
    Description: str = ...,
) -> UpdateSchemaResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
4. See [:material-code-braces: UpdateSchemaResponseTypeDef](./type_defs.md#updateschemaresponsetypedef) 


```python
# update_schema method usage example with argument unpacking

kwargs: UpdateSchemaInputRequestTypeDef = {  # (1)
    "SchemaId": ...,
}

parent.update_schema(**kwargs)
```

1. See [:material-code-braces: UpdateSchemaInputRequestTypeDef](./type_defs.md#updateschemainputrequesttypedef) 

### update\_source\_control\_from\_job

Synchronizes a job to the source control repository.

Type annotations and code completion for `#!python session.client("glue").update_source_control_from_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_source_control_from_job method definition

await def update_source_control_from_job(
    self,
    *,
    JobName: str = ...,
    Provider: SourceControlProviderType = ...,  # (1)
    RepositoryName: str = ...,
    RepositoryOwner: str = ...,
    BranchName: str = ...,
    Folder: str = ...,
    CommitId: str = ...,
    AuthStrategy: SourceControlAuthStrategyType = ...,  # (2)
    AuthToken: str = ...,
) -> UpdateSourceControlFromJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
3. See [:material-code-braces: UpdateSourceControlFromJobResponseTypeDef](./type_defs.md#updatesourcecontrolfromjobresponsetypedef) 


```python
# update_source_control_from_job method usage example with argument unpacking

kwargs: UpdateSourceControlFromJobRequestRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.update_source_control_from_job(**kwargs)
```

1. See [:material-code-braces: UpdateSourceControlFromJobRequestRequestTypeDef](./type_defs.md#updatesourcecontrolfromjobrequestrequesttypedef) 

### update\_table

Updates a metadata table in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").update_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_table method definition

await def update_table(
    self,
    *,
    DatabaseName: str,
    TableInput: TableInputTypeDef,  # (1)
    CatalogId: str = ...,
    SkipArchive: bool = ...,
    TransactionId: str = ...,
    VersionId: str = ...,
    ViewUpdateAction: ViewUpdateActionType = ...,  # (2)
    Force: bool = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: TableInputTypeDef](./type_defs.md#tableinputtypedef) 
2. See [:material-code-brackets: ViewUpdateActionType](./literals.md#viewupdateactiontype) 


```python
# update_table method usage example with argument unpacking

kwargs: UpdateTableRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "TableInput": ...,
}

parent.update_table(**kwargs)
```

1. See [:material-code-braces: UpdateTableRequestRequestTypeDef](./type_defs.md#updatetablerequestrequesttypedef) 

### update\_table\_optimizer

Updates the configuration for an existing table optimizer.

Type annotations and code completion for `#!python session.client("glue").update_table_optimizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_table_optimizer method definition

await def update_table_optimizer(
    self,
    *,
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,  # (2)
) -> dict[str, Any]:
    ...
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: TableOptimizerConfigurationTypeDef](./type_defs.md#tableoptimizerconfigurationtypedef) 


```python
# update_table_optimizer method usage example with argument unpacking

kwargs: UpdateTableOptimizerRequestRequestTypeDef = {  # (1)
    "CatalogId": ...,
    "DatabaseName": ...,
    "TableName": ...,
    "Type": ...,
    "TableOptimizerConfiguration": ...,
}

parent.update_table_optimizer(**kwargs)
```

1. See [:material-code-braces: UpdateTableOptimizerRequestRequestTypeDef](./type_defs.md#updatetableoptimizerrequestrequesttypedef) 

### update\_trigger

Updates a trigger definition.

Type annotations and code completion for `#!python session.client("glue").update_trigger` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_trigger method definition

await def update_trigger(
    self,
    *,
    Name: str,
    TriggerUpdate: TriggerUpdateTypeDef,  # (1)
) -> UpdateTriggerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TriggerUpdateTypeDef](./type_defs.md#triggerupdatetypedef) 
2. See [:material-code-braces: UpdateTriggerResponseTypeDef](./type_defs.md#updatetriggerresponsetypedef) 


```python
# update_trigger method usage example with argument unpacking

kwargs: UpdateTriggerRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "TriggerUpdate": ...,
}

parent.update_trigger(**kwargs)
```

1. See [:material-code-braces: UpdateTriggerRequestRequestTypeDef](./type_defs.md#updatetriggerrequestrequesttypedef) 

### update\_usage\_profile

Update an Glue usage profile.

Type annotations and code completion for `#!python session.client("glue").update_usage_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_usage_profile method definition

await def update_usage_profile(
    self,
    *,
    Name: str,
    Configuration: ProfileConfigurationTypeDef,  # (1)
    Description: str = ...,
) -> UpdateUsageProfileResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ProfileConfigurationTypeDef](./type_defs.md#profileconfigurationtypedef) 
2. See [:material-code-braces: UpdateUsageProfileResponseTypeDef](./type_defs.md#updateusageprofileresponsetypedef) 


```python
# update_usage_profile method usage example with argument unpacking

kwargs: UpdateUsageProfileRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Configuration": ...,
}

parent.update_usage_profile(**kwargs)
```

1. See [:material-code-braces: UpdateUsageProfileRequestRequestTypeDef](./type_defs.md#updateusageprofilerequestrequesttypedef) 

### update\_user\_defined\_function

Updates an existing function definition in the Data Catalog.

Type annotations and code completion for `#!python session.client("glue").update_user_defined_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_user_defined_function method definition

await def update_user_defined_function(
    self,
    *,
    DatabaseName: str,
    FunctionName: str,
    FunctionInput: UserDefinedFunctionInputTypeDef,  # (1)
    CatalogId: str = ...,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: UserDefinedFunctionInputTypeDef](./type_defs.md#userdefinedfunctioninputtypedef) 


```python
# update_user_defined_function method usage example with argument unpacking

kwargs: UpdateUserDefinedFunctionRequestRequestTypeDef = {  # (1)
    "DatabaseName": ...,
    "FunctionName": ...,
    "FunctionInput": ...,
}

parent.update_user_defined_function(**kwargs)
```

1. See [:material-code-braces: UpdateUserDefinedFunctionRequestRequestTypeDef](./type_defs.md#updateuserdefinedfunctionrequestrequesttypedef) 

### update\_workflow

Updates an existing workflow.

Type annotations and code completion for `#!python session.client("glue").update_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# update_workflow method definition

await def update_workflow(
    self,
    *,
    Name: str,
    Description: str = ...,
    DefaultRunProperties: Mapping[str, str] = ...,
    MaxConcurrentRuns: int = ...,
) -> UpdateWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateWorkflowResponseTypeDef](./type_defs.md#updateworkflowresponsetypedef) 


```python
# update_workflow method usage example with argument unpacking

kwargs: UpdateWorkflowRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateWorkflowRequestRequestTypeDef](./type_defs.md#updateworkflowrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("glue").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("glue").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("glue").get_paginator` method with overloads.

- `client.get_paginator("describe_entity")` -> [DescribeEntityPaginator](./paginators.md#describeentitypaginator)
- `client.get_paginator("get_classifiers")` -> [GetClassifiersPaginator](./paginators.md#getclassifierspaginator)
- `client.get_paginator("get_connections")` -> [GetConnectionsPaginator](./paginators.md#getconnectionspaginator)
- `client.get_paginator("get_crawler_metrics")` -> [GetCrawlerMetricsPaginator](./paginators.md#getcrawlermetricspaginator)
- `client.get_paginator("get_crawlers")` -> [GetCrawlersPaginator](./paginators.md#getcrawlerspaginator)
- `client.get_paginator("get_databases")` -> [GetDatabasesPaginator](./paginators.md#getdatabasespaginator)
- `client.get_paginator("get_dev_endpoints")` -> [GetDevEndpointsPaginator](./paginators.md#getdevendpointspaginator)
- `client.get_paginator("get_job_runs")` -> [GetJobRunsPaginator](./paginators.md#getjobrunspaginator)
- `client.get_paginator("get_jobs")` -> [GetJobsPaginator](./paginators.md#getjobspaginator)
- `client.get_paginator("get_partition_indexes")` -> [GetPartitionIndexesPaginator](./paginators.md#getpartitionindexespaginator)
- `client.get_paginator("get_partitions")` -> [GetPartitionsPaginator](./paginators.md#getpartitionspaginator)
- `client.get_paginator("get_resource_policies")` -> [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
- `client.get_paginator("get_security_configurations")` -> [GetSecurityConfigurationsPaginator](./paginators.md#getsecurityconfigurationspaginator)
- `client.get_paginator("get_table_versions")` -> [GetTableVersionsPaginator](./paginators.md#gettableversionspaginator)
- `client.get_paginator("get_tables")` -> [GetTablesPaginator](./paginators.md#gettablespaginator)
- `client.get_paginator("get_triggers")` -> [GetTriggersPaginator](./paginators.md#gettriggerspaginator)
- `client.get_paginator("get_user_defined_functions")` -> [GetUserDefinedFunctionsPaginator](./paginators.md#getuserdefinedfunctionspaginator)
- `client.get_paginator("get_workflow_runs")` -> [GetWorkflowRunsPaginator](./paginators.md#getworkflowrunspaginator)
- `client.get_paginator("list_blueprints")` -> [ListBlueprintsPaginator](./paginators.md#listblueprintspaginator)
- `client.get_paginator("list_connection_types")` -> [ListConnectionTypesPaginator](./paginators.md#listconnectiontypespaginator)
- `client.get_paginator("list_entities")` -> [ListEntitiesPaginator](./paginators.md#listentitiespaginator)
- `client.get_paginator("list_jobs")` -> [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_registries")` -> [ListRegistriesPaginator](./paginators.md#listregistriespaginator)
- `client.get_paginator("list_schema_versions")` -> [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)
- `client.get_paginator("list_schemas")` -> [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- `client.get_paginator("list_table_optimizer_runs")` -> [ListTableOptimizerRunsPaginator](./paginators.md#listtableoptimizerrunspaginator)
- `client.get_paginator("list_triggers")` -> [ListTriggersPaginator](./paginators.md#listtriggerspaginator)
- `client.get_paginator("list_usage_profiles")` -> [ListUsageProfilesPaginator](./paginators.md#listusageprofilespaginator)
- `client.get_paginator("list_workflows")` -> [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)


