# EMRServerlessClient

> [Index](../README.md) > [EMRServerless](./README.md) > EMRServerlessClient

!!! note ""

    Auto-generated documentation for [EMRServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#emrserverless)
    type annotations stubs module [types-aiobotocore-emr-serverless](https://pypi.org/project/types-aiobotocore-emr-serverless/).

## EMRServerlessClient

Type annotations and code completion for `#!python session.client("emr-serverless")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# EMRServerlessClient usage example

from aioboto3.session import Session
from types_aiobotocore_emr_serverless.client import EMRServerlessClient

session = Session()
async with session.client("emr-serverless") as client:
    client: EMRServerlessClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("emr-serverless").exceptions` structure.

```python
# EMRServerlessClient.exceptions usage example

async with session.client("emr-serverless") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.ConflictException,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ServiceQuotaExceededException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# EMRServerlessClient.exceptions type checking example

from types_aiobotocore_emr_serverless.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("emr-serverless").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("emr-serverless").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

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


### cancel\_job\_run

Cancels a job run.

Type annotations and code completion for `#!python session.client("emr-serverless").cancel_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# cancel_job_run method definition

await def cancel_job_run(
    self,
    *,
    applicationId: str,
    jobRunId: str,
) -> CancelJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef)


```python
# cancel_job_run method usage example with argument unpacking

kwargs: CancelJobRunRequestTypeDef = {  # (1)
    "applicationId": ...,
    "jobRunId": ...,
}

parent.cancel_job_run(**kwargs)
```

1. See [:material-code-braces: CancelJobRunRequestTypeDef](./type_defs.md#canceljobrunrequesttypedef)

### create\_application

Creates an application.

Type annotations and code completion for `#!python session.client("emr-serverless").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# create_application method definition

await def create_application(
    self,
    *,
    releaseLabel: str,
    type: str,
    clientToken: str,
    name: str = ...,
    initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,  # (1)
    maximumCapacity: MaximumAllowedResourcesTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    autoStartConfiguration: AutoStartConfigTypeDef = ...,  # (3)
    autoStopConfiguration: AutoStopConfigTypeDef = ...,  # (4)
    networkConfiguration: NetworkConfigurationUnionTypeDef = ...,  # (5)
    architecture: ArchitectureType = ...,  # (6)
    imageConfiguration: ImageConfigurationInputTypeDef = ...,  # (7)
    workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,  # (8)
    runtimeConfiguration: Sequence[ConfigurationUnionTypeDef] = ...,  # (9)
    monitoringConfiguration: MonitoringConfigurationUnionTypeDef = ...,  # (10)
    interactiveConfiguration: InteractiveConfigurationTypeDef = ...,  # (11)
    schedulerConfiguration: SchedulerConfigurationTypeDef = ...,  # (12)
) -> CreateApplicationResponseTypeDef:  # (13)
    ...
```

1. See `Mapping[str, InitialCapacityConfigTypeDef]`
2. See [:material-code-braces: MaximumAllowedResourcesTypeDef](./type_defs.md#maximumallowedresourcestypedef)
3. See [:material-code-braces: AutoStartConfigTypeDef](./type_defs.md#autostartconfigtypedef)
4. See [:material-code-braces: AutoStopConfigTypeDef](./type_defs.md#autostopconfigtypedef)
5. See [:material-code-braces: NetworkConfigurationUnionTypeDef](#networkconfigurationuniontypedef)
6. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype)
7. See [:material-code-braces: ImageConfigurationInputTypeDef](./type_defs.md#imageconfigurationinputtypedef)
8. See `Mapping[str, WorkerTypeSpecificationInputTypeDef]`
9. See `Sequence[ConfigurationUnionTypeDef]`
10. See [:material-code-braces: MonitoringConfigurationUnionTypeDef](#monitoringconfigurationuniontypedef)
11. See [:material-code-braces: InteractiveConfigurationTypeDef](./type_defs.md#interactiveconfigurationtypedef)
12. See [:material-code-braces: SchedulerConfigurationTypeDef](./type_defs.md#schedulerconfigurationtypedef)
13. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestTypeDef = {  # (1)
    "releaseLabel": ...,
    "type": ...,
    "clientToken": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef)

### delete\_application

Deletes an application.

Type annotations and code completion for `#!python session.client("emr-serverless").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestTypeDef](./type_defs.md#deleteapplicationrequesttypedef)

### get\_application

Displays detailed information about a specified application.

Type annotations and code completion for `#!python session.client("emr-serverless").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# get_application method definition

await def get_application(
    self,
    *,
    applicationId: str,
) -> GetApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef)


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationRequestTypeDef](./type_defs.md#getapplicationrequesttypedef)

### get\_dashboard\_for\_job\_run

Creates and returns a URL that you can use to access the application UIs for a
job run.

Type annotations and code completion for `#!python session.client("emr-serverless").get_dashboard_for_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# get_dashboard_for_job_run method definition

await def get_dashboard_for_job_run(
    self,
    *,
    applicationId: str,
    jobRunId: str,
    attempt: int = ...,
    accessSystemProfileLogs: bool = ...,
) -> GetDashboardForJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDashboardForJobRunResponseTypeDef](./type_defs.md#getdashboardforjobrunresponsetypedef)


```python
# get_dashboard_for_job_run method usage example with argument unpacking

kwargs: GetDashboardForJobRunRequestTypeDef = {  # (1)
    "applicationId": ...,
    "jobRunId": ...,
}

parent.get_dashboard_for_job_run(**kwargs)
```

1. See [:material-code-braces: GetDashboardForJobRunRequestTypeDef](./type_defs.md#getdashboardforjobrunrequesttypedef)

### get\_job\_run

Displays detailed information about a job run.

Type annotations and code completion for `#!python session.client("emr-serverless").get_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# get_job_run method definition

await def get_job_run(
    self,
    *,
    applicationId: str,
    jobRunId: str,
    attempt: int = ...,
) -> GetJobRunResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetJobRunResponseTypeDef](./type_defs.md#getjobrunresponsetypedef)


```python
# get_job_run method usage example with argument unpacking

kwargs: GetJobRunRequestTypeDef = {  # (1)
    "applicationId": ...,
    "jobRunId": ...,
}

parent.get_job_run(**kwargs)
```

1. See [:material-code-braces: GetJobRunRequestTypeDef](./type_defs.md#getjobrunrequesttypedef)

### list\_applications

Lists applications based on a set of parameters.

Type annotations and code completion for `#!python session.client("emr-serverless").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    states: Sequence[ApplicationStateType] = ...,  # (1)
) -> ListApplicationsResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[ApplicationStateType]`
2. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestTypeDef](./type_defs.md#listapplicationsrequesttypedef)

### list\_job\_run\_attempts

Lists all attempt of a job run.

Type annotations and code completion for `#!python session.client("emr-serverless").list_job_run_attempts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# list_job_run_attempts method definition

await def list_job_run_attempts(
    self,
    *,
    applicationId: str,
    jobRunId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListJobRunAttemptsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListJobRunAttemptsResponseTypeDef](./type_defs.md#listjobrunattemptsresponsetypedef)


```python
# list_job_run_attempts method usage example with argument unpacking

kwargs: ListJobRunAttemptsRequestTypeDef = {  # (1)
    "applicationId": ...,
    "jobRunId": ...,
}

parent.list_job_run_attempts(**kwargs)
```

1. See [:material-code-braces: ListJobRunAttemptsRequestTypeDef](./type_defs.md#listjobrunattemptsrequesttypedef)

### list\_job\_runs

Lists job runs based on a set of parameters.

Type annotations and code completion for `#!python session.client("emr-serverless").list_job_runs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# list_job_runs method definition

await def list_job_runs(
    self,
    *,
    applicationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    createdAtAfter: TimestampTypeDef = ...,
    createdAtBefore: TimestampTypeDef = ...,
    states: Sequence[JobRunStateType] = ...,  # (1)
    mode: JobRunModeType = ...,  # (2)
) -> ListJobRunsResponseTypeDef:  # (3)
    ...
```

1. See `Sequence[JobRunStateType]`
2. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype)
3. See [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef)


```python
# list_job_runs method usage example with argument unpacking

kwargs: ListJobRunsRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_job_runs(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestTypeDef](./type_defs.md#listjobrunsrequesttypedef)

### list\_tags\_for\_resource

Lists the tags assigned to the resources.

Type annotations and code completion for `#!python session.client("emr-serverless").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

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

### start\_application

Starts a specified application and initializes initial capacity if configured.

Type annotations and code completion for `#!python session.client("emr-serverless").start_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# start_application method definition

await def start_application(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```

```python
# start_application method usage example with argument unpacking

kwargs: StartApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.start_application(**kwargs)
```

1. See [:material-code-braces: StartApplicationRequestTypeDef](./type_defs.md#startapplicationrequesttypedef)

### start\_job\_run

Starts a job run.

Type annotations and code completion for `#!python session.client("emr-serverless").start_job_run` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# start_job_run method definition

await def start_job_run(
    self,
    *,
    applicationId: str,
    clientToken: str,
    executionRoleArn: str,
    jobDriver: JobDriverUnionTypeDef = ...,  # (1)
    configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    executionTimeoutMinutes: int = ...,
    name: str = ...,
    mode: JobRunModeType = ...,  # (3)
    retryPolicy: RetryPolicyTypeDef = ...,  # (4)
) -> StartJobRunResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: JobDriverUnionTypeDef](#jobdriveruniontypedef)
2. See [:material-code-braces: ConfigurationOverridesUnionTypeDef](#configurationoverridesuniontypedef)
3. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype)
4. See [:material-code-braces: RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef)
5. See [:material-code-braces: StartJobRunResponseTypeDef](./type_defs.md#startjobrunresponsetypedef)


```python
# start_job_run method usage example with argument unpacking

kwargs: StartJobRunRequestTypeDef = {  # (1)
    "applicationId": ...,
    "clientToken": ...,
    "executionRoleArn": ...,
}

parent.start_job_run(**kwargs)
```

1. See [:material-code-braces: StartJobRunRequestTypeDef](./type_defs.md#startjobrunrequesttypedef)

### stop\_application

Stops a specified application and releases initial capacity if configured.

Type annotations and code completion for `#!python session.client("emr-serverless").stop_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# stop_application method definition

await def stop_application(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```

```python
# stop_application method usage example with argument unpacking

kwargs: StopApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.stop_application(**kwargs)
```

1. See [:material-code-braces: StopApplicationRequestTypeDef](./type_defs.md#stopapplicationrequesttypedef)

### tag\_resource

Assigns tags to resources.

Type annotations and code completion for `#!python session.client("emr-serverless").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

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

Removes tags from resources.

Type annotations and code completion for `#!python session.client("emr-serverless").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

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

### update\_application

Updates a specified application.

Type annotations and code completion for `#!python session.client("emr-serverless").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# update_application method definition

await def update_application(
    self,
    *,
    applicationId: str,
    clientToken: str,
    initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,  # (1)
    maximumCapacity: MaximumAllowedResourcesTypeDef = ...,  # (2)
    autoStartConfiguration: AutoStartConfigTypeDef = ...,  # (3)
    autoStopConfiguration: AutoStopConfigTypeDef = ...,  # (4)
    networkConfiguration: NetworkConfigurationUnionTypeDef = ...,  # (5)
    architecture: ArchitectureType = ...,  # (6)
    imageConfiguration: ImageConfigurationInputTypeDef = ...,  # (7)
    workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,  # (8)
    interactiveConfiguration: InteractiveConfigurationTypeDef = ...,  # (9)
    releaseLabel: str = ...,
    runtimeConfiguration: Sequence[ConfigurationUnionTypeDef] = ...,  # (10)
    monitoringConfiguration: MonitoringConfigurationUnionTypeDef = ...,  # (11)
    schedulerConfiguration: SchedulerConfigurationTypeDef = ...,  # (12)
) -> UpdateApplicationResponseTypeDef:  # (13)
    ...
```

1. See `Mapping[str, InitialCapacityConfigTypeDef]`
2. See [:material-code-braces: MaximumAllowedResourcesTypeDef](./type_defs.md#maximumallowedresourcestypedef)
3. See [:material-code-braces: AutoStartConfigTypeDef](./type_defs.md#autostartconfigtypedef)
4. See [:material-code-braces: AutoStopConfigTypeDef](./type_defs.md#autostopconfigtypedef)
5. See [:material-code-braces: NetworkConfigurationUnionTypeDef](#networkconfigurationuniontypedef)
6. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype)
7. See [:material-code-braces: ImageConfigurationInputTypeDef](./type_defs.md#imageconfigurationinputtypedef)
8. See `Mapping[str, WorkerTypeSpecificationInputTypeDef]`
9. See [:material-code-braces: InteractiveConfigurationTypeDef](./type_defs.md#interactiveconfigurationtypedef)
10. See `Sequence[ConfigurationUnionTypeDef]`
11. See [:material-code-braces: MonitoringConfigurationUnionTypeDef](#monitoringconfigurationuniontypedef)
12. See [:material-code-braces: SchedulerConfigurationTypeDef](./type_defs.md#schedulerconfigurationtypedef)
13. See [:material-code-braces: UpdateApplicationResponseTypeDef](./type_defs.md#updateapplicationresponsetypedef)


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestTypeDef = {  # (1)
    "applicationId": ...,
    "clientToken": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestTypeDef](./type_defs.md#updateapplicationrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("emr-serverless").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("emr-serverless").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)

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

Type annotations and code completion for `#!python session.client("emr-serverless").get_paginator` method with overloads.

- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_job_run_attempts")` -> [ListJobRunAttemptsPaginator](./paginators.md#listjobrunattemptspaginator)
- `client.get_paginator("list_job_runs")` -> [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)



