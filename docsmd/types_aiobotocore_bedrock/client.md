# BedrockClient

> [Index](../README.md) > [Bedrock](./README.md) > BedrockClient

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## BedrockClient

Type annotations and code completion for `#!python session.client("bedrock")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client)

```python
# BedrockClient usage example

from aioboto3.session import Session
from types_aiobotocore_bedrock.client import BedrockClient

session = Session()
async with session.client("bedrock") as client:
    client: BedrockClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("bedrock").exceptions` structure.

```python
# BedrockClient.exceptions usage example

async with session.client("bedrock") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.TooManyTagsException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# BedrockClient.exceptions type checking example

from types_aiobotocore_bedrock.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("bedrock").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.can_paginate)

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

Type annotations and code completion for `#!python session.client("bedrock").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_model\_customization\_job

Creates a fine-tuning job to customize a base model.

Type annotations and code completion for `#!python session.client("bedrock").create_model_customization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_model_customization_job)

```python
# create_model_customization_job method definition

await def create_model_customization_job(
    self,
    *,
    jobName: str,
    customModelName: str,
    roleArn: str,
    baseModelIdentifier: str,
    trainingDataConfig: TrainingDataConfigTypeDef,  # (1)
    outputDataConfig: OutputDataConfigTypeDef,  # (2)
    hyperParameters: Mapping[str, str],
    clientRequestToken: str = ...,
    customizationType: CustomizationTypeType = ...,  # (3)
    customModelKmsKeyId: str = ...,
    jobTags: Sequence[TagTypeDef] = ...,  # (4)
    customModelTags: Sequence[TagTypeDef] = ...,  # (4)
    validationDataConfig: ValidationDataConfigTypeDef = ...,  # (6)
    vpcConfig: VpcConfigTypeDef = ...,  # (7)
) -> CreateModelCustomizationJobResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef) 
7. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
8. See [:material-code-braces: CreateModelCustomizationJobResponseTypeDef](./type_defs.md#createmodelcustomizationjobresponsetypedef) 


```python
# create_model_customization_job method usage example with argument unpacking

kwargs: CreateModelCustomizationJobRequestRequestTypeDef = {  # (1)
    "jobName": ...,
    "customModelName": ...,
    "roleArn": ...,
    "baseModelIdentifier": ...,
    "trainingDataConfig": ...,
    "outputDataConfig": ...,
    "hyperParameters": ...,
}

parent.create_model_customization_job(**kwargs)
```

1. See [:material-code-braces: CreateModelCustomizationJobRequestRequestTypeDef](./type_defs.md#createmodelcustomizationjobrequestrequesttypedef) 

### create\_provisioned\_model\_throughput

Creates a provisioned throughput with dedicated capacity for a foundation model
or a fine-tuned
model.

Type annotations and code completion for `#!python session.client("bedrock").create_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.create_provisioned_model_throughput)

```python
# create_provisioned_model_throughput method definition

await def create_provisioned_model_throughput(
    self,
    *,
    modelUnits: int,
    provisionedModelName: str,
    modelId: str,
    clientRequestToken: str = ...,
    commitmentDuration: CommitmentDurationType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateProvisionedModelThroughputResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CommitmentDurationType](./literals.md#commitmentdurationtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateProvisionedModelThroughputResponseTypeDef](./type_defs.md#createprovisionedmodelthroughputresponsetypedef) 


```python
# create_provisioned_model_throughput method usage example with argument unpacking

kwargs: CreateProvisionedModelThroughputRequestRequestTypeDef = {  # (1)
    "modelUnits": ...,
    "provisionedModelName": ...,
    "modelId": ...,
}

parent.create_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: CreateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#createprovisionedmodelthroughputrequestrequesttypedef) 

### delete\_custom\_model

Deletes a custom model that you created earlier.

Type annotations and code completion for `#!python session.client("bedrock").delete_custom_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_custom_model)

```python
# delete_custom_model method definition

