# Examples

> [Index](../README.md) > [SageMakerRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#sagemakerruntime)
    type annotations stubs module [types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[sagemaker-runtime]` package installed.

Write your `SageMakerRuntime` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SageMakerRuntimeClient usage example

from aioboto3.session import Session


session = Session()

async with session.client("sagemaker-runtime") as client:  # (1)
    result = await client.invoke_endpoint()  # (2)
```

1. client: [SageMakerRuntimeClient](./client.md)
2. result: [:material-code-braces: InvokeEndpointOutputTypeDef](./type_defs.md#invokeendpointoutputtypedef)






### Explicit type annotations

With `types-aioboto3-lite[sagemaker-runtime]`
or a standalone `types_aiobotocore_sagemaker_runtime` package, you have to explicitly specify
`client: SageMakerRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SageMakerRuntimeClient usage example with type annotations

from aioboto3.session import Session

from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient
from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointOutputTypeDef
from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointInputTypeDef


session = Session()

client: SageMakerRuntimeClient
async with session.client("sagemaker-runtime") as client:  # (1)
    kwargs: InvokeEndpointInputTypeDef = {...}  # (2)
    result: InvokeEndpointOutputTypeDef = await client.invoke_endpoint(**kwargs)  # (3)
```

1. client: [SageMakerRuntimeClient](./client.md)
2. kwargs: [:material-code-braces: InvokeEndpointInputTypeDef](./type_defs.md#invokeendpointinputtypedef)
3. result: [:material-code-braces: InvokeEndpointOutputTypeDef](./type_defs.md#invokeendpointoutputtypedef)






