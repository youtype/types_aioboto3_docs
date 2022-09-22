# BraketClient

> [Index](../README.md) > [Braket](./README.md) > BraketClient

!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).

## BraketClient

Type annotations and code completion for `#!python session.client("braket")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_braket.client import BraketClient

session = Session()
async with session.client("braket") as client:
    client: BraketClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("braket").exceptions` structure.

```python title="Usage example"
async with session.client("braket") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.DeviceOfflineException,
        client.DeviceRetiredException,
        client.InternalServiceException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_braket.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("braket").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_job

Cancels an Amazon Braket job.

Type annotations and code completion for `#!python session.client("braket").cancel_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.cancel_job)

```python title="Method definition"
await def cancel_job(
    self,
    *,
    jobArn: str,
) -> CancelJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CancelJobRequestRequestTypeDef = {  # (1)
    "jobArn": ...,
}

parent.cancel_job(**kwargs)
```

1. See [:material-code-braces: CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef) 

### cancel\_quantum\_task

Cancels the specified task.

Type annotations and code completion for `#!python session.client("braket").cancel_quantum_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.cancel_quantum_task)

```python title="Method definition"
await def cancel_quantum_task(
    self,
    *,
    clientToken: str,
    quantumTaskArn: str,
) -> CancelQuantumTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelQuantumTaskResponseTypeDef](./type_defs.md#cancelquantumtaskresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CancelQuantumTaskRequestRequestTypeDef = {  # (1)
    "clientToken": ...,
    "quantumTaskArn": ...,
}

parent.cancel_quantum_task(**kwargs)
```

1. See [:material-code-braces: CancelQuantumTaskRequestRequestTypeDef](./type_defs.md#cancelquantumtaskrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.client("braket").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### create\_job

Creates an Amazon Braket job.

Type annotations and code completion for `#!python session.client("braket").create_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_job)

```python title="Method definition"
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
    checkpointConfig: JobCheckpointConfigTypeDef = ...,  # (5)
    hyperParameters: Mapping[str, str] = ...,
    inputDataConfig: Sequence[InputFileConfigTypeDef] = ...,  # (6)
    stoppingCondition: JobStoppingConditionTypeDef = ...,  # (7)
    tags: Mapping[str, str] = ...,
) -> CreateJobResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) 
2. See [:material-code-braces: DeviceConfigTypeDef](./type_defs.md#deviceconfigtypedef) 
3. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
4. See [:material-code-braces: JobOutputDataConfigTypeDef](./type_defs.md#joboutputdataconfigtypedef) 
5. See [:material-code-braces: JobCheckpointConfigTypeDef](./type_defs.md#jobcheckpointconfigtypedef) 
6. See [:material-code-braces: InputFileConfigTypeDef](./type_defs.md#inputfileconfigtypedef) 
7. See [:material-code-braces: JobStoppingConditionTypeDef](./type_defs.md#jobstoppingconditiontypedef) 
8. See [:material-code-braces: CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateJobRequestRequestTypeDef = {  # (1)
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

1. See [:material-code-braces: CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef) 

### create\_quantum\_task

Creates a quantum task.

Type annotations and code completion for `#!python session.client("braket").create_quantum_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_quantum_task)

```python title="Method definition"
await def create_quantum_task(
    self,
    *,
    action: str,
    clientToken: str,
    deviceArn: str,
    outputS3Bucket: str,
    outputS3KeyPrefix: str,
    shots: int,
    deviceParameters: str = ...,
    jobToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateQuantumTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateQuantumTaskResponseTypeDef](./type_defs.md#createquantumtaskresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateQuantumTaskRequestRequestTypeDef = {  # (1)
    "action": ...,
    "clientToken": ...,
    "deviceArn": ...,
    "outputS3Bucket": ...,
    "outputS3KeyPrefix": ...,
    "shots": ...,
}

parent.create_quantum_task(**kwargs)
```

