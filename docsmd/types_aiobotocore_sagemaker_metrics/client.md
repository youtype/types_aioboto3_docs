# SageMakerMetricsClient

> [Index](../README.md) > [SageMakerMetrics](./README.md) > SageMakerMetricsClient

!!! note ""

    Auto-generated documentation for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#sagemakermetrics)
    type annotations stubs module [types-aiobotocore-sagemaker-metrics](https://pypi.org/project/types-aiobotocore-sagemaker-metrics/).

## SageMakerMetricsClient

Type annotations and code completion for `#!python session.client("sagemaker-metrics")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

```python
# SageMakerMetricsClient usage example

from aioboto3.session import Session
from types_aiobotocore_sagemaker_metrics.client import SageMakerMetricsClient

session = Session()
async with session.client("sagemaker-metrics") as client:
    client: SageMakerMetricsClient
```

## Exceptions


`aioboto3` client exceptions are generated in runtime.
This class provides code completion for `#!python session.client("sagemaker-metrics").exceptions` structure.

```python
# SageMakerMetricsClient.exceptions usage example

async with session.client("sagemaker-metrics") as client:
    try:
        do_something(client)
    except (
            client.exceptions.ClientError,
    ) as e:
        print(e)
```

```python
# SageMakerMetricsClient.exceptions type checking example

from types_aiobotocore_sagemaker_metrics.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.client("sagemaker-metrics").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.client("sagemaker-metrics").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

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


### batch\_get\_metrics

Used to retrieve training metrics from SageMaker.

Type annotations and code completion for `#!python session.client("sagemaker-metrics").batch_get_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

```python
# batch_get_metrics method definition

await def batch_get_metrics(
    self,
    *,
    MetricQueries: Sequence[MetricQueryTypeDef],  # (1)
) -> BatchGetMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MetricQueryTypeDef](./type_defs.md#metricquerytypedef) 
2. See [:material-code-braces: BatchGetMetricsResponseTypeDef](./type_defs.md#batchgetmetricsresponsetypedef) 


```python
# batch_get_metrics method usage example with argument unpacking

kwargs: BatchGetMetricsRequestRequestTypeDef = {  # (1)
    "MetricQueries": ...,
}

parent.batch_get_metrics(**kwargs)
```

1. See [:material-code-braces: BatchGetMetricsRequestRequestTypeDef](./type_defs.md#batchgetmetricsrequestrequesttypedef) 

### batch\_put\_metrics

Used to ingest training metrics into SageMaker.

Type annotations and code completion for `#!python session.client("sagemaker-metrics").batch_put_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

```python
# batch_put_metrics method definition

await def batch_put_metrics(
    self,
    *,
    TrialComponentName: str,
    MetricData: Sequence[RawMetricDataTypeDef],  # (1)
) -> BatchPutMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RawMetricDataTypeDef](./type_defs.md#rawmetricdatatypedef) 
2. See [:material-code-braces: BatchPutMetricsResponseTypeDef](./type_defs.md#batchputmetricsresponsetypedef) 


```python
# batch_put_metrics method usage example with argument unpacking

kwargs: BatchPutMetricsRequestRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
    "MetricData": ...,
}

parent.batch_put_metrics(**kwargs)
```

1. See [:material-code-braces: BatchPutMetricsRequestRequestTypeDef](./type_defs.md#batchputmetricsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.client("sagemaker-metrics").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.client("sagemaker-metrics").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

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




