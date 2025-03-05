# BraketClient

> [Index](../README.md) > [Braket](./README.md) > BraketClient

!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).

## BraketClient

Type annotations and code completion for `#!python session.client("braket")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# BraketClient usage example

from aioboto3.session import Session
from types_aiobotocore_braket.client import BraketClient

session = Session()
async with session.client("braket") as client:
    client: BraketClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("braket").exceptions` structure.

```python
# BraketClient.exceptions usage example

async with session.client("braket") as client:
    try:
        do_something(client)
    except (
            client.exceptions.AccessDeniedException,
        client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.DeviceOfflineException,
        client.exceptions.DeviceRetiredException,
        client.exceptions.InternalServiceException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ThrottlingException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# BraketClient.exceptions type checking example

from types_aiobotocore_braket.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("braket").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("braket").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

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


### cancel\_job

Cancels an Amazon Braket job.

Type annotations and code completion for `#!python session.client("braket").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# cancel_job method definition

await def cancel_job(
    self,
    *,
    jobArn: str,
) -> CancelJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef)


```python
# cancel_job method usage example with argument unpacking

kwargs: CancelJobRequestTypeDef = {  # (1)
    "jobArn": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobRequestTypeDef](./type_defs.md#canceljobrequesttypedef)

### cancel\_quantum\_task

Cancels the specified task.

Type annotations and code completion for `#!python session.client("braket").cancel_quantum_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# cancel_quantum_task method definition

