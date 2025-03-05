# LookoutforVisionClient

> [Index](../README.md) > [LookoutforVision](./README.md) > LookoutforVisionClient

!!! note ""

    Auto-generated documentation for [LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#lookoutforvision)
    type annotations stubs module [types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

## LookoutforVisionClient

Type annotations and code completion for `#!python session.client("lookoutvision")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# LookoutforVisionClient usage example

from aioboto3.session import Session
from types_aiobotocore_lookoutvision.client import LookoutforVisionClient

session = Session()
async with session.client("lookoutvision") as client:
    client: LookoutforVisionClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("lookoutvision").exceptions` structure.

```python
# LookoutforVisionClient.exceptions usage example

async with session.client("lookoutvision") as client:
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
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# LookoutforVisionClient.exceptions type checking example

from types_aiobotocore_lookoutvision.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("lookoutvision").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("lookoutvision").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

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


### create\_dataset

Creates a new dataset in an Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").create_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# create_dataset method definition

await def create_dataset(
    self,
    *,
    ProjectName: str,
    DatasetType: str,
    DatasetSource: DatasetSourceTypeDef = ...,  # (1)
    ClientToken: str = ...,
) -> CreateDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef)
2. See [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef)


```python
# create_dataset method usage example with argument unpacking

kwargs: CreateDatasetRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "DatasetType": ...,
}

parent.create_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDatasetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef)

### create\_model

Creates a new version of a model within an an Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").create_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# create_model method definition

await def create_model(
    self,
    *,
    ProjectName: str,
    OutputConfig: OutputConfigTypeDef,  # (1)
    Description: str = ...,
    ClientToken: str = ...,
    KmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateModelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
2. See `Sequence[TagTypeDef]`
3. See [:material-code-braces: CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef)


```python
# create_model method usage example with argument unpacking

kwargs: CreateModelRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "OutputConfig": ...,
}

parent.create_model(**kwargs)
```

1. See [:material-code-braces: CreateModelRequestTypeDef](./type_defs.md#createmodelrequesttypedef)

### create\_project

Creates an empty Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# create_project method definition

await def create_project(
    self,
    *,
    ProjectName: str,
    ClientToken: str = ...,
) -> CreateProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef)


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectRequestTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectRequestTypeDef](./type_defs.md#createprojectrequesttypedef)

### delete\_dataset

Deletes an existing Amazon Lookout for Vision <code>dataset</code>.

Type annotations and code completion for `#!python session.client("lookoutvision").delete_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# delete_dataset method definition

await def delete_dataset(
    self,
    *,
    ProjectName: str,
    DatasetType: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

```python
# delete_dataset method usage example with argument unpacking

kwargs: DeleteDatasetRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "DatasetType": ...,
}

parent.delete_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetRequestTypeDef](./type_defs.md#deletedatasetrequesttypedef)

### delete\_model

Deletes an Amazon Lookout for Vision model.

Type annotations and code completion for `#!python session.client("lookoutvision").delete_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# delete_model method definition

await def delete_model(
    self,
    *,
    ProjectName: str,
    ModelVersion: str,
    ClientToken: str = ...,
) -> DeleteModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteModelResponseTypeDef](./type_defs.md#deletemodelresponsetypedef)


```python
# delete_model method usage example with argument unpacking

kwargs: DeleteModelRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "ModelVersion": ...,
}

