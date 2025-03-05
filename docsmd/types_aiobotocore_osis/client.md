# OpenSearchIngestionClient

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > OpenSearchIngestionClient

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## OpenSearchIngestionClient

Type annotations and code completion for `#!python session.client("osis")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# OpenSearchIngestionClient usage example

from aioboto3.session import Session
from types_aiobotocore_osis.client import OpenSearchIngestionClient

session = Session()
async with session.client("osis") as client:
    client: OpenSearchIngestionClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("osis").exceptions` structure.

```python
# OpenSearchIngestionClient.exceptions usage example

async with session.client("osis") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.DisabledOperationException,
        client.exceptions.InternalException,
        client.exceptions.InvalidPaginationTokenException,
        client.exceptions.LimitExceededException,
        client.exceptions.ResourceAlreadyExistsException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# OpenSearchIngestionClient.exceptions type checking example

from types_aiobotocore_osis.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("osis").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("osis").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

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


### create\_pipeline

Creates an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").create_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# create_pipeline method definition

await def create_pipeline(
    self,
    *,
    PipelineName: str,
    MinUnits: int,
    MaxUnits: int,
    PipelineConfigurationBody: str,
    LogPublishingOptions: LogPublishingOptionsTypeDef = ...,  # (1)
    VpcOptions: VpcOptionsUnionTypeDef = ...,  # (2)
    BufferOptions: BufferOptionsTypeDef = ...,  # (3)
    EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreatePipelineResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef)
2. See [:material-code-braces: VpcOptionsUnionTypeDef](#vpcoptionsuniontypedef)
3. See [:material-code-braces: BufferOptionsTypeDef](./type_defs.md#bufferoptionstypedef)
4. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef)
5. See `Sequence[TagTypeDef]`
6. See [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)


```python
# create_pipeline method usage example with argument unpacking

kwargs: CreatePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
    "MinUnits": ...,
    "MaxUnits": ...,
    "PipelineConfigurationBody": ...,
}

parent.create_pipeline(**kwargs)
```

1. See [:material-code-braces: CreatePipelineRequestTypeDef](./type_defs.md#createpipelinerequesttypedef)

### delete\_pipeline

Deletes an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").delete_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# delete_pipeline method definition

await def delete_pipeline(
    self,
    *,
    PipelineName: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_pipeline method usage example with argument unpacking

kwargs: DeletePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.delete_pipeline(**kwargs)
```