await def cancel_quantum_task(
    self,
    *,
    clientToken: str,
    quantumTaskArn: str,
) -> CancelQuantumTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelQuantumTaskResponseTypeDef](./type_defs.md#cancelquantumtaskresponsetypedef)


```python
# cancel_quantum_task method usage example with argument unpacking

kwargs: CancelQuantumTaskRequestTypeDef = {  # (1)
    "clientToken": ...,
    "quantumTaskArn": ...,
}

parent.cancel_quantum_task(**kwargs)
```

1. See [:material-code-braces: CancelQuantumTaskRequestTypeDef](./type_defs.md#cancelquantumtaskrequesttypedef)

### create\_job

Creates an Amazon Braket job.

Type annotations and code completion for `#!python session.client("braket").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# create_job method definition

await def create_job(
    self,
    *,
    algorithmSpecification: AlgorithmSpecificationTypeDef,  # (1)
    clientToken: str,
    deviceConfig: DeviceConfigTypeDef,  # (2)
    instanceConfig: InstanceConfigTypeDef,  # (3)
    jobName: str,
    outputDataConfig: JobOutputDataConfigTypeDef,  # (4)
    roleArn: str,
    associations: Sequence[AssociationTypeDef] = ...,  # (5)
    checkpointConfig: JobCheckpointConfigTypeDef = ...,  # (6)
    hyperParameters: Mapping[str, str] = ...,
    inputDataConfig: Sequence[InputFileConfigTypeDef] = ...,  # (7)
    stoppingCondition: JobStoppingConditionTypeDef = ...,  # (8)
    tags: Mapping[str, str] = ...,
) -> CreateJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef)
2. See [:material-code-braces: DeviceConfigTypeDef](./type_defs.md#deviceconfigtypedef)
3. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef)
4. See [:material-code-braces: JobOutputDataConfigTypeDef](./type_defs.md#joboutputdataconfigtypedef)
5. See `Sequence[AssociationTypeDef]`
6. See [:material-code-braces: JobCheckpointConfigTypeDef](./type_defs.md#jobcheckpointconfigtypedef)
7. See `Sequence[InputFileConfigTypeDef]`
8. See [:material-code-braces: JobStoppingConditionTypeDef](./type_defs.md#jobstoppingconditiontypedef)
9. See [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef)


```python
# create_job method usage example with argument unpacking

kwargs: CreateJobRequestTypeDef = {  # (1)
    "algorithmSpecification": ...,
    "clientToken": ...,
    "deviceConfig": ...,
    "instanceConfig": ...,
    "jobName": ...,
    "outputDataConfig": ...,
    "roleArn": ...,
}

parent.create_job(**kwargs)
```

1. See [:material-code-braces: CreateJobRequestTypeDef](./type_defs.md#createjobrequesttypedef)

### create\_quantum\_task

Creates a quantum task.

Type annotations and code completion for `#!python session.client("braket").create_quantum_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# create_quantum_task method definition

await def create_quantum_task(
    self,
    *,
    action: str,
    clientToken: str,
    deviceArn: str,
    outputS3Bucket: str,
    outputS3KeyPrefix: str,
    shots: int,
    associations: Sequence[AssociationTypeDef] = ...,  # (1)
    deviceParameters: str = ...,
    jobToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateQuantumTaskResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[AssociationTypeDef]`
2. See [:material-code-braces: CreateQuantumTaskResponseTypeDef](./type_defs.md#createquantumtaskresponsetypedef)


```python
# create_quantum_task method usage example with argument unpacking

kwargs: CreateQuantumTaskRequestTypeDef = {  # (1)
    "action": ...,
    "clientToken": ...,
    "deviceArn": ...,
    "outputS3Bucket": ...,
    "outputS3KeyPrefix": ...,
    "shots": ...,
}

parent.create_quantum_task(**kwargs)
```

1. See [:material-code-braces: CreateQuantumTaskRequestTypeDef](./type_defs.md#createquantumtaskrequesttypedef)

### get\_device

Retrieves the devices available in Amazon Braket.

Type annotations and code completion for `#!python session.client("braket").get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# get_device method definition

await def get_device(
    self,
    *,
    deviceArn: str,
) -> GetDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef)


```python
# get_device method usage example with argument unpacking

kwargs: GetDeviceRequestTypeDef = {  # (1)
    "deviceArn": ...,
}

parent.get_device(**kwargs)
```

1. See [:material-code-braces: GetDeviceRequestTypeDef](./type_defs.md#getdevicerequesttypedef)

### get\_job

Retrieves the specified Amazon Braket job.

Type annotations and code completion for `#!python session.client("braket").get_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# get_job method definition

await def get_job(
    self,
    *,
    jobArn: str,
    additionalAttributeNames: Sequence[HybridJobAdditionalAttributeNameType] = ...,  # (1)
) -> GetJobResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[Literal['QueueInfo']]`
2. See [:material-code-braces: GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef)


```python
# get_job method usage example with argument unpacking

kwargs: GetJobRequestTypeDef = {  # (1)
    "jobArn": ...,
}

parent.get_job(**kwargs)
```

1. See [:material-code-braces: GetJobRequestTypeDef](./type_defs.md#getjobrequesttypedef)

### get\_quantum\_task

Retrieves the specified quantum task.

Type annotations and code completion for `#!python session.client("braket").get_quantum_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# get_quantum_task method definition

await def get_quantum_task(
    self,
    *,
    quantumTaskArn: str,
    additionalAttributeNames: Sequence[QuantumTaskAdditionalAttributeNameType] = ...,  # (1)
) -> GetQuantumTaskResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[Literal['QueueInfo']]`
2. See [:material-code-braces: GetQuantumTaskResponseTypeDef](./type_defs.md#getquantumtaskresponsetypedef)


```python
# get_quantum_task method usage example with argument unpacking

kwargs: GetQuantumTaskRequestTypeDef = {  # (1)
    "quantumTaskArn": ...,
}

parent.get_quantum_task(**kwargs)
```

1. See [:material-code-braces: GetQuantumTaskRequestTypeDef](./type_defs.md#getquantumtaskrequesttypedef)

### list\_tags\_for\_resource

Shows the tags associated with this resource.

Type annotations and code completion for `#!python session.client("braket").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### search\_devices

Searches for devices using the specified filters.

Type annotations and code completion for `#!python session.client("braket").search_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# search_devices method definition

await def search_devices(
    self,
    *,
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchDevicesResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[SearchDevicesFilterTypeDef]`
2. See [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef)


```python
# search_devices method usage example with argument unpacking

kwargs: SearchDevicesRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.search_devices(**kwargs)
```

1. See [:material-code-braces: SearchDevicesRequestTypeDef](./type_defs.md#searchdevicesrequesttypedef)

### search\_jobs

Searches for Amazon Braket jobs that match the specified filter values.

Type annotations and code completion for `#!python session.client("braket").search_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# search_jobs method definition

await def search_jobs(
    self,
    *,
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchJobsResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[SearchJobsFilterTypeDef]`
2. See [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef)


```python
# search_jobs method usage example with argument unpacking

kwargs: SearchJobsRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.search_jobs(**kwargs)
```

1. See [:material-code-braces: SearchJobsRequestTypeDef](./type_defs.md#searchjobsrequesttypedef)

### search\_quantum\_tasks

Searches for tasks that match the specified filter values.

Type annotations and code completion for `#!python session.client("braket").search_quantum_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# search_quantum_tasks method definition

await def search_quantum_tasks(
    self,
    *,
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchQuantumTasksResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[SearchQuantumTasksFilterTypeDef]`
2. See [:material-code-braces: SearchQuantumTasksResponseTypeDef](./type_defs.md#searchquantumtasksresponsetypedef)


```python
# search_quantum_tasks method usage example with argument unpacking

kwargs: SearchQuantumTasksRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.search_quantum_tasks(**kwargs)
```

1. See [:material-code-braces: SearchQuantumTasksRequestTypeDef](./type_defs.md#searchquantumtasksrequesttypedef)

### tag\_resource

Add a tag to the specified resource.

Type annotations and code completion for `#!python session.client("braket").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

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

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Remove tags from a resource.

Type annotations and code completion for `#!python session.client("braket").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("braket").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("braket").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

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

Type annotations and code completion for `#!python session.client("braket").get_paginator` method with overloads.

- `client.get_paginator("search_devices")` -> [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
- `client.get_paginator("search_jobs")` -> [SearchJobsPaginator](./paginators.md#searchjobspaginator)
- `client.get_paginator("search_quantum_tasks")` -> [SearchQuantumTasksPaginator](./paginators.md#searchquantumtaskspaginator)