parent.delete_model(**kwargs)
```

1. See [:material-code-braces: DeleteModelRequestTypeDef](./type_defs.md#deletemodelrequesttypedef)

### delete\_project

Deletes an Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    ProjectName: str,
    ClientToken: str = ...,
) -> DeleteProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteProjectResponseTypeDef](./type_defs.md#deleteprojectresponsetypedef)


```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectRequestTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectRequestTypeDef](./type_defs.md#deleteprojectrequesttypedef)

### describe\_dataset

Describe an Amazon Lookout for Vision dataset.

Type annotations and code completion for `#!python session.client("lookoutvision").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    ProjectName: str,
    DatasetType: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef)


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "DatasetType": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestTypeDef](./type_defs.md#describedatasetrequesttypedef)

### describe\_model

Describes a version of an Amazon Lookout for Vision model.

Type annotations and code completion for `#!python session.client("lookoutvision").describe_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# describe_model method definition

await def describe_model(
    self,
    *,
    ProjectName: str,
    ModelVersion: str,
) -> DescribeModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelResponseTypeDef](./type_defs.md#describemodelresponsetypedef)


```python
# describe_model method usage example with argument unpacking

kwargs: DescribeModelRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "ModelVersion": ...,
}

parent.describe_model(**kwargs)
```

1. See [:material-code-braces: DescribeModelRequestTypeDef](./type_defs.md#describemodelrequesttypedef)

### describe\_model\_packaging\_job

Describes an Amazon Lookout for Vision model packaging job.

Type annotations and code completion for `#!python session.client("lookoutvision").describe_model_packaging_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# describe_model_packaging_job method definition

await def describe_model_packaging_job(
    self,
    *,
    ProjectName: str,
    JobName: str,
) -> DescribeModelPackagingJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelPackagingJobResponseTypeDef](./type_defs.md#describemodelpackagingjobresponsetypedef)


```python
# describe_model_packaging_job method usage example with argument unpacking

kwargs: DescribeModelPackagingJobRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "JobName": ...,
}

parent.describe_model_packaging_job(**kwargs)
```

1. See [:material-code-braces: DescribeModelPackagingJobRequestTypeDef](./type_defs.md#describemodelpackagingjobrequesttypedef)

### describe\_project

Describes an Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").describe_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# describe_project method definition

await def describe_project(
    self,
    *,
    ProjectName: str,
) -> DescribeProjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef)


```python
# describe_project method usage example with argument unpacking

kwargs: DescribeProjectRequestTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.describe_project(**kwargs)
```

1. See [:material-code-braces: DescribeProjectRequestTypeDef](./type_defs.md#describeprojectrequesttypedef)

### detect\_anomalies

Detects anomalies in an image that you supply.

Type annotations and code completion for `#!python session.client("lookoutvision").detect_anomalies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# detect_anomalies method definition

await def detect_anomalies(
    self,
    *,
    ProjectName: str,
    ModelVersion: str,
    Body: BlobTypeDef,
    ContentType: str,
) -> DetectAnomaliesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DetectAnomaliesResponseTypeDef](./type_defs.md#detectanomaliesresponsetypedef)


```python
# detect_anomalies method usage example with argument unpacking

kwargs: DetectAnomaliesRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "ModelVersion": ...,
    "Body": ...,
    "ContentType": ...,
}

parent.detect_anomalies(**kwargs)
```

1. See [:material-code-braces: DetectAnomaliesRequestTypeDef](./type_defs.md#detectanomaliesrequesttypedef)

### list\_dataset\_entries

Lists the JSON Lines within a dataset.

Type annotations and code completion for `#!python session.client("lookoutvision").list_dataset_entries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# list_dataset_entries method definition

await def list_dataset_entries(
    self,
    *,
    ProjectName: str,
    DatasetType: str,
    Labeled: bool = ...,
    AnomalyClass: str = ...,
    BeforeCreationDate: TimestampTypeDef = ...,
    AfterCreationDate: TimestampTypeDef = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SourceRefContains: str = ...,
) -> ListDatasetEntriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetEntriesResponseTypeDef](./type_defs.md#listdatasetentriesresponsetypedef)


```python
# list_dataset_entries method usage example with argument unpacking

kwargs: ListDatasetEntriesRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "DatasetType": ...,
}

parent.list_dataset_entries(**kwargs)
```

1. See [:material-code-braces: ListDatasetEntriesRequestTypeDef](./type_defs.md#listdatasetentriesrequesttypedef)

### list\_model\_packaging\_jobs

Lists the model packaging jobs created for an Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").list_model_packaging_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# list_model_packaging_jobs method definition

await def list_model_packaging_jobs(
    self,
    *,
    ProjectName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListModelPackagingJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListModelPackagingJobsResponseTypeDef](./type_defs.md#listmodelpackagingjobsresponsetypedef)


```python
# list_model_packaging_jobs method usage example with argument unpacking

kwargs: ListModelPackagingJobsRequestTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.list_model_packaging_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelPackagingJobsRequestTypeDef](./type_defs.md#listmodelpackagingjobsrequesttypedef)

### list\_models

Lists the versions of a model in an Amazon Lookout for Vision project.

Type annotations and code completion for `#!python session.client("lookoutvision").list_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# list_models method definition

await def list_models(
    self,
    *,
    ProjectName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListModelsResponseTypeDef](./type_defs.md#listmodelsresponsetypedef)


```python
# list_models method usage example with argument unpacking

kwargs: ListModelsRequestTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.list_models(**kwargs)
```

1. See [:material-code-braces: ListModelsRequestTypeDef](./type_defs.md#listmodelsrequesttypedef)

### list\_projects

Lists the Amazon Lookout for Vision projects in your AWS account that are in
the AWS Region in which you call <code>ListProjects</code>.

Type annotations and code completion for `#!python session.client("lookoutvision").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProjectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestTypeDef](./type_defs.md#listprojectsrequesttypedef)

### list\_tags\_for\_resource

Returns a list of tags attached to the specified Amazon Lookout for Vision
model.

Type annotations and code completion for `#!python session.client("lookoutvision").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### start\_model

Starts the running of the version of an Amazon Lookout for Vision model.

Type annotations and code completion for `#!python session.client("lookoutvision").start_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# start_model method definition

await def start_model(
    self,
    *,
    ProjectName: str,
    ModelVersion: str,
    MinInferenceUnits: int,
    ClientToken: str = ...,
    MaxInferenceUnits: int = ...,
) -> StartModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartModelResponseTypeDef](./type_defs.md#startmodelresponsetypedef)


```python
# start_model method usage example with argument unpacking

kwargs: StartModelRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "ModelVersion": ...,
    "MinInferenceUnits": ...,
}

parent.start_model(**kwargs)
```

1. See [:material-code-braces: StartModelRequestTypeDef](./type_defs.md#startmodelrequesttypedef)

### start\_model\_packaging\_job

Starts an Amazon Lookout for Vision model packaging job.

Type annotations and code completion for `#!python session.client("lookoutvision").start_model_packaging_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# start_model_packaging_job method definition

await def start_model_packaging_job(
    self,
    *,
    ProjectName: str,
    ModelVersion: str,
    Configuration: ModelPackagingConfigurationUnionTypeDef,  # (1)
    JobName: str = ...,
    Description: str = ...,
    ClientToken: str = ...,
) -> StartModelPackagingJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ModelPackagingConfigurationUnionTypeDef](#modelpackagingconfigurationuniontypedef)
2. See [:material-code-braces: StartModelPackagingJobResponseTypeDef](./type_defs.md#startmodelpackagingjobresponsetypedef)


```python
# start_model_packaging_job method usage example with argument unpacking

kwargs: StartModelPackagingJobRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "ModelVersion": ...,
    "Configuration": ...,
}

parent.start_model_packaging_job(**kwargs)
```

1. See [:material-code-braces: StartModelPackagingJobRequestTypeDef](./type_defs.md#startmodelpackagingjobrequesttypedef)

### stop\_model

Stops the hosting of a running model.

Type annotations and code completion for `#!python session.client("lookoutvision").stop_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# stop_model method definition

await def stop_model(
    self,
    *,
    ProjectName: str,
    ModelVersion: str,
    ClientToken: str = ...,
) -> StopModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopModelResponseTypeDef](./type_defs.md#stopmodelresponsetypedef)


```python
# stop_model method usage example with argument unpacking

kwargs: StopModelRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "ModelVersion": ...,
}

parent.stop_model(**kwargs)
```

1. See [:material-code-braces: StopModelRequestTypeDef](./type_defs.md#stopmodelrequesttypedef)

### tag\_resource

Adds one or more key-value tags to an Amazon Lookout for Vision model.

Type annotations and code completion for `#!python session.client("lookoutvision").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See `Sequence[TagTypeDef]`


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes one or more tags from an Amazon Lookout for Vision model.

Type annotations and code completion for `#!python session.client("lookoutvision").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_dataset\_entries

Adds or updates one or more JSON Line entries in a dataset.

Type annotations and code completion for `#!python session.client("lookoutvision").update_dataset_entries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# update_dataset_entries method definition

await def update_dataset_entries(
    self,
    *,
    ProjectName: str,
    DatasetType: str,
    Changes: BlobTypeDef,
    ClientToken: str = ...,
) -> UpdateDatasetEntriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDatasetEntriesResponseTypeDef](./type_defs.md#updatedatasetentriesresponsetypedef)


```python
# update_dataset_entries method usage example with argument unpacking

kwargs: UpdateDatasetEntriesRequestTypeDef = {  # (1)
    "ProjectName": ...,
    "DatasetType": ...,
    "Changes": ...,
}

parent.update_dataset_entries(**kwargs)
```

1. See [:material-code-braces: UpdateDatasetEntriesRequestTypeDef](./type_defs.md#updatedatasetentriesrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("lookoutvision").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("lookoutvision").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.client("lookoutvision").get_paginator` method with overloads.

- `client.get_paginator("list_dataset_entries")` -> [ListDatasetEntriesPaginator](./paginators.md#listdatasetentriespaginator)
- `client.get_paginator("list_model_packaging_jobs")` -> [ListModelPackagingJobsPaginator](./paginators.md#listmodelpackagingjobspaginator)
- `client.get_paginator("list_models")` -> [ListModelsPaginator](./paginators.md#listmodelspaginator)
- `client.get_paginator("list_projects")` -> [ListProjectsPaginator](./paginators.md#listprojectspaginator)



