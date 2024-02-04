# BedrockRuntime module

> [Index](../README.md) > BedrockRuntime


!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## How to install



### From PyPI with pip

Install `types-aioboto3` for `BedrockRuntime` service.

```bash
# install with aioboto3 type annotations
python -m pip install 'types-aioboto3[bedrock-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aioboto3-lite[bedrock-runtime]'


# standalone installation
python -m pip install types-aiobotocore-bedrock-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BedrockRuntimeClient

Type annotations and code completion for  `#!python session.client("bedrock-runtime")` as [BedrockRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime.Client)

```python
# BedrockRuntimeClient usage example

from aioboto3.session import Session

from types_aiobotocore_bedrock_runtime.client import BedrockRuntimeClient


session = Session()
async with session.client("bedrock-runtime") as client:
    client: BedrockRuntimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BedrockRuntimeServiceName usage example

from types_aiobotocore_bedrock_runtime.literals import BedrockRuntimeServiceName

def get_value() -> BedrockRuntimeServiceName:
    return "bedrock-runtime"
```

- [BedrockRuntimeServiceName](./literals.md#bedrockruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ModelStreamErrorExceptionTypeDef](./type_defs.md#modelstreamerrorexceptiontypedef)
- [ModelTimeoutExceptionTypeDef](./type_defs.md#modeltimeoutexceptiontypedef)
- [PayloadPartTypeDef](./type_defs.md#payloadparttypedef)
- [ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
- [ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef)
- [InvokeModelRequestRequestTypeDef](./type_defs.md#invokemodelrequestrequesttypedef)
- [InvokeModelWithResponseStreamRequestRequestTypeDef](./type_defs.md#invokemodelwithresponsestreamrequestrequesttypedef)
- [InvokeModelResponseTypeDef](./type_defs.md#invokemodelresponsetypedef)
- [ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef)
- [InvokeModelWithResponseStreamResponseTypeDef](./type_defs.md#invokemodelwithresponsestreamresponsetypedef)