await def delete_custom_model(
    self,
    *,
    modelIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_custom_model method usage example with argument unpacking

kwargs: DeleteCustomModelRequestRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.delete_custom_model(**kwargs)
```

1. See [:material-code-braces: DeleteCustomModelRequestRequestTypeDef](./type_defs.md#deletecustommodelrequestrequesttypedef) 

### delete\_model\_invocation\_logging\_configuration

Delete the invocation logging.

Type annotations and code completion for `#!python session.client("bedrock").delete_model_invocation_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_model_invocation_logging_configuration)

```python
# delete_model_invocation_logging_configuration method definition

await def delete_model_invocation_logging_configuration(
    self,
) -> Dict[str, Any]:
    ...
```


### delete\_provisioned\_model\_throughput

Deletes a provisioned throughput.

Type annotations and code completion for `#!python session.client("bedrock").delete_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.delete_provisioned_model_throughput)

```python
# delete_provisioned_model_throughput method definition

await def delete_provisioned_model_throughput(
    self,
    *,
    provisionedModelId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_provisioned_model_throughput method usage example with argument unpacking

kwargs: DeleteProvisionedModelThroughputRequestRequestTypeDef = {  # (1)
    "provisionedModelId": ...,
}

parent.delete_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: DeleteProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#deleteprovisionedmodelthroughputrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("bedrock").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.generate_presigned_url)

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


### get\_custom\_model

Get the properties associated with a Amazon Bedrock custom model that you have
created.For more information, see [Custom
models](https://docs.aws.amazon.com/bedrock/latest/userguide/custom-models.html)
in the Bedrock User
Guide.

Type annotations and code completion for `#!python session.client("bedrock").get_custom_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_custom_model)

```python
# get_custom_model method definition

await def get_custom_model(
    self,
    *,
    modelIdentifier: str,
) -> GetCustomModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCustomModelResponseTypeDef](./type_defs.md#getcustommodelresponsetypedef) 


```python
# get_custom_model method usage example with argument unpacking

kwargs: GetCustomModelRequestRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.get_custom_model(**kwargs)
```

1. See [:material-code-braces: GetCustomModelRequestRequestTypeDef](./type_defs.md#getcustommodelrequestrequesttypedef) 

### get\_foundation\_model

Get details about a Amazon Bedrock foundation model.

Type annotations and code completion for `#!python session.client("bedrock").get_foundation_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_foundation_model)

```python
# get_foundation_model method definition

await def get_foundation_model(
    self,
    *,
    modelIdentifier: str,
) -> GetFoundationModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFoundationModelResponseTypeDef](./type_defs.md#getfoundationmodelresponsetypedef) 


```python
# get_foundation_model method usage example with argument unpacking

kwargs: GetFoundationModelRequestRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.get_foundation_model(**kwargs)
```

1. See [:material-code-braces: GetFoundationModelRequestRequestTypeDef](./type_defs.md#getfoundationmodelrequestrequesttypedef) 

### get\_model\_customization\_job

Retrieves the properties associated with a model-customization job, including
the status of the
job.

Type annotations and code completion for `#!python session.client("bedrock").get_model_customization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_model_customization_job)

```python
# get_model_customization_job method definition

await def get_model_customization_job(
    self,
    *,
    jobIdentifier: str,
) -> GetModelCustomizationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelCustomizationJobResponseTypeDef](./type_defs.md#getmodelcustomizationjobresponsetypedef) 


```python
# get_model_customization_job method usage example with argument unpacking

kwargs: GetModelCustomizationJobRequestRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.get_model_customization_job(**kwargs)
```

1. See [:material-code-braces: GetModelCustomizationJobRequestRequestTypeDef](./type_defs.md#getmodelcustomizationjobrequestrequesttypedef) 

### get\_model\_invocation\_logging\_configuration

Get the current configuration values for model invocation logging.

Type annotations and code completion for `#!python session.client("bedrock").get_model_invocation_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_model_invocation_logging_configuration)

```python
# get_model_invocation_logging_configuration method definition

await def get_model_invocation_logging_configuration(
    self,
) -> GetModelInvocationLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelInvocationLoggingConfigurationResponseTypeDef](./type_defs.md#getmodelinvocationloggingconfigurationresponsetypedef) 

### get\_provisioned\_model\_throughput

Get details for a provisioned throughput.

Type annotations and code completion for `#!python session.client("bedrock").get_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.get_provisioned_model_throughput)

```python
# get_provisioned_model_throughput method definition

await def get_provisioned_model_throughput(
    self,
    *,
    provisionedModelId: str,
) -> GetProvisionedModelThroughputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProvisionedModelThroughputResponseTypeDef](./type_defs.md#getprovisionedmodelthroughputresponsetypedef) 


```python
# get_provisioned_model_throughput method usage example with argument unpacking

kwargs: GetProvisionedModelThroughputRequestRequestTypeDef = {  # (1)
    "provisionedModelId": ...,
}

parent.get_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: GetProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#getprovisionedmodelthroughputrequestrequesttypedef) 

### list\_custom\_models

Returns a list of the custom models that you have created with the
`CreateModelCustomizationJob`
operation.

Type annotations and code completion for `#!python session.client("bedrock").list_custom_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_custom_models)

```python
# list_custom_models method definition

await def list_custom_models(
    self,
    *,
    creationTimeBefore: Union[datetime, str] = ...,
    creationTimeAfter: Union[datetime, str] = ...,
    nameContains: str = ...,
    baseModelArnEquals: str = ...,
    foundationModelArnEquals: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortModelsByType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
) -> ListCustomModelsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef) 


```python
# list_custom_models method usage example with argument unpacking

kwargs: ListCustomModelsRequestRequestTypeDef = {  # (1)
    "creationTimeBefore": ...,
}

parent.list_custom_models(**kwargs)
```

1. See [:material-code-braces: ListCustomModelsRequestRequestTypeDef](./type_defs.md#listcustommodelsrequestrequesttypedef) 

### list\_foundation\_models

List of Amazon Bedrock foundation models that you can use.

Type annotations and code completion for `#!python session.client("bedrock").list_foundation_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_foundation_models)

```python
# list_foundation_models method definition

await def list_foundation_models(
    self,
    *,
    byProvider: str = ...,
    byCustomizationType: ModelCustomizationType = ...,  # (1)
    byOutputModality: ModelModalityType = ...,  # (2)
    byInferenceType: InferenceTypeType = ...,  # (3)
) -> ListFoundationModelsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCustomizationType](./literals.md#modelcustomizationtype) 
2. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
3. See [:material-code-brackets: InferenceTypeType](./literals.md#inferencetypetype) 
4. See [:material-code-braces: ListFoundationModelsResponseTypeDef](./type_defs.md#listfoundationmodelsresponsetypedef) 


```python
# list_foundation_models method usage example with argument unpacking

kwargs: ListFoundationModelsRequestRequestTypeDef = {  # (1)
    "byProvider": ...,
}

parent.list_foundation_models(**kwargs)
```

1. See [:material-code-braces: ListFoundationModelsRequestRequestTypeDef](./type_defs.md#listfoundationmodelsrequestrequesttypedef) 

### list\_model\_customization\_jobs

Returns a list of model customization jobs that you have submitted.

Type annotations and code completion for `#!python session.client("bedrock").list_model_customization_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_model_customization_jobs)

```python
# list_model_customization_jobs method definition

await def list_model_customization_jobs(
    self,
    *,
    creationTimeAfter: Union[datetime, str] = ...,
    creationTimeBefore: Union[datetime, str] = ...,
    statusEquals: FineTuningJobStatusType = ...,  # (1)
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListModelCustomizationJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: FineTuningJobStatusType](./literals.md#finetuningjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef) 


```python
# list_model_customization_jobs method usage example with argument unpacking

kwargs: ListModelCustomizationJobsRequestRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_model_customization_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelCustomizationJobsRequestRequestTypeDef](./type_defs.md#listmodelcustomizationjobsrequestrequesttypedef) 

### list\_provisioned\_model\_throughputs

List the provisioned capacities.

Type annotations and code completion for `#!python session.client("bedrock").list_provisioned_model_throughputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_provisioned_model_throughputs)

```python
# list_provisioned_model_throughputs method definition

await def list_provisioned_model_throughputs(
    self,
    *,
    creationTimeAfter: Union[datetime, str] = ...,
    creationTimeBefore: Union[datetime, str] = ...,
    statusEquals: ProvisionedModelStatusType = ...,  # (1)
    modelArnEquals: str = ...,
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortByProvisionedModelsType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListProvisionedModelThroughputsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef) 


```python
# list_provisioned_model_throughputs method usage example with argument unpacking

kwargs: ListProvisionedModelThroughputsRequestRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_provisioned_model_throughputs(**kwargs)
```

1. See [:material-code-braces: ListProvisionedModelThroughputsRequestRequestTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequestrequesttypedef) 

### list\_tags\_for\_resource

List the tags associated with the specified resource.

Type annotations and code completion for `#!python session.client("bedrock").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_model\_invocation\_logging\_configuration

Set the configuration values for model invocation logging.

Type annotations and code completion for `#!python session.client("bedrock").put_model_invocation_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.put_model_invocation_logging_configuration)

```python
# put_model_invocation_logging_configuration method definition

await def put_model_invocation_logging_configuration(
    self,
    *,
    loggingConfig: LoggingConfigTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 


```python
# put_model_invocation_logging_configuration method usage example with argument unpacking

kwargs: PutModelInvocationLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "loggingConfig": ...,
}

parent.put_model_invocation_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutModelInvocationLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putmodelinvocationloggingconfigurationrequestrequesttypedef) 

### stop\_model\_customization\_job

Stops an active model customization job.

Type annotations and code completion for `#!python session.client("bedrock").stop_model_customization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.stop_model_customization_job)

```python
# stop_model_customization_job method definition

await def stop_model_customization_job(
    self,
    *,
    jobIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_model_customization_job method usage example with argument unpacking

kwargs: StopModelCustomizationJobRequestRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.stop_model_customization_job(**kwargs)
```

1. See [:material-code-braces: StopModelCustomizationJobRequestRequestTypeDef](./type_defs.md#stopmodelcustomizationjobrequestrequesttypedef) 

### tag\_resource

Associate tags with a resource.

Type annotations and code completion for `#!python session.client("bedrock").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Remove one or more tags from a resource.

Type annotations and code completion for `#!python session.client("bedrock").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_provisioned\_model\_throughput

Update a provisioned throughput.

Type annotations and code completion for `#!python session.client("bedrock").update_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.update_provisioned_model_throughput)

```python
# update_provisioned_model_throughput method definition

await def update_provisioned_model_throughput(
    self,
    *,
    provisionedModelId: str,
    desiredProvisionedModelName: str = ...,
    desiredModelId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_provisioned_model_throughput method usage example with argument unpacking

kwargs: UpdateProvisionedModelThroughputRequestRequestTypeDef = {  # (1)
    "provisionedModelId": ...,
}

parent.update_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: UpdateProvisionedModelThroughputRequestRequestTypeDef](./type_defs.md#updateprovisionedmodelthroughputrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("bedrock").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> BedrockClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("bedrock").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client.__aexit__)

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

Type annotations and code completion for `#!python session.client("bedrock").get_paginator` method with overloads.

- `client.get_paginator("list_custom_models")` -> [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
- `client.get_paginator("list_model_customization_jobs")` -> [ListModelCustomizationJobsPaginator](./paginators.md#listmodelcustomizationjobspaginator)
- `client.get_paginator("list_provisioned_model_throughputs")` -> [ListProvisionedModelThroughputsPaginator](./paginators.md#listprovisionedmodelthroughputspaginator)



