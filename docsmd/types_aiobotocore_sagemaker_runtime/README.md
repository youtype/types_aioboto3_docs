# SageMakerRuntime module

> [Index](../README.md) > SageMakerRuntime


!!! note ""

    Auto-generated documentation for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#sagemakerruntime)
    type annotations stubs module [types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aioboto3` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aioboto3==13.3.0' mypy_boto3_builder`
1. Select `aioboto3` AWS SDK.
1. Add `SageMakerRuntime` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aioboto3` for `SageMakerRuntime` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[sagemaker-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[sagemaker-runtime]'

# standalone installation
python -m pip install types-aiobotocore-sagemaker-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SageMakerRuntimeClient

Type annotations and code completion for  `#!python session.client("sagemaker-runtime")` as [SageMakerRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client)

```python
# SageMakerRuntimeClient usage example

from aioboto3.session import Session

from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient


session = Session()
async with session.client("sagemaker-runtime") as client:
    client: SageMakerRuntimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# SageMakerRuntimeServiceName usage example

from types_aiobotocore_sagemaker_runtime.literals import SageMakerRuntimeServiceName

def get_value() -> SageMakerRuntimeServiceName:
    return "sagemaker-runtime"
```

- [SageMakerRuntimeServiceName](./literals.md#sagemakerruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [InternalStreamFailureTypeDef](./type_defs.md#internalstreamfailuretypedef)
- [InvokeEndpointAsyncInputRequestTypeDef](./type_defs.md#invokeendpointasyncinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ModelStreamErrorTypeDef](./type_defs.md#modelstreamerrortypedef)
- [PayloadPartTypeDef](./type_defs.md#payloadparttypedef)
- [InvokeEndpointInputRequestTypeDef](./type_defs.md#invokeendpointinputrequesttypedef)
- [InvokeEndpointWithResponseStreamInputRequestTypeDef](./type_defs.md#invokeendpointwithresponsestreaminputrequesttypedef)
- [InvokeEndpointAsyncOutputTypeDef](./type_defs.md#invokeendpointasyncoutputtypedef)
- [InvokeEndpointOutputTypeDef](./type_defs.md#invokeendpointoutputtypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [InvokeEndpointWithResponseStreamOutputTypeDef](./type_defs.md#invokeendpointwithresponsestreamoutputtypedef)
