# LaunchWizardClient

> [Index](../README.md) > [LaunchWizard](./README.md) > LaunchWizardClient

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## LaunchWizardClient

Type annotations and code completion for `#!python session.client("launch-wizard")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client)

```python
# LaunchWizardClient usage example

from aioboto3.session import Session
from types_aiobotocore_launch_wizard.client import LaunchWizardClient

session = Session()
async with session.client("launch-wizard") as client:
    client: LaunchWizardClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("launch-wizard").exceptions` structure.

```python
# LaunchWizardClient.exceptions usage example

async with session.client("launch-wizard") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InternalServerException,
        client.exceptions.ResourceLimitException,
        client.exceptions.ResourceNotFoundException,
        client.exceptions.ValidationException,
    ) as e:
        print(e)
```

```python
# LaunchWizardClient.exceptions type checking example

from types_aiobotocore_launch_wizard.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("launch-wizard").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.can_paginate)

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

Type annotations and code completion for `#!python session.client("launch-wizard").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_deployment

Creates a deployment for the given workload.

Type annotations and code completion for `#!python session.client("launch-wizard").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.create_deployment)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    deploymentPatternName: str,
    name: str,
    specifications: Mapping[str, str],
    workloadName: str,
    dryRun: bool = ...,
) -> CreateDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef) 


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentInputRequestTypeDef = {  # (1)
    "deploymentPatternName": ...,
    "name": ...,
    "specifications": ...,
    "workloadName": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentInputRequestTypeDef](./type_defs.md#createdeploymentinputrequesttypedef) 

### delete\_deployment

Deletes a deployment.

Type annotations and code completion for `#!python session.client("launch-wizard").delete_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.delete_deployment)

```python
# delete_deployment method definition

await def delete_deployment(
    self,
    *,
    deploymentId: str,
) -> DeleteDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDeploymentOutputTypeDef](./type_defs.md#deletedeploymentoutputtypedef) 


```python
# delete_deployment method usage example with argument unpacking

kwargs: DeleteDeploymentInputRequestTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.delete_deployment(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentInputRequestTypeDef](./type_defs.md#deletedeploymentinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("launch-wizard").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.generate_presigned_url)

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


### get\_deployment

Returns information about the deployment.

Type annotations and code completion for `#!python session.client("launch-wizard").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_deployment)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    deploymentId: str,
) -> GetDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentOutputTypeDef](./type_defs.md#getdeploymentoutputtypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentInputRequestTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentInputRequestTypeDef](./type_defs.md#getdeploymentinputrequesttypedef) 

### get\_workload

Returns information about a workload.

Type annotations and code completion for `#!python session.client("launch-wizard").get_workload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.get_workload)

```python
# get_workload method definition

await def get_workload(
    self,
    *,
    workloadName: str,
) -> GetWorkloadOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadOutputTypeDef](./type_defs.md#getworkloadoutputtypedef) 


```python
# get_workload method usage example with argument unpacking

kwargs: GetWorkloadInputRequestTypeDef = {  # (1)
    "workloadName": ...,
}

parent.get_workload(**kwargs)
```

1. See [:material-code-braces: GetWorkloadInputRequestTypeDef](./type_defs.md#getworkloadinputrequesttypedef) 

### list\_deployment\_events

Lists the events of a deployment.

Type annotations and code completion for `#!python session.client("launch-wizard").list_deployment_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployment_events)

```python
# list_deployment_events method definition

await def list_deployment_events(
    self,
    *,
    deploymentId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeploymentEventsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef) 


```python
# list_deployment_events method usage example with argument unpacking

kwargs: ListDeploymentEventsInputRequestTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.list_deployment_events(**kwargs)
```

1. See [:material-code-braces: ListDeploymentEventsInputRequestTypeDef](./type_defs.md#listdeploymenteventsinputrequesttypedef) 

### list\_deployments

Lists the deployments that have been created.

Type annotations and code completion for `#!python session.client("launch-wizard").list_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_deployments)

```python
# list_deployments method definition

await def list_deployments(
    self,
    *,
    filters: Sequence[DeploymentFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDeploymentsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
2. See [:material-code-braces: ListDeploymentsOutputTypeDef](./type_defs.md#listdeploymentsoutputtypedef) 


```python
# list_deployments method usage example with argument unpacking

kwargs: ListDeploymentsInputRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_deployments(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsInputRequestTypeDef](./type_defs.md#listdeploymentsinputrequesttypedef) 

### list\_workload\_deployment\_patterns

Lists the workload deployment patterns.

Type annotations and code completion for `#!python session.client("launch-wizard").list_workload_deployment_patterns` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_workload_deployment_patterns)

```python
# list_workload_deployment_patterns method definition

await def list_workload_deployment_patterns(
    self,
    *,
    workloadName: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkloadDeploymentPatternsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadDeploymentPatternsOutputTypeDef](./type_defs.md#listworkloaddeploymentpatternsoutputtypedef) 


```python
# list_workload_deployment_patterns method usage example with argument unpacking

kwargs: ListWorkloadDeploymentPatternsInputRequestTypeDef = {  # (1)
    "workloadName": ...,
}

parent.list_workload_deployment_patterns(**kwargs)
```

1. See [:material-code-braces: ListWorkloadDeploymentPatternsInputRequestTypeDef](./type_defs.md#listworkloaddeploymentpatternsinputrequesttypedef) 

### list\_workloads

Lists the workloads.

Type annotations and code completion for `#!python session.client("launch-wizard").list_workloads` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.list_workloads)

```python
# list_workloads method definition

await def list_workloads(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkloadsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadsOutputTypeDef](./type_defs.md#listworkloadsoutputtypedef) 


```python
# list_workloads method usage example with argument unpacking

kwargs: ListWorkloadsInputRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_workloads(**kwargs)
```

1. See [:material-code-braces: ListWorkloadsInputRequestTypeDef](./type_defs.md#listworkloadsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("launch-wizard").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> LaunchWizardClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("launch-wizard").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard.Client.__aexit__)

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

Type annotations and code completion for `#!python session.client("launch-wizard").get_paginator` method with overloads.

- `client.get_paginator("list_deployment_events")` -> [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
- `client.get_paginator("list_deployments")` -> [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
- `client.get_paginator("list_workload_deployment_patterns")` -> [ListWorkloadDeploymentPatternsPaginator](./paginators.md#listworkloaddeploymentpatternspaginator)
- `client.get_paginator("list_workloads")` -> [ListWorkloadsPaginator](./paginators.md#listworkloadspaginator)



