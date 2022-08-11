# Waiters

> [Index](../README.md) > [Proton](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
    type annotations stubs module [types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).

## EnvironmentDeployedWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("environment_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.EnvironmentDeployed)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import EnvironmentDeployedWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: EnvironmentDeployedWaiter = client.get_waiter("environment_deployed")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [EnvironmentDeployedWaiter](./waiters.md#environmentdeployedwaiter)


### wait

Type annotations and code completion for `#!python EnvironmentDeployedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetEnvironmentInputEnvironmentDeployedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentInputEnvironmentDeployedWaitTypeDef](./type_defs.md#getenvironmentinputenvironmentdeployedwaittypedef) 
## EnvironmentTemplateVersionRegisteredWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("environment_template_version_registered")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.EnvironmentTemplateVersionRegistered)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import EnvironmentTemplateVersionRegisteredWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: EnvironmentTemplateVersionRegisteredWaiter = client.get_waiter("environment_template_version_registered")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [EnvironmentTemplateVersionRegisteredWaiter](./waiters.md#environmenttemplateversionregisteredwaiter)


### wait

Type annotations and code completion for `#!python EnvironmentTemplateVersionRegisteredWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef](./type_defs.md#getenvironmenttemplateversioninputenvironmenttemplateversionregisteredwaittypedef) 
## ServiceCreatedWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("service_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceCreated)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import ServiceCreatedWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: ServiceCreatedWaiter = client.get_waiter("service_created")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [ServiceCreatedWaiter](./waiters.md#servicecreatedwaiter)


### wait

Type annotations and code completion for `#!python ServiceCreatedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceInputServiceCreatedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetServiceInputServiceCreatedWaitTypeDef](./type_defs.md#getserviceinputservicecreatedwaittypedef) 
## ServiceDeletedWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("service_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceDeleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import ServiceDeletedWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: ServiceDeletedWaiter = client.get_waiter("service_deleted")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [ServiceDeletedWaiter](./waiters.md#servicedeletedwaiter)


### wait

Type annotations and code completion for `#!python ServiceDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceInputServiceDeletedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetServiceInputServiceDeletedWaitTypeDef](./type_defs.md#getserviceinputservicedeletedwaittypedef) 
## ServiceInstanceDeployedWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("service_instance_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceInstanceDeployed)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import ServiceInstanceDeployedWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: ServiceInstanceDeployedWaiter = client.get_waiter("service_instance_deployed")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [ServiceInstanceDeployedWaiter](./waiters.md#serviceinstancedeployedwaiter)


### wait

Type annotations and code completion for `#!python ServiceInstanceDeployedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    name: str,
    serviceName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef = {  # (1)
    "name": ...,
    "serviceName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef](./type_defs.md#getserviceinstanceinputserviceinstancedeployedwaittypedef) 
## ServicePipelineDeployedWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("service_pipeline_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServicePipelineDeployed)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import ServicePipelineDeployedWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: ServicePipelineDeployedWaiter = client.get_waiter("service_pipeline_deployed")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [ServicePipelineDeployedWaiter](./waiters.md#servicepipelinedeployedwaiter)


### wait

Type annotations and code completion for `#!python ServicePipelineDeployedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceInputServicePipelineDeployedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetServiceInputServicePipelineDeployedWaitTypeDef](./type_defs.md#getserviceinputservicepipelinedeployedwaittypedef) 
## ServiceTemplateVersionRegisteredWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("service_template_version_registered")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceTemplateVersionRegistered)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import ServiceTemplateVersionRegisteredWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: ServiceTemplateVersionRegisteredWaiter = client.get_waiter("service_template_version_registered")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [ServiceTemplateVersionRegisteredWaiter](./waiters.md#servicetemplateversionregisteredwaiter)


### wait

Type annotations and code completion for `#!python ServiceTemplateVersionRegisteredWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef = {  # (1)
    "majorVersion": ...,
    "minorVersion": ...,
    "templateName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef](./type_defs.md#getservicetemplateversioninputservicetemplateversionregisteredwaittypedef) 
## ServiceUpdatedWaiter

Type annotations and code completion for `#!python session.client("proton").get_waiter("service_updated")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Waiter.ServiceUpdated)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_proton.waiter import ServiceUpdatedWaiter

session = get_session()
async with session.client("proton") as client:  # (1)
    waiter: ServiceUpdatedWaiter = client.get_waiter("service_updated")  # (2)
    await waiter.wait()
```

1. client: [ProtonClient](./client.md)
2. waiter: [ServiceUpdatedWaiter](./waiters.md#serviceupdatedwaiter)


### wait

Type annotations and code completion for `#!python ServiceUpdatedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    name: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetServiceInputServiceUpdatedWaitTypeDef = {  # (1)
    "name": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetServiceInputServiceUpdatedWaitTypeDef](./type_defs.md#getserviceinputserviceupdatedwaittypedef) 
