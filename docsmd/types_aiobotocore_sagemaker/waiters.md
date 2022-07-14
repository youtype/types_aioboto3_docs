# Waiters

> [Index](../README.md) > [SageMaker](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
    type annotations stubs module [types-aiobotocore-sagemaker](https://pypi.org/project/types-aiobotocore-sagemaker/).

## EndpointDeletedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("endpoint_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.EndpointDeleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import EndpointDeletedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: EndpointDeletedWaiter = client.get_waiter("endpoint_deleted")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


### wait

Type annotations and code completion for `#!python EndpointDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    EndpointName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEndpointInputEndpointDeletedWaitTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointInputEndpointDeletedWaitTypeDef](./type_defs.md#describeendpointinputendpointdeletedwaittypedef) 
## EndpointInServiceWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("endpoint_in_service")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.EndpointInService)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import EndpointInServiceWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: EndpointInServiceWaiter = client.get_waiter("endpoint_in_service")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [EndpointInServiceWaiter](./waiters.md#endpointinservicewaiter)


### wait

Type annotations and code completion for `#!python EndpointInServiceWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    EndpointName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEndpointInputEndpointInServiceWaitTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointInputEndpointInServiceWaitTypeDef](./type_defs.md#describeendpointinputendpointinservicewaittypedef) 
## ImageCreatedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("image_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageCreated)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import ImageCreatedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: ImageCreatedWaiter = client.get_waiter("image_created")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [ImageCreatedWaiter](./waiters.md#imagecreatedwaiter)


### wait

Type annotations and code completion for `#!python ImageCreatedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ImageName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageRequestImageCreatedWaitTypeDef = {  # (1)
    "ImageName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImageRequestImageCreatedWaitTypeDef](./type_defs.md#describeimagerequestimagecreatedwaittypedef) 
## ImageDeletedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("image_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageDeleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import ImageDeletedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: ImageDeletedWaiter = client.get_waiter("image_deleted")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [ImageDeletedWaiter](./waiters.md#imagedeletedwaiter)


### wait

Type annotations and code completion for `#!python ImageDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ImageName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageRequestImageDeletedWaitTypeDef = {  # (1)
    "ImageName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImageRequestImageDeletedWaitTypeDef](./type_defs.md#describeimagerequestimagedeletedwaittypedef) 
## ImageUpdatedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("image_updated")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageUpdated)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import ImageUpdatedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: ImageUpdatedWaiter = client.get_waiter("image_updated")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [ImageUpdatedWaiter](./waiters.md#imageupdatedwaiter)


### wait

Type annotations and code completion for `#!python ImageUpdatedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ImageName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageRequestImageUpdatedWaitTypeDef = {  # (1)
    "ImageName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImageRequestImageUpdatedWaitTypeDef](./type_defs.md#describeimagerequestimageupdatedwaittypedef) 
## ImageVersionCreatedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("image_version_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageVersionCreated)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import ImageVersionCreatedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: ImageVersionCreatedWaiter = client.get_waiter("image_version_created")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [ImageVersionCreatedWaiter](./waiters.md#imageversioncreatedwaiter)


### wait

Type annotations and code completion for `#!python ImageVersionCreatedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ImageName: str,
    Version: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageVersionRequestImageVersionCreatedWaitTypeDef = {  # (1)
    "ImageName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImageVersionRequestImageVersionCreatedWaitTypeDef](./type_defs.md#describeimageversionrequestimageversioncreatedwaittypedef) 
## ImageVersionDeletedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("image_version_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageVersionDeleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import ImageVersionDeletedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: ImageVersionDeletedWaiter = client.get_waiter("image_version_deleted")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [ImageVersionDeletedWaiter](./waiters.md#imageversiondeletedwaiter)


### wait

Type annotations and code completion for `#!python ImageVersionDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ImageName: str,
    Version: int = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImageVersionRequestImageVersionDeletedWaitTypeDef = {  # (1)
    "ImageName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeImageVersionRequestImageVersionDeletedWaitTypeDef](./type_defs.md#describeimageversionrequestimageversiondeletedwaittypedef) 
## NotebookInstanceDeletedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("notebook_instance_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.NotebookInstanceDeleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import NotebookInstanceDeletedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: NotebookInstanceDeletedWaiter = client.get_waiter("notebook_instance_deleted")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [NotebookInstanceDeletedWaiter](./waiters.md#notebookinstancedeletedwaiter)


### wait

Type annotations and code completion for `#!python NotebookInstanceDeletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    NotebookInstanceName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNotebookInstanceInputNotebookInstanceDeletedWaitTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNotebookInstanceInputNotebookInstanceDeletedWaitTypeDef](./type_defs.md#describenotebookinstanceinputnotebookinstancedeletedwaittypedef) 
## NotebookInstanceInServiceWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("notebook_instance_in_service")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.NotebookInstanceInService)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import NotebookInstanceInServiceWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: NotebookInstanceInServiceWaiter = client.get_waiter("notebook_instance_in_service")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [NotebookInstanceInServiceWaiter](./waiters.md#notebookinstanceinservicewaiter)


### wait

Type annotations and code completion for `#!python NotebookInstanceInServiceWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    NotebookInstanceName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNotebookInstanceInputNotebookInstanceInServiceWaitTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNotebookInstanceInputNotebookInstanceInServiceWaitTypeDef](./type_defs.md#describenotebookinstanceinputnotebookinstanceinservicewaittypedef) 
## NotebookInstanceStoppedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("notebook_instance_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.NotebookInstanceStopped)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import NotebookInstanceStoppedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: NotebookInstanceStoppedWaiter = client.get_waiter("notebook_instance_stopped")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [NotebookInstanceStoppedWaiter](./waiters.md#notebookinstancestoppedwaiter)


### wait

Type annotations and code completion for `#!python NotebookInstanceStoppedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    NotebookInstanceName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNotebookInstanceInputNotebookInstanceStoppedWaitTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNotebookInstanceInputNotebookInstanceStoppedWaitTypeDef](./type_defs.md#describenotebookinstanceinputnotebookinstancestoppedwaittypedef) 
## ProcessingJobCompletedOrStoppedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("processing_job_completed_or_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ProcessingJobCompletedOrStopped)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import ProcessingJobCompletedOrStoppedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: ProcessingJobCompletedOrStoppedWaiter = client.get_waiter("processing_job_completed_or_stopped")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [ProcessingJobCompletedOrStoppedWaiter](./waiters.md#processingjobcompletedorstoppedwaiter)


### wait

Type annotations and code completion for `#!python ProcessingJobCompletedOrStoppedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    ProcessingJobName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeProcessingJobRequestProcessingJobCompletedOrStoppedWaitTypeDef = {  # (1)
    "ProcessingJobName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeProcessingJobRequestProcessingJobCompletedOrStoppedWaitTypeDef](./type_defs.md#describeprocessingjobrequestprocessingjobcompletedorstoppedwaittypedef) 
## TrainingJobCompletedOrStoppedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("training_job_completed_or_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.TrainingJobCompletedOrStopped)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import TrainingJobCompletedOrStoppedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: TrainingJobCompletedOrStoppedWaiter = client.get_waiter("training_job_completed_or_stopped")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [TrainingJobCompletedOrStoppedWaiter](./waiters.md#trainingjobcompletedorstoppedwaiter)


### wait

Type annotations and code completion for `#!python TrainingJobCompletedOrStoppedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    TrainingJobName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTrainingJobRequestTrainingJobCompletedOrStoppedWaitTypeDef = {  # (1)
    "TrainingJobName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTrainingJobRequestTrainingJobCompletedOrStoppedWaitTypeDef](./type_defs.md#describetrainingjobrequesttrainingjobcompletedorstoppedwaittypedef) 
## TransformJobCompletedOrStoppedWaiter

Type annotations and code completion for `#!python session.client("sagemaker").get_waiter("transform_job_completed_or_stopped")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.TransformJobCompletedOrStopped)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_sagemaker.waiter import TransformJobCompletedOrStoppedWaiter

session = get_session()
async with session.client("sagemaker") as client:  # (1)
    waiter: TransformJobCompletedOrStoppedWaiter = client.get_waiter("transform_job_completed_or_stopped")  # (2)
    await waiter.wait()
```

1. client: [SageMakerClient](./client.md)
2. waiter: [TransformJobCompletedOrStoppedWaiter](./waiters.md#transformjobcompletedorstoppedwaiter)


### wait

Type annotations and code completion for `#!python TransformJobCompletedOrStoppedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    TransformJobName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransformJobRequestTransformJobCompletedOrStoppedWaitTypeDef = {  # (1)
    "TransformJobName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTransformJobRequestTransformJobCompletedOrStoppedWaitTypeDef](./type_defs.md#describetransformjobrequesttransformjobcompletedorstoppedwaittypedef) 