1. See [:material-code-braces: DeletePipelineRequestTypeDef](./type_defs.md#deletepipelinerequesttypedef)

### get\_pipeline

Retrieves information about an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").get_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# get_pipeline method definition

await def get_pipeline(
    self,
    *,
    PipelineName: str,
) -> GetPipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPipelineResponseTypeDef](./type_defs.md#getpipelineresponsetypedef)


```python
# get_pipeline method usage example with argument unpacking

kwargs: GetPipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.get_pipeline(**kwargs)
```

1. See [:material-code-braces: GetPipelineRequestTypeDef](./type_defs.md#getpipelinerequesttypedef)

### get\_pipeline\_blueprint

Retrieves information about a specific blueprint for OpenSearch Ingestion.

Type annotations and code completion for `#!python session.client("osis").get_pipeline_blueprint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# get_pipeline_blueprint method definition

await def get_pipeline_blueprint(
    self,
    *,
    BlueprintName: str,
    Format: str = ...,
) -> GetPipelineBlueprintResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPipelineBlueprintResponseTypeDef](./type_defs.md#getpipelineblueprintresponsetypedef)


```python
# get_pipeline_blueprint method usage example with argument unpacking

kwargs: GetPipelineBlueprintRequestTypeDef = {  # (1)
    "BlueprintName": ...,
}

parent.get_pipeline_blueprint(**kwargs)
```

1. See [:material-code-braces: GetPipelineBlueprintRequestTypeDef](./type_defs.md#getpipelineblueprintrequesttypedef)

### get\_pipeline\_change\_progress

Returns progress information for the current change happening on an OpenSearch
Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").get_pipeline_change_progress` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# get_pipeline_change_progress method definition

await def get_pipeline_change_progress(
    self,
    *,
    PipelineName: str,
) -> GetPipelineChangeProgressResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPipelineChangeProgressResponseTypeDef](./type_defs.md#getpipelinechangeprogressresponsetypedef)


```python
# get_pipeline_change_progress method usage example with argument unpacking

kwargs: GetPipelineChangeProgressRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.get_pipeline_change_progress(**kwargs)
```

1. See [:material-code-braces: GetPipelineChangeProgressRequestTypeDef](./type_defs.md#getpipelinechangeprogressrequesttypedef)

### list\_pipeline\_blueprints

Retrieves a list of all available blueprints for Data Prepper.

Type annotations and code completion for `#!python session.client("osis").list_pipeline_blueprints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# list_pipeline_blueprints method definition

await def list_pipeline_blueprints(
    self,
) -> ListPipelineBlueprintsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPipelineBlueprintsResponseTypeDef](./type_defs.md#listpipelineblueprintsresponsetypedef)



### list\_pipelines

Lists all OpenSearch Ingestion pipelines in the current Amazon Web Services
account and Region.

Type annotations and code completion for `#!python session.client("osis").list_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# list_pipelines method definition

await def list_pipelines(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPipelinesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)


```python
# list_pipelines method usage example with argument unpacking

kwargs: ListPipelinesRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_pipelines(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestTypeDef](./type_defs.md#listpipelinesrequesttypedef)

### list\_tags\_for\_resource

Lists all resource tags associated with an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    Arn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### start\_pipeline

Starts an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").start_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# start_pipeline method definition

await def start_pipeline(
    self,
    *,
    PipelineName: str,
) -> StartPipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartPipelineResponseTypeDef](./type_defs.md#startpipelineresponsetypedef)


```python
# start_pipeline method usage example with argument unpacking

kwargs: StartPipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.start_pipeline(**kwargs)
```

1. See [:material-code-braces: StartPipelineRequestTypeDef](./type_defs.md#startpipelinerequesttypedef)

### stop\_pipeline

Stops an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").stop_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# stop_pipeline method definition

await def stop_pipeline(
    self,
    *,
    PipelineName: str,
) -> StopPipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopPipelineResponseTypeDef](./type_defs.md#stoppipelineresponsetypedef)


```python
# stop_pipeline method usage example with argument unpacking

kwargs: StopPipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.stop_pipeline(**kwargs)
```

1. See [:material-code-braces: StopPipelineRequestTypeDef](./type_defs.md#stoppipelinerequesttypedef)

### tag\_resource

Tags an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    Arn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See `Sequence[TagTypeDef]`


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "Arn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes one or more tags from an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    Arn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "Arn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_pipeline

Updates an OpenSearch Ingestion pipeline.

Type annotations and code completion for `#!python session.client("osis").update_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# update_pipeline method definition

await def update_pipeline(
    self,
    *,
    PipelineName: str,
    MinUnits: int = ...,
    MaxUnits: int = ...,
    PipelineConfigurationBody: str = ...,
    LogPublishingOptions: LogPublishingOptionsTypeDef = ...,  # (1)
    BufferOptions: BufferOptionsTypeDef = ...,  # (2)
    EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,  # (3)
) -> UpdatePipelineResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef)
2. See [:material-code-braces: BufferOptionsTypeDef](./type_defs.md#bufferoptionstypedef)
3. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef)
4. See [:material-code-braces: UpdatePipelineResponseTypeDef](./type_defs.md#updatepipelineresponsetypedef)


```python
# update_pipeline method usage example with argument unpacking

kwargs: UpdatePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.update_pipeline(**kwargs)
```

1. See [:material-code-braces: UpdatePipelineRequestTypeDef](./type_defs.md#updatepipelinerequesttypedef)

### validate\_pipeline

Checks whether an OpenSearch Ingestion pipeline configuration is valid prior to
creation.

Type annotations and code completion for `#!python session.client("osis").validate_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# validate_pipeline method definition

await def validate_pipeline(
    self,
    *,
    PipelineConfigurationBody: str,
) -> ValidatePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ValidatePipelineResponseTypeDef](./type_defs.md#validatepipelineresponsetypedef)


```python
# validate_pipeline method usage example with argument unpacking

kwargs: ValidatePipelineRequestTypeDef = {  # (1)
    "PipelineConfigurationBody": ...,
}

parent.validate_pipeline(**kwargs)
```

1. See [:material-code-braces: ValidatePipelineRequestTypeDef](./type_defs.md#validatepipelinerequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("osis").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("osis").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