1. See [:material-code-braces: CreateQuantumTaskRequestRequestTypeDef](./type_defs.md#createquantumtaskrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("braket").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_device

Retrieves the devices available in Amazon Braket.

Type annotations and code completion for `#!python session.client("braket").get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.get_device)

```python title="Method definition"
await def get_device(
    self,
    *,
    deviceArn: str,
) -> GetDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDeviceRequestRequestTypeDef = {  # (1)
    "deviceArn": ...,
}

parent.get_device(**kwargs)
```

1. See [:material-code-braces: GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef) 

### get\_job

Retrieves the specified Amazon Braket job.

Type annotations and code completion for `#!python session.client("braket").get_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.get_job)

```python title="Method definition"
await def get_job(
    self,
    *,
    jobArn: str,
) -> GetJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetJobRequestRequestTypeDef = {  # (1)
    "jobArn": ...,
}

parent.get_job(**kwargs)
```

1. See [:material-code-braces: GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef) 

### get\_quantum\_task

Retrieves the specified quantum task.

Type annotations and code completion for `#!python session.client("braket").get_quantum_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.get_quantum_task)

```python title="Method definition"
await def get_quantum_task(
    self,
    *,
    quantumTaskArn: str,
) -> GetQuantumTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQuantumTaskResponseTypeDef](./type_defs.md#getquantumtaskresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetQuantumTaskRequestRequestTypeDef = {  # (1)
    "quantumTaskArn": ...,
}

parent.get_quantum_task(**kwargs)
```

1. See [:material-code-braces: GetQuantumTaskRequestRequestTypeDef](./type_defs.md#getquantumtaskrequestrequesttypedef) 

### list\_tags\_for\_resource

Shows the tags associated with this resource.

Type annotations and code completion for `#!python session.client("braket").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.list_tags_for_resource)

```python title="Method definition"
await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### search\_devices

Searches for devices using the specified filters.

Type annotations and code completion for `#!python session.client("braket").search_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_devices)

```python title="Method definition"
await def search_devices(
    self,
    *,
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchDevicesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef) 
2. See [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchDevicesRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.search_devices(**kwargs)
```

1. See [:material-code-braces: SearchDevicesRequestRequestTypeDef](./type_defs.md#searchdevicesrequestrequesttypedef) 

### search\_jobs

Searches for Amazon Braket jobs that match the specified filter values.

Type annotations and code completion for `#!python session.client("braket").search_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_jobs)

```python title="Method definition"
await def search_jobs(
    self,
    *,
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef) 
2. See [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchJobsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.search_jobs(**kwargs)
```

1. See [:material-code-braces: SearchJobsRequestRequestTypeDef](./type_defs.md#searchjobsrequestrequesttypedef) 

### search\_quantum\_tasks

Searches for tasks that match the specified filter values.

Type annotations and code completion for `#!python session.client("braket").search_quantum_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_quantum_tasks)

```python title="Method definition"
await def search_quantum_tasks(
    self,
    *,
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchQuantumTasksResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef) 
2. See [:material-code-braces: SearchQuantumTasksResponseTypeDef](./type_defs.md#searchquantumtasksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchQuantumTasksRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.search_quantum_tasks(**kwargs)
```

1. See [:material-code-braces: SearchQuantumTasksRequestRequestTypeDef](./type_defs.md#searchquantumtasksrequestrequesttypedef) 

### tag\_resource

Add a tag to the specified resource.

Type annotations and code completion for `#!python session.client("braket").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.tag_resource)

```python title="Method definition"
await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Remove tags from a resource.

Type annotations and code completion for `#!python session.client("braket").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.untag_resource)

```python title="Method definition"
await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("braket").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> BraketClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("braket").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.client("braket").get_paginator` method with overloads.

- `client.get_paginator("search_devices")` -> [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
- `client.get_paginator("search_jobs")` -> [SearchJobsPaginator](./paginators.md#searchjobspaginator)
- `client.get_paginator("search_quantum_tasks")` -> [SearchQuantumTasksPaginator](./paginators.md#searchquantumtaskspaginator)



