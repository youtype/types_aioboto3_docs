# SagemakerEdgeManagerClient

> [Index](../README.md) > [SagemakerEdgeManager](./README.md) > SagemakerEdgeManagerClient

!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#sagemakeredgemanager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## SagemakerEdgeManagerClient

Type annotations and code completion for `#!python session.client("sagemaker-edge")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python
# SagemakerEdgeManagerClient usage example

from aioboto3.session import Session
from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient

session = Session()
async with session.client("sagemaker-edge") as client:
    client: SagemakerEdgeManagerClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("sagemaker-edge").exceptions` structure.

```python
# SagemakerEdgeManagerClient.exceptions usage example

async with session.client("sagemaker-edge") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
        client.exceptions.InternalServiceException,
    ) as e:
        print(e)
```

```python
# SagemakerEdgeManagerClient.exceptions type checking example

from types_aiobotocore_sagemaker_edge.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("sagemaker-edge").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("sagemaker-edge").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

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


### get\_deployments

Use to get the active deployments from a device.

Type annotations and code completion for `#!python session.client("sagemaker-edge").get_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python
# get_deployments method definition

await def get_deployments(
    self,
    *,
    DeviceName: str,
    DeviceFleetName: str,
) -> GetDeploymentsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeploymentsResultTypeDef](./type_defs.md#getdeploymentsresulttypedef) 


```python
# get_deployments method usage example with argument unpacking

kwargs: GetDeploymentsRequestRequestTypeDef = {  # (1)
    "DeviceName": ...,
    "DeviceFleetName": ...,
}

parent.get_deployments(**kwargs)
```

1. See [:material-code-braces: GetDeploymentsRequestRequestTypeDef](./type_defs.md#getdeploymentsrequestrequesttypedef) 

### get\_device\_registration

Use to check if a device is registered with SageMaker Edge Manager.

Type annotations and code completion for `#!python session.client("sagemaker-edge").get_device_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python
# get_device_registration method definition

await def get_device_registration(
    self,
    *,
    DeviceName: str,
    DeviceFleetName: str,
) -> GetDeviceRegistrationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef) 


```python
# get_device_registration method usage example with argument unpacking

kwargs: GetDeviceRegistrationRequestRequestTypeDef = {  # (1)
    "DeviceName": ...,
    "DeviceFleetName": ...,
}

parent.get_device_registration(**kwargs)
```

1. See [:material-code-braces: GetDeviceRegistrationRequestRequestTypeDef](./type_defs.md#getdeviceregistrationrequestrequesttypedef) 

### send\_heartbeat

Use to get the current status of devices registered on SageMaker Edge Manager.

Type annotations and code completion for `#!python session.client("sagemaker-edge").send_heartbeat` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python
# send_heartbeat method definition

await def send_heartbeat(
    self,
    *,
    AgentVersion: str,
    DeviceName: str,
    DeviceFleetName: str,
    AgentMetrics: Sequence[EdgeMetricTypeDef] = ...,  # (1)
    Models: Sequence[ModelTypeDef] = ...,  # (2)
    DeploymentResult: DeploymentResultTypeDef = ...,  # (3)
) -> EmptyResponseMetadataTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef) 
2. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
3. See [:material-code-braces: DeploymentResultTypeDef](./type_defs.md#deploymentresulttypedef) 
4. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# send_heartbeat method usage example with argument unpacking

kwargs: SendHeartbeatRequestRequestTypeDef = {  # (1)
    "AgentVersion": ...,
    "DeviceName": ...,
    "DeviceFleetName": ...,
}

parent.send_heartbeat(**kwargs)
```

1. See [:material-code-braces: SendHeartbeatRequestRequestTypeDef](./type_defs.md#sendheartbeatrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("sagemaker-edge").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("sagemaker-edge").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

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




