# Waiters

> [Index](../README.md) > [CloudFront](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
    type annotations stubs module [types-aiobotocore-cloudfront](https://pypi.org/project/types-aiobotocore-cloudfront/).

## DistributionDeployedWaiter

Type annotations and code completion for `#!python session.client("cloudfront").get_waiter("distribution_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Waiter.DistributionDeployed)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cloudfront.waiter import DistributionDeployedWaiter

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    waiter: DistributionDeployedWaiter = client.get_waiter("distribution_deployed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [DistributionDeployedWaiter](./waiters.md#distributiondeployedwaiter)


### wait

Type annotations and code completion for `#!python DistributionDeployedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetDistributionRequestDistributionDeployedWaitTypeDef = {  # (1)
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetDistributionRequestDistributionDeployedWaitTypeDef](./type_defs.md#getdistributionrequestdistributiondeployedwaittypedef) 
## InvalidationCompletedWaiter

Type annotations and code completion for `#!python session.client("cloudfront").get_waiter("invalidation_completed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Waiter.InvalidationCompleted)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cloudfront.waiter import InvalidationCompletedWaiter

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    waiter: InvalidationCompletedWaiter = client.get_waiter("invalidation_completed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [InvalidationCompletedWaiter](./waiters.md#invalidationcompletedwaiter)


### wait

Type annotations and code completion for `#!python InvalidationCompletedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    DistributionId: str,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetInvalidationRequestInvalidationCompletedWaitTypeDef = {  # (1)
    "DistributionId": ...,
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetInvalidationRequestInvalidationCompletedWaitTypeDef](./type_defs.md#getinvalidationrequestinvalidationcompletedwaittypedef) 
## StreamingDistributionDeployedWaiter

Type annotations and code completion for `#!python session.client("cloudfront").get_waiter("streaming_distribution_deployed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Waiter.StreamingDistributionDeployed)

```python title="Usage example"
from aioboto3.session import Session

from types_aiobotocore_cloudfront.waiter import StreamingDistributionDeployedWaiter

session = get_session()
async with session.client("cloudfront") as client:  # (1)
    waiter: StreamingDistributionDeployedWaiter = client.get_waiter("streaming_distribution_deployed")  # (2)
    await waiter.wait()
```

1. client: [CloudFrontClient](./client.md)
2. waiter: [StreamingDistributionDeployedWaiter](./waiters.md#streamingdistributiondeployedwaiter)


### wait

Type annotations and code completion for `#!python StreamingDistributionDeployedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    Id: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = {  # (1)
    "Id": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef](./type_defs.md#getstreamingdistributionrequeststreamingdistributiondeployedwaittypedef) 
