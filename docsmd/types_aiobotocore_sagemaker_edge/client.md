# SagemakerEdgeManagerClient

> [Index](../README.md) > [SagemakerEdgeManager](./README.md) > SagemakerEdgeManagerClient

!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## SagemakerEdgeManagerClient

Type annotations and code completion for `#!python session.client("sagemaker-edge")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python title="Usage example"
from aioboto3.session import Session
from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient

session = Session()
async with session.client("sagemaker-edge") as client:
    client: SagemakerEdgeManagerClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("sagemaker-edge").exceptions` structure.

```python title="Usage example"
async with session.client("sagemaker-edge") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServiceException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_sagemaker_edge.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.client("sagemaker-edge").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.client("sagemaker-edge").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.generate_presigned_url)

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


### get\_device\_registration

Use to check if a device is registered with SageMaker Edge Manager.

Type annotations and code completion for `#!python session.client("sagemaker-edge").get_device_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.get_device_registration)

```python title="Method definition"
await def get_device_registration(
    self,
    *,
    DeviceName: str,
    DeviceFleetName: str,
) -> GetDeviceRegistrationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef) 


```python title="Usage example with kwargs"
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.send_heartbeat)

```python title="Method definition"
await def send_heartbeat(
    self,
    *,
    AgentVersion: str,
    DeviceName: str,
    DeviceFleetName: str,
    AgentMetrics: Sequence[EdgeMetricTypeDef] = ...,  # (1)
    Models: Sequence[ModelTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef) 
2. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> SagemakerEdgeManagerClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("sagemaker-edge").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





