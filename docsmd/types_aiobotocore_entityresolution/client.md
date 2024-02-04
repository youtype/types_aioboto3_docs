# EntityResolutionClient

> [Index](../README.md) > [EntityResolution](./README.md) > EntityResolutionClient

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## EntityResolutionClient

Type annotations and code completion for `#!python session.client("entityresolution")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client)

```python
# EntityResolutionClient usage example

from aioboto3.session import Session
from types_aiobotocore_entityresolution.client import EntityResolutionClient

session = Session()
async with session.client("entityresolution") as client:
    client: EntityResolutionClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("entityresolution").exceptions` structure.

```python
# EntityResolutionClient.exceptions usage example

async with session.client("entityresolution") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.ExceedsLimitException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# EntityResolutionClient.exceptions type checking example

from types_aiobotocore_entityresolution.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("entityresolution").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("entityresolution").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_id\_mapping\_workflow

Creates an `IdMappingWorkflow` object which stores the configuration of the
data processing job to be
run.

Type annotations and code completion for `#!python session.client("entityresolution").create_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_id_mapping_workflow)

```python
# create_id_mapping_workflow method definition

await def create_id_mapping_workflow(
    self,
    *,
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowName: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateIdMappingWorkflowOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: CreateIdMappingWorkflowOutputTypeDef](./type_defs.md#createidmappingworkflowoutputtypedef) 


```python
# create_id_mapping_workflow method usage example with argument unpacking

kwargs: CreateIdMappingWorkflowInputRequestTypeDef = {  # (1)
    "idMappingTechniques": ...,
    "inputSourceConfig": ...,
    "outputSourceConfig": ...,
    "roleArn": ...,
    "workflowName": ...,
}

parent.create_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: CreateIdMappingWorkflowInputRequestTypeDef](./type_defs.md#createidmappingworkflowinputrequesttypedef) 

### create\_matching\_workflow

Creates a `MatchingWorkflow` object which stores the configuration of the data
processing job to be
run.

Type annotations and code completion for `#!python session.client("entityresolution").create_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_matching_workflow)

```python
# create_matching_workflow method definition

await def create_matching_workflow(
    self,
    *,
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: str = ...,
    incrementalRunConfig: IncrementalRunConfigTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
) -> CreateMatchingWorkflowOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
5. See [:material-code-braces: CreateMatchingWorkflowOutputTypeDef](./type_defs.md#creatematchingworkflowoutputtypedef) 


```python
# create_matching_workflow method usage example with argument unpacking

kwargs: CreateMatchingWorkflowInputRequestTypeDef = {  # (1)
    "inputSourceConfig": ...,
    "outputSourceConfig": ...,
    "resolutionTechniques": ...,
    "roleArn": ...,
    "workflowName": ...,
}

parent.create_matching_workflow(**kwargs)
```

1. See [:material-code-braces: CreateMatchingWorkflowInputRequestTypeDef](./type_defs.md#creatematchingworkflowinputrequesttypedef) 

### create\_schema\_mapping

Creates a schema mapping, which defines the schema of the input customer
records
table.

Type annotations and code completion for `#!python session.client("entityresolution").create_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.create_schema_mapping)

```python
# create_schema_mapping method definition

await def create_schema_mapping(
    self,
    *,
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateSchemaMappingOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: CreateSchemaMappingOutputTypeDef](./type_defs.md#createschemamappingoutputtypedef) 


```python
# create_schema_mapping method usage example with argument unpacking

kwargs: CreateSchemaMappingInputRequestTypeDef = {  # (1)
    "mappedInputFields": ...,
    "schemaName": ...,
}

parent.create_schema_mapping(**kwargs)
```

1. See [:material-code-braces: CreateSchemaMappingInputRequestTypeDef](./type_defs.md#createschemamappinginputrequesttypedef) 

### delete\_id\_mapping\_workflow

Deletes the `IdMappingWorkflow` with a given name.

Type annotations and code completion for `#!python session.client("entityresolution").delete_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_id_mapping_workflow)

```python
# delete_id_mapping_workflow method definition

await def delete_id_mapping_workflow(
    self,
    *,
    workflowName: str,
) -> DeleteIdMappingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIdMappingWorkflowOutputTypeDef](./type_defs.md#deleteidmappingworkflowoutputtypedef) 


```python
# delete_id_mapping_workflow method usage example with argument unpacking

kwargs: DeleteIdMappingWorkflowInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.delete_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteIdMappingWorkflowInputRequestTypeDef](./type_defs.md#deleteidmappingworkflowinputrequesttypedef) 

### delete\_matching\_workflow

Deletes the `MatchingWorkflow` with a given name.

Type annotations and code completion for `#!python session.client("entityresolution").delete_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_matching_workflow)

```python
# delete_matching_workflow method definition

await def delete_matching_workflow(
    self,
    *,
    workflowName: str,
) -> DeleteMatchingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMatchingWorkflowOutputTypeDef](./type_defs.md#deletematchingworkflowoutputtypedef) 


```python
# delete_matching_workflow method usage example with argument unpacking

kwargs: DeleteMatchingWorkflowInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.delete_matching_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteMatchingWorkflowInputRequestTypeDef](./type_defs.md#deletematchingworkflowinputrequesttypedef) 

### delete\_schema\_mapping

Deletes the `SchemaMapping` with a given name.

Type annotations and code completion for `#!python session.client("entityresolution").delete_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.delete_schema_mapping)

```python
# delete_schema_mapping method definition

await def delete_schema_mapping(
    self,
    *,
    schemaName: str,
) -> DeleteSchemaMappingOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteSchemaMappingOutputTypeDef](./type_defs.md#deleteschemamappingoutputtypedef) 


```python
# delete_schema_mapping method usage example with argument unpacking

kwargs: DeleteSchemaMappingInputRequestTypeDef = {  # (1)
    "schemaName": ...,
}

parent.delete_schema_mapping(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaMappingInputRequestTypeDef](./type_defs.md#deleteschemamappinginputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("entityresolution").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.generate_presigned_url)

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


### get\_id\_mapping\_job

Gets the status, metrics, and errors (if there are any) that are associated
with a
job.

Type annotations and code completion for `#!python session.client("entityresolution").get_id_mapping_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_id_mapping_job)

```python
# get_id_mapping_job method definition

await def get_id_mapping_job(
    self,
    *,
    jobId: str,
    workflowName: str,
) -> GetIdMappingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdMappingJobOutputTypeDef](./type_defs.md#getidmappingjoboutputtypedef) 


```python
# get_id_mapping_job method usage example with argument unpacking

kwargs: GetIdMappingJobInputRequestTypeDef = {  # (1)
    "jobId": ...,
    "workflowName": ...,
}

parent.get_id_mapping_job(**kwargs)
```

1. See [:material-code-braces: GetIdMappingJobInputRequestTypeDef](./type_defs.md#getidmappingjobinputrequesttypedef) 

### get\_id\_mapping\_workflow

Returns the `IdMappingWorkflow` with a given name, if it exists.

Type annotations and code completion for `#!python session.client("entityresolution").get_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_id_mapping_workflow)

```python
# get_id_mapping_workflow method definition

await def get_id_mapping_workflow(
    self,
    *,
    workflowName: str,
) -> GetIdMappingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdMappingWorkflowOutputTypeDef](./type_defs.md#getidmappingworkflowoutputtypedef) 


```python
# get_id_mapping_workflow method usage example with argument unpacking

kwargs: GetIdMappingWorkflowInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.get_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: GetIdMappingWorkflowInputRequestTypeDef](./type_defs.md#getidmappingworkflowinputrequesttypedef) 

### get\_match\_id

Returns the corresponding Match ID of a customer record if the record has been
processed.

Type annotations and code completion for `#!python session.client("entityresolution").get_match_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_match_id)

```python
# get_match_id method definition

await def get_match_id(
    self,
    *,
    record: Mapping[str, str],
    workflowName: str,
) -> GetMatchIdOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchIdOutputTypeDef](./type_defs.md#getmatchidoutputtypedef) 


```python
# get_match_id method usage example with argument unpacking

kwargs: GetMatchIdInputRequestTypeDef = {  # (1)
    "record": ...,
    "workflowName": ...,
}

parent.get_match_id(**kwargs)
```

1. See [:material-code-braces: GetMatchIdInputRequestTypeDef](./type_defs.md#getmatchidinputrequesttypedef) 

### get\_matching\_job

Gets the status, metrics, and errors (if there are any) that are associated
with a
job.

Type annotations and code completion for `#!python session.client("entityresolution").get_matching_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_matching_job)

```python
# get_matching_job method definition

await def get_matching_job(
    self,
    *,
    jobId: str,
    workflowName: str,
) -> GetMatchingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchingJobOutputTypeDef](./type_defs.md#getmatchingjoboutputtypedef) 


```python
# get_matching_job method usage example with argument unpacking

kwargs: GetMatchingJobInputRequestTypeDef = {  # (1)
    "jobId": ...,
    "workflowName": ...,
}

parent.get_matching_job(**kwargs)
```

1. See [:material-code-braces: GetMatchingJobInputRequestTypeDef](./type_defs.md#getmatchingjobinputrequesttypedef) 

### get\_matching\_workflow

Returns the `MatchingWorkflow` with a given name, if it exists.

Type annotations and code completion for `#!python session.client("entityresolution").get_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_matching_workflow)

```python
# get_matching_workflow method definition

await def get_matching_workflow(
    self,
    *,
    workflowName: str,
) -> GetMatchingWorkflowOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchingWorkflowOutputTypeDef](./type_defs.md#getmatchingworkflowoutputtypedef) 


```python
# get_matching_workflow method usage example with argument unpacking

kwargs: GetMatchingWorkflowInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.get_matching_workflow(**kwargs)
```

1. See [:material-code-braces: GetMatchingWorkflowInputRequestTypeDef](./type_defs.md#getmatchingworkflowinputrequesttypedef) 

### get\_provider\_service

Returns the `ProviderService` of a given name.

Type annotations and code completion for `#!python session.client("entityresolution").get_provider_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_provider_service)

```python
# get_provider_service method definition

await def get_provider_service(
    self,
    *,
    providerName: str,
    providerServiceName: str,
) -> GetProviderServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProviderServiceOutputTypeDef](./type_defs.md#getproviderserviceoutputtypedef) 


```python
# get_provider_service method usage example with argument unpacking

kwargs: GetProviderServiceInputRequestTypeDef = {  # (1)
    "providerName": ...,
    "providerServiceName": ...,
}

parent.get_provider_service(**kwargs)
```

1. See [:material-code-braces: GetProviderServiceInputRequestTypeDef](./type_defs.md#getproviderserviceinputrequesttypedef) 

### get\_schema\_mapping

Returns the SchemaMapping of a given name.

Type annotations and code completion for `#!python session.client("entityresolution").get_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.get_schema_mapping)

```python
# get_schema_mapping method definition

await def get_schema_mapping(
    self,
    *,
    schemaName: str,
) -> GetSchemaMappingOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSchemaMappingOutputTypeDef](./type_defs.md#getschemamappingoutputtypedef) 


```python
# get_schema_mapping method usage example with argument unpacking

kwargs: GetSchemaMappingInputRequestTypeDef = {  # (1)
    "schemaName": ...,
}

parent.get_schema_mapping(**kwargs)
```

1. See [:material-code-braces: GetSchemaMappingInputRequestTypeDef](./type_defs.md#getschemamappinginputrequesttypedef) 

### list\_id\_mapping\_jobs

Lists all ID mapping jobs for a given workflow.

Type annotations and code completion for `#!python session.client("entityresolution").list_id_mapping_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_id_mapping_jobs)

```python
# list_id_mapping_jobs method definition

await def list_id_mapping_jobs(
    self,
    *,
    workflowName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIdMappingJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef) 


```python
# list_id_mapping_jobs method usage example with argument unpacking

kwargs: ListIdMappingJobsInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.list_id_mapping_jobs(**kwargs)
```

1. See [:material-code-braces: ListIdMappingJobsInputRequestTypeDef](./type_defs.md#listidmappingjobsinputrequesttypedef) 

### list\_id\_mapping\_workflows

Returns a list of all the `IdMappingWorkflows` that have been created for an
Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("entityresolution").list_id_mapping_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_id_mapping_workflows)

```python
# list_id_mapping_workflows method definition

await def list_id_mapping_workflows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListIdMappingWorkflowsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef) 


```python
# list_id_mapping_workflows method usage example with argument unpacking

kwargs: ListIdMappingWorkflowsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_id_mapping_workflows(**kwargs)
```

1. See [:material-code-braces: ListIdMappingWorkflowsInputRequestTypeDef](./type_defs.md#listidmappingworkflowsinputrequesttypedef) 

### list\_matching\_jobs

Lists all jobs for a given workflow.

Type annotations and code completion for `#!python session.client("entityresolution").list_matching_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_matching_jobs)

```python
# list_matching_jobs method definition

await def list_matching_jobs(
    self,
    *,
    workflowName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMatchingJobsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


```python
# list_matching_jobs method usage example with argument unpacking

kwargs: ListMatchingJobsInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.list_matching_jobs(**kwargs)
```

1. See [:material-code-braces: ListMatchingJobsInputRequestTypeDef](./type_defs.md#listmatchingjobsinputrequesttypedef) 

### list\_matching\_workflows

Returns a list of all the `MatchingWorkflows` that have been created for an
Amazon Web Services
account.

Type annotations and code completion for `#!python session.client("entityresolution").list_matching_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_matching_workflows)

```python
# list_matching_workflows method definition

await def list_matching_workflows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMatchingWorkflowsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


```python
# list_matching_workflows method usage example with argument unpacking

kwargs: ListMatchingWorkflowsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_matching_workflows(**kwargs)
```

1. See [:material-code-braces: ListMatchingWorkflowsInputRequestTypeDef](./type_defs.md#listmatchingworkflowsinputrequesttypedef) 

### list\_provider\_services

Returns a list of all the `ProviderServices` that are available in this Amazon
Web Services
Region.

Type annotations and code completion for `#!python session.client("entityresolution").list_provider_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_provider_services)

```python
# list_provider_services method definition

await def list_provider_services(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    providerName: str = ...,
) -> ListProviderServicesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef) 


```python
# list_provider_services method usage example with argument unpacking

kwargs: ListProviderServicesInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_provider_services(**kwargs)
```

1. See [:material-code-braces: ListProviderServicesInputRequestTypeDef](./type_defs.md#listproviderservicesinputrequesttypedef) 

### list\_schema\_mappings

Returns a list of all the `SchemaMappings` that have been created for an Amazon
Web Services
account.

Type annotations and code completion for `#!python session.client("entityresolution").list_schema_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_schema_mappings)

```python
# list_schema_mappings method definition

await def list_schema_mappings(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSchemaMappingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


```python
# list_schema_mappings method usage example with argument unpacking

kwargs: ListSchemaMappingsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_schema_mappings(**kwargs)
```

1. See [:material-code-braces: ListSchemaMappingsInputRequestTypeDef](./type_defs.md#listschemamappingsinputrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with an Entity Resolution resource.

Type annotations and code completion for `#!python session.client("entityresolution").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### start\_id\_mapping\_job

Starts the `IdMappingJob` of a workflow.

Type annotations and code completion for `#!python session.client("entityresolution").start_id_mapping_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.start_id_mapping_job)

```python
# start_id_mapping_job method definition

await def start_id_mapping_job(
    self,
    *,
    workflowName: str,
) -> StartIdMappingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartIdMappingJobOutputTypeDef](./type_defs.md#startidmappingjoboutputtypedef) 


```python
# start_id_mapping_job method usage example with argument unpacking

kwargs: StartIdMappingJobInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.start_id_mapping_job(**kwargs)
```

1. See [:material-code-braces: StartIdMappingJobInputRequestTypeDef](./type_defs.md#startidmappingjobinputrequesttypedef) 

### start\_matching\_job

Starts the `MatchingJob` of a workflow.

Type annotations and code completion for `#!python session.client("entityresolution").start_matching_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.start_matching_job)

```python
# start_matching_job method definition

await def start_matching_job(
    self,
    *,
    workflowName: str,
) -> StartMatchingJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMatchingJobOutputTypeDef](./type_defs.md#startmatchingjoboutputtypedef) 


```python
# start_matching_job method usage example with argument unpacking

kwargs: StartMatchingJobInputRequestTypeDef = {  # (1)
    "workflowName": ...,
}

parent.start_matching_job(**kwargs)
```

1. See [:material-code-braces: StartMatchingJobInputRequestTypeDef](./type_defs.md#startmatchingjobinputrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified Entity Resolution
resource.

Type annotations and code completion for `#!python session.client("entityresolution").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified Entity Resolution resource.

Type annotations and code completion for `#!python session.client("entityresolution").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_id\_mapping\_workflow

Updates an existing `IdMappingWorkflow`.

Type annotations and code completion for `#!python session.client("entityresolution").update_id_mapping_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_id_mapping_workflow)

```python
# update_id_mapping_workflow method definition

await def update_id_mapping_workflow(
    self,
    *,
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: Sequence[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowName: str,
    description: str = ...,
) -> UpdateIdMappingWorkflowOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: UpdateIdMappingWorkflowOutputTypeDef](./type_defs.md#updateidmappingworkflowoutputtypedef) 


```python
# update_id_mapping_workflow method usage example with argument unpacking

kwargs: UpdateIdMappingWorkflowInputRequestTypeDef = {  # (1)
    "idMappingTechniques": ...,
    "inputSourceConfig": ...,
    "outputSourceConfig": ...,
    "roleArn": ...,
    "workflowName": ...,
}

parent.update_id_mapping_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateIdMappingWorkflowInputRequestTypeDef](./type_defs.md#updateidmappingworkflowinputrequesttypedef) 

### update\_matching\_workflow

Updates an existing `MatchingWorkflow`.

Type annotations and code completion for `#!python session.client("entityresolution").update_matching_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_matching_workflow)

```python
# update_matching_workflow method definition

await def update_matching_workflow(
    self,
    *,
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: str = ...,
    incrementalRunConfig: IncrementalRunConfigTypeDef = ...,  # (4)
) -> UpdateMatchingWorkflowOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
5. See [:material-code-braces: UpdateMatchingWorkflowOutputTypeDef](./type_defs.md#updatematchingworkflowoutputtypedef) 


```python
# update_matching_workflow method usage example with argument unpacking

kwargs: UpdateMatchingWorkflowInputRequestTypeDef = {  # (1)
    "inputSourceConfig": ...,
    "outputSourceConfig": ...,
    "resolutionTechniques": ...,
    "roleArn": ...,
    "workflowName": ...,
}

parent.update_matching_workflow(**kwargs)
```

1. See [:material-code-braces: UpdateMatchingWorkflowInputRequestTypeDef](./type_defs.md#updatematchingworkflowinputrequesttypedef) 

### update\_schema\_mapping

Updates a schema mapping.

Type annotations and code completion for `#!python session.client("entityresolution").update_schema_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.update_schema_mapping)

```python
# update_schema_mapping method definition

await def update_schema_mapping(
    self,
    *,
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: str = ...,
) -> UpdateSchemaMappingOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: UpdateSchemaMappingOutputTypeDef](./type_defs.md#updateschemamappingoutputtypedef) 


```python
# update_schema_mapping method usage example with argument unpacking

kwargs: UpdateSchemaMappingInputRequestTypeDef = {  # (1)
    "mappedInputFields": ...,
    "schemaName": ...,
}

parent.update_schema_mapping(**kwargs)
```

1. See [:material-code-braces: UpdateSchemaMappingInputRequestTypeDef](./type_defs.md#updateschemamappinginputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("entityresolution").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> EntityResolutionClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("entityresolution").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("entityresolution").get_paginator` method with overloads.

- `client.get_paginator("list_id_mapping_jobs")` -> [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
- `client.get_paginator("list_id_mapping_workflows")` -> [ListIdMappingWorkflowsPaginator](./paginators.md#listidmappingworkflowspaginator)
- `client.get_paginator("list_matching_jobs")` -> [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
- `client.get_paginator("list_matching_workflows")` -> [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
- `client.get_paginator("list_provider_services")` -> [ListProviderServicesPaginator](./paginators.md#listproviderservicespaginator)
- `client.get_paginator("list_schema_mappings")` -> [ListSchemaMappingsPaginator](./paginators.md#listschemamappingspaginator)



